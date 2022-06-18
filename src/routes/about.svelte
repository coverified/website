<script>
    import Button from '../components/Button.svelte';
    import Col from 'sveltestrap/src/Col.svelte';
    import Row from 'sveltestrap/src/Row.svelte';
    import Container from 'sveltestrap/src/Container.svelte';
</script>

<svelte:head>
    <title>Das CoVerified-Team aus dem #WirvsVirus Hackathon</title>
    <meta
        name="description"
        content="Digitale Lösungen für die Zivilgesellschaft – Als eines der
geförderten Projekte aus dem #WirvsVirus Hackathon
entwickeln wir Open Social Innovation."
    />
</svelte:head>
<Container class="mt-0 mt-md-5  pt-3 text-center">
    <h1>
        #WirvsVirus<br />
        Wir sind CoVerified
    </h1>
    <p>
        Ein Wochenende im März war die Geburtsstunde von CoVerified: 3 Entwickler aus Bayern stürzten sich mit knapp
        30.000 anderen in den #WirvsVirus Hackathon. Im Kopf die Idee, aktiv gegen Desinformation und die Spaltung der
        Gesellschaft vorgehen. Das Wochenende endete nicht nur mit neuen Team-Membern und einem funktionsfähigen
        Prototypen, sondern mit dem unglaublichen Gefühl, Teil einer besonderen Community zu sein und als
        Zivilgesellschaft an Lösungen aktiv mitwirken zu können.
    </p>
    <div class="bg-primary text-white mt-5">
        <p class="zitat">
            „Nach unserer Überzeugung gibt es kein größeres und wirksameres Mittel zu wechselseitiger Bildung als das
            Zusammenarbeiten.“
        </p>
        <p>Johann Wolfgang von Goethe</p>
    </div>
    <h2 class="mt-5">
        <span class="green">Unsere Mission</span>
    </h2>
    <p>
        CoVerified denkt Kommunikation im öffentlichen Sektor neu und entwickelt zukunftsorientierte, digitale Lösungen
        für Staat, Verwaltung und Institutionen.
    </p>
    <Row class="text-left mt-5">
        <Col sm="auto" lg="4">
            <p class="text-primary">#Demokratie</p>
            <p>
                Wir glauben, dass eine gut informierte Bevölkerung der Schlüssel zu einer funktionierenden Gesellschaft
                ist und Bildung das Vertrauen in staatliche Entscheidungen fördert. Gesichertes Wissen leicht zugänglich
                machen und in der Breite der Bevölkerung für Faktensicherheit sorgen, ist das Ziel von Coverified. Denn
                Wissen fördern und Demokratie stärken sind wichtiger denn je.
            </p>
        </Col>
        <Col sm="auto" lg="4" class="mt-3 mt-md-0">
            <p class="text-primary">#OpenSocialInnovation</p>
            <p>
                Mit der Idee im Kopf und Leidenschaft im Herzen sind wir in den Hackathon #WirvsVirus 2020 gestartet.
                Seite an Seite mit knapp 150 Projekten haben wir Lösungen für die Probleme im Zuge der COVID-19-Pandemie
                entwickelt. Wir sind überzeugt, dass Open Social Innovation dem großen Innovationspotential der
                Zivilgesellschaft die Tür öffnet und gelebte Partizipation wunderbare Lösungen für viele
                gesellschaftliche Herausforderungen bereithält.
            </p>
        </Col>
        <Col sm="auto" lg="4" class="mt-3 mt-md-0">
            <p class="text-primary">#GovTech</p>
            <p>
                Als GovTech-Startup arbeiten wir bei CoVerified daran, die Digitalisierung mit innovativen
                Kommunikationslösungen mitzugestalten und neue Informationsstandards zu setzen. Wir sehen uns als
                Innovationspartnerin, die intelligente Softwareprodukte für den öffentlichen Sektor von morgen liefert
                und die notwendigen digitalen Tranformationsprozesse in der Verwaltung mit neuen Technologien begleitet.
            </p>
        </Col>
    </Row>
    <h2>
        <span class="green">#digitalpioneers</span>
    </h2>
    <p>
        Das ist das interdisziplinäre Team, das mit Herzblut hinter CoVerified steht. 8 Expert:innen, die sich remote
        gefunden haben, um gemeinsam etwas zu bewirken und Open Social Innovation von der Idee bis zur Umsetzung zu
        gestalten.
    </p>
    <div class="digitalpioneers">
        <div class="overlay__container">
            <img loading="lazy" src="alessa_fetzer.jpg" alt="Alessa Fetzer" width="625" height="625" />
            <div class="overlay__container-popup">
                <p class="overlay__container-popup--name">
                    Alessa Fetzer<br />
                    <span class="overlay__container-popup--title">Projektmanagerin</span>
                </p>
                <div class="overlay__container-popup--links">
                    <a href="https://www.xing.com/profile/Alessa_Fetzer/" target="_blank" title="Xing" rel="noopener">
                        <img src="xing.svg" alt="Xing Logo" loading="lazy" width="35" height="39" />
                    </a>
                    <a href="https://www.linkedin.com/in/alessafetzer/" target="_blank" title="linkedIn" rel="noopener">
                        <img src="linkedin.svg" alt="linkedIn Logo" loading="lazy" width="35" height="39" />
                    </a>
                </div>
            </div>
        </div>
        <div class="overlay__container">
            <img loading="lazy" src="christina_vollnhals.jpg" alt="Christina Vollnhals" width="625" height="625" />
            <div class="overlay__container-popup">
                <p class="overlay__container-popup--name">
                    Christina Vollnhals<br />
                    <span class="overlay__container-popup--title">UX-Designerin</span>
                </p>
                <div class="overlay__container-popup--links">
                    <a
                        href="https://www.xing.com/profile/Christina_Vollnhals/"
                        target="_blank"
                        title="Xing"
                        rel="noopener"
                    >
                        <img src="xing.svg" alt="Xing Logo" loading="lazy" width="35" height="39" />
                    </a>
                    <a
                        href="https://www.linkedin.com/in/christina-vollnhals-21b96513b/"
                        target="_blank"
                        title="linkedIn"
                        rel="noopener"
                    >
                        <img src="linkedin.svg" alt="linkedIn Logo" loading="lazy" width="35" height="39" />
                    </a>
                </div>
            </div>
        </div>
        <div class="overlay__container">
            <img
                loading="lazy"
                src="florian_schlittenbauer.jpg"
                alt="Florian Schlittenbauer"
                width="625"
                height="625"
            />
            <div class="overlay__container-popup">
                <p class="overlay__container-popup--name">
                    Florian Schlittenbauer<br />
                    <span class="overlay__container-popup--title">Webentwickler</span>
                </p>
                <div class="overlay__container-popup--links">
                    <a
                        href="https://www.xing.com/profile/Florian_Schlittenbauer/cv"
                        target="_blank"
                        title="Xing"
                        rel="noopener"
                    >
                        <img src="xing.svg" alt="Xing Logo" loading="lazy" width="35" height="39" />
                    </a>
                    <a href="https://www.linkedin.com/in/schliflo/" target="_blank" title="linkedIn" rel="noopener">
                        <img src="linkedin.svg" alt="linkedIn Logo" loading="lazy" width="35" height="39" />
                    </a>
                </div>
            </div>
        </div>
        <div class="overlay__container">
            <img loading="lazy" src="johannes_hiry.jpg" alt="Johannes Hiry" width="625" height="625" />
            <div class="overlay__container-popup">
                <p class="overlay__container-popup--name">
                    Johannes Hiry<br />
                    <span class="overlay__container-popup--title">Gesellschafter</span>
                </p>
                <div class="overlay__container-popup--links">
                    <a href="https://www.xing.com/profile/Johannes_Hiry/cv" target="_blank" title="Xing" rel="noopener">
                        <img src="xing.svg" alt="Xing Logo" loading="lazy" width="35" height="39" />
                    </a>
                    <a
                        href="https://www.linkedin.com/in/johannes-hiry/"
                        target="_blank"
                        title="linkedIn"
                        rel="noopener"
                    >
                        <img src="linkedin.svg" alt="linkedIn Logo" loading="lazy" width="35" height="39" />
                    </a>
                </div>
            </div>
        </div>
        <div class="overlay__container">
            <img loading="lazy" src="julia_diehl.jpg" alt="Julia Diehl" width="625" height="625" />
            <div class="overlay__container-popup">
                <p class="overlay__container-popup--name">
                    Julia Diehl<br />
                    <span class="overlay__container-popup--title">UX-Designerin / Marketing & Kommunikation</span>
                </p>
                <div class="overlay__container-popup--links">
                    <a
                        href="https://www.linkedin.com/in/julia-diehl-ux-co/"
                        target="_blank"
                        title="linkedIn"
                        rel="noopener"
                    >
                        <img src="linkedin.svg" alt="linkedIn Logo" loading="lazy" width="35" height="39" />
                    </a>
                </div>
            </div>
        </div>
        <div class="overlay__container">
            <img loading="lazy" src="steven_killian.jpg" alt="Steven Killian" width="625" height="625" />
            <div class="overlay__container-popup">
                <p class="overlay__container-popup--name">
                    Steven Killian<br />
                    <span class="overlay__container-popup--title">Webentwickler</span>
                </p>
                <div class="overlay__container-popup--links">
                    <a
                        href="https://www.linkedin.com/in/steven-killian-224b65199/"
                        target="_blank"
                        title="linkedIn"
                        rel="noopener"
                    >
                        <img src="linkedin.svg" alt="linkedIn Logo" loading="lazy" width="35" height="39" />
                    </a>
                </div>
            </div>
        </div>
        <div class="overlay__container">
            <img loading="lazy" src="paula_weise.jpg" alt="Paula Weise" width="625" height="625" />
            <div class="overlay__container-popup">
                <p class="overlay__container-popup--name">
                    Paula Weise<br />
                    <span class="overlay__container-popup--title">Designerin</span>
                </p>
                <div class="overlay__container-popup--links">
                    <a href="https://www.xing.com/profile/Paula_Weise4/cv" target="_blank" title="Xing" rel="noopener">
                        <img src="xing.svg" alt="Xing Logo" loading="lazy" width="35" height="39" />
                    </a>
                    <a
                        href="https://www.linkedin.com/in/paula-weise-b979091a2/"
                        target="_blank"
                        title="linkedIn"
                        rel="noopener"
                    >
                        <img src="linkedin.svg" alt="linkedIn Logo" loading="lazy" width="35" height="39" />
                    </a>
                </div>
            </div>
        </div>
    </div>
    <div class="bg-secondary">
        <h2 class="mt-0">
            <span class="green--light-grey">Unser Leistungsprofil</span>
        </h2>
        <p>Wir begleiten Kommunikationsprojekte von der Idee bis zur Umsetzung</p>
        <Row class="text-left my-5">
            <Col sm="auto" lg="3">
                <p class="text-primary">Software-Entwicklung</p>
                <p>Von Strategie und Konzeption über Design und Programmierung bis zur Implementierung.</p>
            </Col>
            <Col sm="auto" lg="3">
                <p class="text-primary">Projektmanagement</p>
                <p>Beratung, Projektleitung und Abstimmung mit allen Beteiligten</p>
            </Col>
            <Col sm="auto" lg="3">
                <p class="text-primary">Marketing & Kommunikation</p>
                <p>Planung, Gestaltung und Umsetzung von Kommunikations-Maßnahmen z.B. Kampagne</p>
            </Col>
            <Col sm="auto" lg="3">
                <p class="text-primary">Service & Maintainance</p>
                <p>Betreuung von Einbindung und Betrieb der Kommunikationslösungen Trainings für Anwender:innen</p>
            </Col>
        </Row>
        <Button label="Jetzt Kontakt aufnehmen&nbsp;&#8594;" href="/contact" style="btn-primary" />
    </div>
    <div class="bg-primary bg-primary--twitter text-center">
        <img loading="lazy" src="twitter.svg" alt="twitter logo" width="61" height="51" class="twitter-logo" />
        <h3 class="text-white h1">Werde Teil unserer Mission und folge uns auf Twitter</h3>
        <Button
            style="btn-secondary"
            href="https://twitter.com/CoVeri_fied"
            target="_blank"
            rel="noopener"
            label="CoVerified auf Twitter folgen"
        />
    </div>
</Container>

<style type="text/scss">
    .bg-primary {
        position: relative;
        background-color: var(--color-primary) !important;
        z-index: 100;
        padding-top: 5rem;
        padding-bottom: 5rem;
        text-align: left;

        &:before {
            content: '';
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

        &--twitter {
            padding-top: 5.4375rem;
        }

        .twitter-logo {
            width: 5%;
            margin: 0 auto;
            padding-bottom: 0.5rem;
        }
    }

    .bg-secondary {
        position: relative;
        background-color: var(--color-lighter-grey) !important;
        z-index: 100;
        margin-top: 7.75rem;
        padding-top: 5rem;
        padding-bottom: 4.625rem;

        &:before {
            content: '';
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

    .zitat {
        font-size: 3rem;
        line-height: 1.25;
    }

    .digitalpioneers {
        display: grid;
        grid-template-columns: repeat(auto-fit, 16rem);
        justify-content: center;
        grid-template-rows: 1fr;
        grid-gap: 1.5rem;
        z-index: 1;

        .overlay__container {
            position: relative;

            &:hover .overlay__container-popup {
                opacity: 0.8;
            }

            &-popup {
                position: absolute;
                top: 0;
                bottom: 0;
                left: 0;
                right: 0;
                opacity: 0;
                transition: 0.25s ease-in;
                background-color: var(--color-primary);
                width: 100%;
                height: auto;
                border-radius: 10rem;
                color: var(--color-white);

                &--name {
                    font-weight: 500;
                    position: absolute;
                    top: 3.1875rem;
                    left: 0;
                    right: 0;
                }

                &--title {
                    font-weight: 300;
                    font-size: 1.15rem;
                }

                &--links {
                    display: flex;
                    justify-content: center;
                    position: absolute;
                    bottom: 3.1875rem;
                    left: 0;
                    right: 0;

                    a {
                        img {
                            width: 60%;
                        }
                    }
                }
            }

            img {
                display: block;
                width: 100%;
                height: auto;
                z-index: -10;
            }
        }
    }

    @media (min-width: 770px) {
    }

    @media (min-width: 1200px) {
    }

    @media (max-width: 992px) {
        .zitat {
            font-size: 2.25rem;
        }

        .digitalpioneers {
            grid-template-columns: repeat(auto-fit, 12rem);

            .overlay__container {
                &-popup {
                    opacity: 0.7;

                    &--name {
                        font-size: 1.15rem;
                        top: 2.75rem;
                        line-height: 1.5;
                    }

                    &--title {
                        font-size: 1rem;
                    }

                    &--links {
                        bottom: 1rem;
                    }
                }
            }
        }

        .bg-secondary {
            margin-top: 1.75rem;
        }

        .bg-primary {
            .twitter-logo {
                width: 15%;
            }
        }
    }

    @media (max-width: 768px) {
        .digitalpioneers {
            grid-template-columns: repeat(auto-fit, 14rem);
        }
    }

    @media (max-width: 524px) {
        .digitalpioneers {
            grid-template-columns: repeat(auto-fit, 10rem);
            justify-content: center;
        }
    }
</style>
