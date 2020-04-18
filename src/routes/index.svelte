<script>
    import Button from '../components/Button.svelte';
    import Col from 'sveltestrap/src/Col.svelte';
    import Row from 'sveltestrap/src/Row.svelte';
    import Container from 'sveltestrap/src/Container.svelte';
</script>

<style type="text/scss">
    :root {
        overflow-x: hidden;
    }

    h1 {
        font-size: 2.25rem;
        font-weight: 700;
        color: var(--color-white);
        line-height: 48px;
        max-width: 645px;
    }

    h2 {
        font-size: 1.625rem;
        color: var(--color-anthracite);
        font-weight: 800;
        margin: 0 0 2.5rem 0;
    }

    .container {
        position: relative;
        height: auto;
        margin-bottom: 6.5em;


        &:before {
            content: "";
            position: absolute;
            background: var(--color-primary);
            display: block;
            width: 100vw;
            height: 100%;
            left: 50%;
            right: 0;
            bottom: 0;
            top: 0;
            transform: translateX(-50%);
        }

        > div:not(.info__box) {
            position: absolute;
            right: 0;
            bottom: 5rem;
            display: flex;
            align-items: center;
        }

        .coverified__informationgraphic {
            position: relative;
            width: 50%;
            padding-top: 2rem;
            padding-bottom: .5rem;
        }

        .wirvsvirus__logo {
            width: 26rem;
            height: auto;
            position: absolute;
            right: 0;
            top: 10%;
        }

        .info__box {
            right: 0;
            bottom: 0;
            transform: translateY(50%);
            background-color: var(--color-white);
            border: 2px solid var(--color-light-grey);
            box-shadow: 0 1px 6px -3px rgba(0, 0, 0, 0.11);
            display: block;
            position: absolute;
            border-radius: .33rem;
            padding: 1rem 1.75rem;
        }
    }

    .integration__buttons {
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    .logo {
        width: 3.125rem;
    }

    .background-primary {
        position: relative;
        padding-top: 7rem;
        padding-bottom: 7rem;
        margin-top: 6.25rem;
        margin-bottom: -7rem;
    
        &:before {
            content: "";
            position: absolute;
            background: var(--color-primary);
            display: block;
            width: 100vw;
            height: 100%;
            left: 50%;
            right: 0;
            bottom: 0;
            top: 0;
            transform: translateX(-50%);
        }

        
        h2 {
           color: var(--color-white);
        }

        li {
            color: var(--color-white);
        }
    }

    ul.list-style-dash {
        margin-top: 2.25rem;
        > li {
            list-style-position: inside;
            line-height: 34px;
            
            // &:before {
            //     content: '\2014';
            //     position: absolute;
            //     margin-left: -20px;
            // }
        }
    }

    .col-lg-2 {
        margin-bottom: 10rem;
    }

    coverified-articles {
        --open-padding: 1rem;
    }

    @media (max-width: 992px) {
        h1 {
            font-size: 2rem;
        }

        .container {
            display: flex;
            justify-content: center;
            margin-bottom: 8.5rem;

            > div:not(.info__box) {
                right: unset;
                bottom: 4.5rem;
            }

            > .info__box {
                right: unset;
            }

            .wirvsvirus__logo {
                left: 0;
                margin: 0 auto;
                top: 56%;
                width: 22rem;
            }

            .coverified__informationgraphic {
                width: 58%;
                padding-bottom: 18.5rem;
            }
        }
        .integration__buttons {
            flex-direction: column;
            justify-content: center;
            align-content: center;   
        }

        .logo {
            display: block;
            margin: 0 auto;
            margin-bottom: 2rem;
        }
    }

    @media (max-width: 768px) {
        h1 {
            font-size: 1.8rem;
        }
        .container {
            > div:not(.info__box) {
                bottom: 5rem;
            }

            .coverified__informationgraphic {
                width: 69%;
                padding-bottom: 21.5rem;
            }

            .wirvsvirus__logo {
                top: 48%;
            }
        }
    }


    @media (max-width: 576px) {
        h1 {
            font-size: 1.575rem;
            line-height: 33.6px;
        }

        .container {
            > div:not(.info__box) {
                bottom: 7rem;
                padding-left: .5rem;
                padding-right: .5rem;
            }

            > .info__box {
                right: 0;
            }

            .coverified__informationgraphic {
                width: 90%;
            }

            .wirvsvirus__logo {
                width: 16rem;
                top: 47%;
                right: 0;
                left: 0;
                margin: 0 auto;
            }
        }
    }
</style>

<svelte:head>
    <title>CoVerified</title>
    <meta name="description" content="CoVerified"/>
</svelte:head>

<h1 class="sr-only">CoVerified</h1>
<div class="container">
    <img class="coverified__informationgraphic" src="coverified-information-graphic.svg"
         alt="Coverified Information graphic">
    <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
    <div>
        <h1>
            Verifizierte Informationen zu <br />
            COVID-19 mit einen Klick verfügbar.
        </h1>
    </div>
    <div class="info__box">
        <coverified-cases></coverified-cases>
    </div>
</div>

<Container class="mt-5 pt-5">
<Row>
    <Col sm="auto" lg="6">
        <h2>
            Unseren Info-Button einfach auf Ihrer Website integrieren.
        </h2>
        <p>
            Auch Sie wollen Ihre Kundschaft und Nutzer*innen mit Verifizierten Informationen über die aktuelle Covid19 Situation versorgen?
        </p>
    </Col>
    <Col sm="auto" lg="6">
        <!-- TODO IMAGE -->
    </Col>
</Row>
<Row class="mt-5">
    <Col sm="auto" lg="6">
        <h2>
            So gehts! Einfach per JavaScript oder WordPress Plugin einbinden:
        </h2>
    </Col>
    <Col sm="auto" lg="12">
        <div class="my-5 integration__buttons">
            <Button href={'https://github.com/coverified/webcomponent#simple-integration'} label={'JavaScript'} target={'_blank'} rel={'noopener'}></Button>
            <Button href={'https://github.com/coverified/plugin-wordpress'} label={'WordPress-Plugin'} target={'_blank'} rel={'noopener'}></Button>
        </div>
    </Col>
</Row>
<Row class="mt-5">
    <Col sm="auto" lg="6">
        <h2>
            6 gute Gründe, warum Sie das kostenlose Widget nutzen sollten: 
        </h2>
    </Col>
</Row>
<Row class="mt-5 justify-content-center">
    <Col sm="auto" lg="6" class="mb-5">
            <Row class="mb-5">
                <Col lg="2" class="justify-content-center">
                    <img class="logo" src="favicon-32x32.png" alt="CoVerified Logo">
                </Col>
                <Col lg="6">
                <p>
                    Mithelfen! Wir wollen zur besseren Information der Bevölkerung beitragen.
                </p>
                </Col>
            </Row>
            <Row class="mt-5 mb-5">
                <Col lg="2">
                <img class="logo" src="favicon-32x32.png" alt="CoVerified Logo">
                </Col>
                <Col lg="6">
                <p>
                    Richtig informieren! Wir wollen proaktiv gegen die Verbreitung von Falschinformationen arbeiten.
                </p>
                </Col>
            </Row>
            <Row class="mt-5">
                <Col lg="2">
                <img class="logo" src="favicon-32x32.png" alt="CoVerified Logo">
                </Col>
                <Col lg="6">
                <p>
                    Seriös sein! Der Besucher Ihrer Website wird direkt informiert von verifizierten Quellen (siehe unten).
                </p>
                </Col>
            </Row>
    
    </Col>
    <Col sm="auto" lg="6">
        <Row class="mb-5">
            <Col lg="2">
                <img class="logo" src="favicon-32x32.png" alt="CoVerified Logo">
            </Col>
            <Col lg="6">
                <p>
                    Wir wollen zur besseren Information der Bevölkerung beitragen.
                </p>
            </Col>
        </Row>
        <Row class="mt-5 mb-5">
            <Col lg="2">
                <img class="logo" src="favicon-32x32.png" alt="CoVerified Logo">
            </Col>
            <Col lg="6">
                <p>
                    Wir wollen proaktiv gegen die Verbreitung von Falschinformationen arbeiten.
                </p>
            </Col>
        </Row>
        <Row class="mt-5">
            <Col lg="2">
                <img class="logo" src="favicon-32x32.png" alt="CoVerified Logo">
            </Col>
            <Col lg="6">
                <p>
                    Der Besucher Ihrer Website kann direkt informiert...
                </p>
            </Col>
        </Row>
    </Col>
</Row>
<div class="background-primary">
    <Row class="mt-5">
        <Col sm="auto" lg="6">
            <h2>
                So funktioniert der<br class="d-none d-lg-block"/> Informations-Button<br class="d-none d-lg-block"/>auf Ihrer Website:
            </h2>
            <!-- TODO IMAGE -->
        </Col>
        <Col sm="auto" lg="6">
            <ul class="list-style-dash">
                <li>
	                Unser CoVerified-Button erscheint immer unten rechts auf der Website und kann geöffnet werden.
                </li>
                <li>
                    Mit einem Tipp oder Klick öffnet sich ein Fenster mit aktuellen Informationen zur Covid19-Krise.
                </li>
                <li>
 	                An erster Stelle werden die aktuellen Fallzahlen der John Hopkins University gezeigt.
                </li>
                <li>
 	                Darunter folgen die brandneusten Infos auf, nur von staatlichen oder wissenschaftlich anerkannten Stellen.
                </li>
                <li>
 	                Die Vorschau der zugehörigen Artikel ist direkt auf die Quelle der Information verlinkt, damit Sie sich in Ruhe den ganzen Artikel durchlesen können.
                </li>
                <li>
 	                Barrierefreiheit: Unser Informations-Tool (auf Deutsch Werkzeug) nimmt die voreingestellte Schriftgröße des Browsers an, ist für Screenreading-Assistenten angepasst und soll auf lange Sicht auch mehrsprachig Informationen zur Verfügung stellen.
                </li>
                <li>
 	                Unsere Datenbank wird gefüttert mit allen aktuellen Daten aus den RSS-Feeds offizieller Stellen. Diese Informationen werden gebündelt und als News-Vorschau in unserem Widget dargestellt. Klickt oder tippt der Nutzer auf ein solches Vorschau-Feld, wird er direkt zur aktuellen Meldung auf die Seite der jeweiligen Quelle weitergeleitet.
                </li>
            </ul>
        </Col>
    </Row>
</div>
</Container>