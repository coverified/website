<script>
  import Button from "../components/Button.svelte";
  import Container from "sveltestrap/src/Container.svelte";
  import { onMount } from 'svelte';

  onMount(() => {
        const faders = document.querySelectorAll('.fade-in');
        const appearOptions = {
            threshold: 0,
            rootMargin: '0px 0px -300px 0px'
        };
        const appearOnScroll = new IntersectionObserver(function(entries, appearOnScroll) {
        entries.forEach(entry => {
            if (!entry.isIntersecting) {
                return;
            } else {
                entry.target.classList.add('appear');
                appearOnScroll.unobserve(entry.target);
            }
        });
    }, appearOptions);

    faders.forEach(fader => {        
        appearOnScroll.observe(fader);
    })    
  });
</script>

<style type="text/scss">
   .bg-primary {
        position: relative;
        background-color: var(--color-primary) !important;
        z-index: 100;
        padding-top: 5rem;
        padding-bottom: 5rem;
        text-align: left;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 6rem 17.5rem 20rem 20rem 38rem 15rem;        
        color: var(--color-white);
        margin-top: 4rem;

        &:before {
            content: "";
            background-color: var(--color-primary);
            position: absolute;
            display: block;
            width: 100vw;
            height: 100%;
            left: 50%;
            right: 0;
            bottom: 0;
            top: 0;
            transform: translateX(-50%);
            z-index: -10;
        }

        img {
            grid-column: 1 / 1;
            max-width: 70%;
        }

        h2 {
            margin-top: 0;
            color: var(--color-white);
            grid-column: 1 / -1 ;
            margin-bottom: 3.25rem;
        }
    
        .technologie__container {
            grid-column: 2 / 2;
            align-items: center;
            position: relative;

            &:after {
                content: "";
                position: absolute;
                border: 1px solid var(--color-white);
                width: 15rem;
                top: 15px;
                transform: translate(-100%, 0);
            }

            .partial {
                position: relative;
                
                p {
                    padding-left: 4.25rem;
                }
                
                &:before {
                    content:attr(data-value);
                    border: 2px solid var(--color-brigt-green);
                    border-radius: 10rem;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    width: 3.375rem;
                    height: 3.375rem;
                    position: absolute;
                    top: -0.6875rem;
                }
            }
        }
    }

    .fade-in {
        opacity: 0;
        transition: opacity 300ms cubic-bezier(.1,.34,.87,.44);
    }

    /* Set to global for intersectionobserver */
    :global(.appear) {
        opacity: 1 !important;
    }

    .mb-80 {
        margin-bottom: 5rem;
    }

    .mt--4 {
        margin-top: -4rem;
    }

    .grid-wrapper {
        display: grid;
        grid-template-columns: 12.5rem 12.5rem 12.5rem;
        justify-content: center;
        grid-template-rows: 5rem min-content;
        column-gap: 9rem;
        row-gap: 3.75rem;
        margin-top: 3rem;
        margin-bottom: 3rem;

        img {
            max-width: 100%;
        }
    }

    .row--1 {
        grid-row: 1 / 1;    
    }

    .row--2 {
        grid-row: 2 / 2;    
    }

    .column--1 {
        grid-column: 1 / 1;
    }

    .column--2 {
        grid-column: 2 / 2;
    }
    .column--3 {
        grid-column: 3 / 3;
    }
  
    .bg-secondary {
        position: relative;
        background-color: var(--color-lighter-grey) !important;
        z-index: 100;
        padding-top: 5rem;
        padding-bottom: 4.625rem;

        &:before {
            content: "";
            background-color: var(--color-lighter-grey);
            position: absolute;
            display: block;
            width: 100vw;
            height: 100%;
            left: 50%;
            right: 0;
            bottom: 0;
            top: 0;
            transform: translateX(-50%);
            z-index: -10;
        }
    }

    @keyframes fadeIn {
        0% {
            opacity: 0;
        }
        100% {
            opacity: 1;
        }
    }

    @media (max-width: 992px) {            
        .bg-primary {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding-top: 2.75rem;
            padding-bottom: 2.75rem;

            .technologie__container {
                margin-bottom: 2rem;
                
                &:after {
                    content: none;
                }
            }

            img {
                margin-bottom: 3rem;
            }
        }


        .mt--4 {
            margin-top: 3rem;
        }

        .grid-wrapper {
            display: flex;
            flex-direction: column;
            row-gap: 1rem;
            
            img {
                width: 30% !important;
                display: flex;
                margin: 0 auto;
            }

            .w-mobile-50 {
                width: 50%;
            }
        }
    }
</style>

<svelte:head>
  <title>Mit der CoVerified-Technologie gegen Infodemie</title>
  <meta name="description" content="Unsere im Rahmen des #WirvsVirus Hackathon entwickelte
Tool-Chain bündelt sichere Informationen aus seriösen
Quellen und wirkt so Infodemie entgegen." />
</svelte:head>
<Container class="mt-5 pt-3 text-center">
    <h1>
        CoVerified macht Informationen aus sicheren Quellen zentral verfügbar
    </h1>
    <p>
        Das im Rahmen des #WirvsVirus Hackathon entwickelte CoVerified-Prinzip bündelt Informationen aus sicheren Quellen und macht sie über neue digitale Kanäle abrufbar.
    </p>
    <div class="bg-primary">
        <h2>
            Das CoVerified-Prinzip Schritt-für-Schritt erklärt:
        </h2>
        <img src="technologie_quellen.svg" alt="Quellen">
        <div class="technologie__container align-self-end">
            <div data-value="1" class="partial"><p><b>Seriöse Quellen auswählen</b></p></div>
            <p>
                Wir nutzen bestehende Infos aus RSS Feeds seriöser Quellen, die wir nach festgelegten transparenten Kriterien auswählen.
            </p>
        </div>
        <img src="technologie_themenauswahl.svg" alt="Themenauswahl">
        <div class="technologie__container align-self-end">
            <div data-value="2" class="partial"><p><b>Inhalt thematisch vertaggen</b></p></div>
            <p>
                Wir reichern die so gewonnen Daten und Inhalte mit weiteren Meta-Informationen an, ohne den eigentlichen Inhalt zu verändern. Ziel ist es, je nach Fokus und Bedarf relevanten Content nach Themen und Fragestellung automatisch zu selektieren.
            </p>
        </div>
        <img src="technologie_spracherkennung.svg" alt="Spracherkennung" class="fade-in">
        <div class="technologie__container fade-in align-self-end">
            <div data-value="3" class="partial"><p><b>Content-Sprache erkennen</b></p></div>
            <p>
                Natural Language Processing (NLP) ergänzt die Beiträge zusätzlich um die jeweilige Sprachinformation. Damit kann auch Mehrsprachigkeit und ein EU-weiter Einsatz gewährleistet werden.
            </p>
        </div>
        <img src="technologie_datenbank.svg" alt="Datenbank" class="fade-in">
        <div class="align-self-center">
            <div class="technologie__container fade-in mb-5">
                <div data-value="4" class="partial"><p><b>In Datenbank bündeln</b></p></div>
                <p>
                    Die gefilterten und aufbereiteten Daten fließen in eine Datenbank, werden dort über unsere API (Schnittstelle) gezielt abgefragt und situativ relevant in die verschiedenen Ausgabeformate ausgespielt.
                </p>
            </div>
            <div class="technologie__container fade-in">
                <div data-value="5" class="partial"><p><b>Ausgabe steuern</b></p></div>
                <p>
                    Über die Verwaltungsoberfläche können Einbinder Positionierung, Quellen und Themen individuell konfigurieren und eigene Fragestellungen, Informationen und News ergänzen. Damit können die Position auf der Webseite und die Inhalte des Widgets an den Kontext der Webseite angepasst und damit für die Endnutzer:innen besonders relevant angeboten werden.
                </p>
            </div>
        </div>
        <img src="technologie_wissenskanal.svg" alt="Wissenskanal" class="fade-in mt--4">
        <div class="technologie__container fade-in">
            <div data-value="6" class="partial"><p><b>Kommunikationskanal</b></p></div>
            <p>
                Abschließend wird der gewünschte Kommunikationskanal gewählt, über den die sicheren Informationen ausgespielt werden sollen, z.B. Web-Widget, Browser-Extension, eigene Webseite
            </p>
        </div>
    </div>    
    <div class="bg-secondary">
        <h2 class="mt-0">
            <span class="green--light-grey">Maßgeschneiderte Einbindung</span>
        </h2>
        <div class="grid-wrapper">
            <div class="grid-image row--1 column--1">
                <img src="icon_konfiguration_infoausgabe.svg" alt="Konfiguration der Info-Ausgabe" class="w-50">
            </div>
            <div class="grid-text column--1 row--2">
                Themen- und Quellen-Fokus der Informationen konfigurieren
            </div>
            <div class="grid-image column--2 row--1 mt-4 mt-md-0">
                <img src="icon_kuratieren_von_inhalten.svg" alt="Kuratieren von Inhalten" class="w-mobile-50">
            </div>
            <div class="grid-text column--2 row--2">
                Inhalte nach Fragestellungen kuratieren
            </div>
            <div class="grid-image column--3 row--1 mt-4 mt-md-0">
                <img src="icon_invididuelle_inhalte.svg" alt="Eigene Inhalte erstellen" class="w-50">
            </div>
            <div class="grid-text column--3 row--2">
                Visuelle Darstellung des Kanals individualisieren
            </div>
        </div>
        <Button href="/contact" label="Mehr Details? Kontaktieren Sie uns" style="btn-primary"></Button>
    </div>
    <h2>
        Eine besser informierte Gesellschaft ist Ihnen wichtig?
    </h2>
    <p>
        <span class="green">Dann unterstützen Sie unser Projekt</span> und werden Sie Teil der Wissens-Bewegung.
    </p>
    <div class="mb-120 mt-5">
        <Button style="btn-primary mb-5" label="Partner:in/Investor:in werden" href="/contact"></Button>
    </div>
</Container>
