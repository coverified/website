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

    .check-symbol {
        background: var(--color-primary);
        width: 3.125rem;
        height: auto;
        position: relative;

        &:before {
            content: "✓";
            position: absolute;
            font-size: 1.75rem;
            background: var(--color-primary);
            width: 2.8125rem;
            height: 2.8125rem;
            font-weight: 400;
            text-align: center;
            border-radius: 50%;
            left: 0;
            top: 7px;
            line-height: 1;
            padding-top: .5rem;
            color: var(--color-white);
        }
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
            
            + li {
                margin-top: 2.1875rem;
            }
        }
    }

    .widget-mockup {
        width: 30rem;
        max-width: 100%;
    }

    coverified-articles {
        --open-padding: 1rem;
    }

    .empfehlungs_text {
        font-size: .75rem;
        font-style: italic;
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

        .check-symbol {
            background: var(--color-primary);
            width: 3.125rem;
            height: auto;
            position: relative;
            margin: 0 auto;

            &:before {
                content: "✓";
                position: absolute;
                font-size: 1.75rem;
                background: var(--color-primary);
                width: 2.8125rem;
                height: 2.8125rem;
                font-weight: 400;
                text-align: center;
                border-radius: 50%;
                top: -57px;
                line-height: 1;
                padding-top: .5rem;
                color: var(--color-white);
                left: 50%;
            }
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
            .check-symbol {
                margin-top: 2rem;
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
            Mit einem Klick verifizierte <br />
            Informationen zu COVID-19.
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
            So binden Sie den Info-Button in Ihre Website ein.
        </h2>
        <p>
            Helfen Sie und versorgen Ihre Nutzer*innen mit verifizierten Informationen zur aktuellen Covid-19 Situation. Los geht's!
        </p>
    </Col>
    <Col sm="auto" lg="6">
        <img src="coverified-devices.png" alt="Coverified Devices Mockup">
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
        <p class="empfehlungs_text">
            Wir empfehlen Ihnen, bei Verwendung unseres Widgets einen entsprechenden Vermerk in Ihrer Datenschutzerklärung zu hinterlegen. Wir selbst erheben und verarbeiten keinerlei personenbezogene Daten, unser Serviceprovider allerdings Server-Logfiles der IP Adressen. Die Informationen in unserem Widget zeigen auf die Angebote Dritter, auf denen deren Datenschutzerklärungen greifen.
        </p>
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
    <Col sm="auto" lg="6" class="mb-5 text-center text-lg-left">
            <Row class="mb-5 flex-column flex-lg-row">
                <Col lg="2">
                    <div class="check-symbol"></div>
                </Col>
                <Col lg="6">
                <p>
                    Gemeinsam helfen! Sie tragen dazu bei, dass Menschen im Netz verlässliche Informationen erhalten.
                </p>
                </Col>
            </Row>
            <Row class="mt-5 mb-4 flex-column flex-lg-row">
                <Col lg="2">
                    <div class="check-symbol"></div>
                </Col>
                <Col lg="6">
                    <p>
                        Richtig informieren! Sie arbeiten proaktiv gegen die Verbreitung von Falschinformationen.
                    </p>
                </Col>
            </Row>
            <Row class="mt-5 flex-column flex-lg-row">
                <Col lg="2">
                    <div class="check-symbol"></div>
                </Col>
                <Col lg="6">
                    <p>
                        Einfach umzusetzen! Nur 1 Zeile JavaScript Code oder das fertige Wordpress Plugin in Ihre Homepage einfügen.
                    </p>
                </Col>
            </Row>
    </Col>
    <Col sm="auto" lg="6" class="text-center text-lg-left">
        <Row class="mb-5 flex-column flex-lg-row">
            <Col lg="2">
                <div class="check-symbol"></div>
            </Col>
            <Col lg="6" class="justify-content-center">
                <p >
                    Jetzt informieren! Sie halten die Besucher*innen Ihrer Homepage immer auf dem neuesten Stand zur Coronakrise.
                </p>
            </Col>
        </Row>
        <Row class="my-5 flex-column flex-lg-row">
            <Col lg="2">
                <div class="check-symbol"></div>
            </Col>
            <Col lg="6">
                <p>
                    Alle miteinbeziehen! Das Widget soll möglichst viele Menschen erreichen, daher ist es barrierefrei und Open Source programmiert.
                </p>
            </Col>
        </Row>
        <Row class="mt-5 flex-column flex-lg-row">
            <Col lg="2">
                <div class="check-symbol"></div>
            </Col>
            <Col lg="6">
                <p>
                    Jetzt handeln! Wir glauben, dass wir alle gemeinsam etwas tun können und der beste Zeitpunkt dafür jetzt ist.
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
            <img src="coverified-widget-mockup.png" class="widget-mockup" alt="CoVerified Widget Mockup">
        </Col>
        <Col sm="auto" lg="6">
            <ul class="list-style-dash">
                <li>
	                Der CoVerified-Button erscheint immer unten rechts auf Ihrer Website.
                </li>
                <li>
                    Mit einem Klick öffnet sich ein Fenster mit aktuellen Informationen zur Covid-19 Situation.
                </li>
                <li>
 	                An erster Stelle nennen wir die aktuellen Fallzahlen der John Hopkins University.
                </li>
                <li>
 	               Darunter folgen die neusten Infos, jeweils aus offiziellen und wissenschaftlich anerkannten Quellen.
                </li>
                <li>
 	                Die Vorschau der zugehörigen Artikel ist direkt auf die Informationsquelle verlinkt, damit Sie auch den ganzen Artikel durchlesen können.
                </li>
                <li>
                    Barrierefreiheit: Unser Informations-Tool (auf Deutsch Werkzeug) nimmt die voreingestellte Schriftgröße Ihres Browsers an, ist für Screenreading-Assistenten angepasst und wird zukünftig auch mehrsprachig zur Verfügung stehen.
                </li>
                <li>
 	                Unsere Datenbank besteht aus aktuellen Daten aus den RSS-Feeds offizieller Stellen. Diese Infos werden gebündelt und als News-Vorschau in unserem Widget dargestellt. Klicken Sie auf ein solches Vorschau-Feld, werden Sie direkt zur aktuellen Meldung auf die Seite der jeweiligen Quelle weitergeleitet.
                </li>
            </ul>
        </Col>
    </Row>
</div>
</Container>