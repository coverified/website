<script>
    import Button from '../components/Button.svelte';
    import Container from 'sveltestrap/src/Container.svelte';
</script>

<style type="text/scss">
    .mt-72 {
        margin-top: 4.5rem;
    }

    .bg-primary {
        position: relative;        
        background-color: var(--color-primary) !important;
        z-index: 100;
        padding-top: 5rem;
        padding-bottom: 5rem;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 20rem 25rem 25rem;        
        column-gap: 6.25rem;

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

        &:after {
            content: "";
            position: absolute;
            left: 0;
            right: auto;
            width: 0;
            height: 0;
            border-style: solid;
            bottom: 0;
            border-width: 3rem 3rem 0 3rem;
            border-color: var(--color-primary) transparent transparent transparent;
            left: 50%;
            transform: translate(-50%, 100%);
        }

        .logo-wika {
            width: 25%;
        }
    }

    .column--1-3 {
        grid-column: 1 / -1;
    }

    .row--2-3 {
        grid-row : 2 / -1;
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

    .row--1 {
        grid-row: 1 / 1;
    }

    .row--2 {
        grid-row: 2 / 2;
    }

    .row--3 {
        grid-row: 3 / 3;
    }

    .animation {
        width: 27rem;
        height: auto;
        display: block;
    }

    .grid-wrapper {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr min-content;
        grid-gap: 2rem;
    }

    .grid-image {
        grid-row: 1 / 1;    
        width: 60%;
        margin: 0 auto;
    }
    
    .grid-text {
        grid-row: 2 / 2;
    }

    .digitalpioneers {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(6.25rem, 1fr));
        grid-template-rows: 1fr;
        grid-gap: 1rem;
        margin-bottom: 3rem;
    }
    
    @media (max-width: 992px) {    
        h1 {
            font-size: 2rem;
        }

        .grid-wrapper {
            display: flex;
            flex-direction: column;
        }

        .animation {
            width: 100%;
            height: auto;
        }

        .bg-primary {
            display: flex;
            flex-direction: column;
            padding-top: 3.5rem;
            padding-bottom: 3.5rem;

            .image {
                width: 30% !important;

                &--50 {
                    width: 50%;
                }
            }

            .logo-wika {
                width: 50%;
            }
        }
    }

    @media (max-width: 768px) {

    }

    @media (max-width: 576px) {
        h1,
        .h1 {
            font-size: 2rem;
        }        
    }

    @media (min-width: 1600px) {
        .coverified-video {
            width: auto !important;
            max-width: 100%;
            display: flex;
            margin: 0 auto;
        }
    }
</style>

<svelte:head>
    <title>Mit CoVerified Digitalisierung gestalten| Wir denken digitale Kommunikation neu</title>
    <meta name="description" content="Unsere Software-Produkte gestalten Digitalisierung und
schaffen einen neuen Informationsstandard zur einfachen
Information der breiten Bevölkerung."/>
</svelte:head>
<Container class="mt-5 pt-3 text-center">
    <h1 class="h1 mt-0">
        Mit CoVerified Digitalisierung gestalten<br />
        &ndash; Wir denken digitale Kommunikation neu &ndash;
    </h1>
    <p>
        Unsere Software-Produkte gestalten Digitalisierung und schaffen einen neuen Informationsstandard zur einfachen Information der breiten Bevölkerung. Denn eine gut informierte Gesellschaft ist die Basis einer starken Demokratie.
    </p>
</Container>
<video class="w-100 h-auto mt-5 mb-3 coverified-video" src="coverified-video.mp4" preload=”none” muted autoplay></video>        
<Container class="pt-3 text-center">
    <h2 class="mt-5">
        Mehr Wissen <span class="green">für alle</span>.        
    </h2>
    <p>
        Wir gestalten digitale Produkte, die sichere Informationen bündeln und einfach zugänglich machen.
    </p>
    <div class="grid-wrapper mt-5">
        <img loading="lazy" src="diesituation.png" alt="Die Situation" width="254" height="307" class="grid-image w-50">
        <div class="grid-text">
            <p>
                <b>Die Situation:</b><br />
                Verlässliche Informationen sind im Netz verstreut und mühsam zu finden
            </p>
        </div>    
        <img class="grid-image" loading="lazy" src="unsereloesung.png" alt="Unsere Lösung" width="316" height="307">
        <div class="grid-text">
            <p>
                <b>Unsere Lösung:</b><br />
                Wir bündeln das Wissen aus sicheren Quellen und stellen es über neue digitale Kanäle zur Verfügung
            </p>
        </div>
        <img class="grid-image" loading="lazy" src="unserevision.png" alt="Unsere Vision" width="297" height="307">
        <div class="grid-text">
            <p>
                <b>Unsere Vision:</b><br /> 
                eine informierte, faktensichere, Öffentlichkeit mit mehr Verständnis, Weitsicht und Toleranz
            </p>
        </div>    
    </div>
    <div class=" bg-primary text-white mt-72">
        <div class="column--1-3 row--1">
            <h2 class="text-white mt-0">
                Die CoVerified Lösung für mehr Wissen im Netz:
            </h2>
            <img class="logo-wika mb-4 mx-auto" loading="lazy" src="logo-wika.svg" alt="Wika Logo" width="284" height="112">
            <p class="mb-5 mb-md-0 font-weight-300">
                Corona, Klimaschutz, Zuwanderung, Pflege, Digitalisierung... diese und viele weitere Themen bewegen ganz Deutschland. Aber wo kann man verlässliche Informationen dazu finden? Unser Web-Widget Wika bündelt unverfälschte Meldungen aus erster Hand und macht sie bequem und ansprechend webweit verfügbar.    
            </p>
        </div>
        <div class="row--2 column--1 order-1 order-lg-1 d-flex justify-content-center flex-column align-items-center">
            <img loading="lazy" src="icon_story.png" alt="Story Elemente" width="109" height="146" class="w-50 image mb-4">
            <p>
                Bequemer Einstieg über Stories zu aktuell relevanten Informationen
            </p>
        </div>        
        <div class="row--3 column--1 order-1 order-lg-1 d-flex justify-content-center flex-column align-items-center mt-5 mb-lg-0">
            <img loading="lazy" src="icon_themenauswahl.png" alt="Themenauswahl" width="302" height="105" class="mb-4 image--50">
            <p>
                Gezieltes Informieren über Auswahl von Themen
            </p>
        </div>
        <div class="column--2 row--2-3 order-3 order-lg-2">
            <video class="animation mx-auto my-5" src="widgetanimation.mov" preload=”none” controls></video>        
        </div>
        <div class="row--2 column--3 order-2 order-lg-3 d-flex justify-content-center flex-column align-items-center my-5 my-lg-0">
            <img class="mb-4 image w-75" loading="lazy" src="icon_kuratieren.svg" alt="Kuratierte Inhalte" width="151" height="96">
            <p>
                Kuratierte Inhalte zu nutzer*innen-zentrierten Fragestellungen
            </p>
        </div>
        <div class="row--3 column--3 order-2 order-lg-3 d-flex justify-content-center flex-column align-items-center">
            <img class="w-50 image mb-4" loading="lazy" src="icon_trends.svg" alt="Automatische Relevanzsortierung" width="120" height="80">
            <p>
                Automatische Relevanz-Sortierung nach Themen-Trends im Netz
            </p>
        </div>
    </div>
    <h2>
        Wika <span class="green">bringt Wissen zu den Menschen</span> - ohne zusätzlichen Aufwand
    </h2>
    <div class="grid-wrapper mb-5">
        <img loading="lazy" class="grid-image w-50" src="rss-feed.png" alt="Die Situation" width="137" height="170">
        <div class="grid-text">
            <p>
                Wir nutzen bestehende RSS Feeds – somit entsteht <b>kein zusätzlicher redaktioneller Aufwand</b>
            </p>        
        </div>        
        <img loading="lazy" src="webeinbindung.png" alt="Unsere Lösung" width="265" height="182" class="grid-image my-auto">
        <div class="grid-text">
            <p>
                Unser Widget ist webweit einbindbar – Informationen bekommen damit eine <b>enorme Reichweite</b>
            </p>
        </div>
        <img loading="lazy" src="nutzerinzentriert.png" alt="Unsere Vision" width="200" height="210" class="grid-image">
        <div class="grid-text">
            <p>
                Unsere Lösung ist <b>nutzer:innen-zentriert</b> entwickelt – somit erreichen wir eine <b>höhere Akzeptanz</b>
            </p>
        </div>
    </div>
    <Button style="btn-primary" label="Zur Funktionsweise&nbsp;&#8594;" href="/technologie"></Button>
    <h2>
        <span class="green">#digitalpioneers</span>        
    </h2>
    <p class="mb-5">Hinter CoVerified stehen 9 Expert:innen mit Leidenschaft für Digitalisierung und Open Social Innovation.</p>
    <div class="digitalpioneers">
        <img loading="lazy" src="alessa_fetzer.jpg" alt="Alessa Fetzer" width="625" height="625">
        <img loading="lazy" src="christina_vollnhals.jpg" alt="Christina Vollnhals" width="625" height="625">
        <img loading="lazy" src="florian_schlittenbauer.jpg" alt="Florian Schlittenbauer" width="625" height="625">
        <img loading="lazy" src="johannes_hiry.jpg" alt="Johannes Hiry" width="625" height="625">
        <img loading="lazy" src="julia_diehl.jpg" alt="Julia Diehl" width="625" height="625">
        <img loading="lazy" src="paula_weise.jpg" alt="Paula Weise" width="625" height="625">
        <img loading="lazy" src="steven_killian.jpg" alt="Steven Killian" width="625" height="625">
        <img loading="lazy" src="carmen_bernhardt.jpg" alt="Carmen Bernhardt" width="625" height="625">
        <img loading="lazy" src="baerbel.jpg" alt="Bärbel" width="625" height="625">
    </div>
    <Button style="btn-primary" label="CoVerified kennenlernen&nbsp;&#8594;" href="/about"></Button>
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