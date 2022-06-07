<script>
    import Button from '../components/Button.svelte';
    import Container from 'sveltestrap/src/Container.svelte';
</script>

<svelte:head>
    <title>Mit CoVerified Digitalisierung gestalten| Wir denken digitale Kommunikation neu</title>
    <meta
        name="description"
        content="Unsere Software-Produkte gestalten Digitalisierung und
schaffen mehr Wert."
    />
</svelte:head>
<Container class="mt-0 mt-md-5  pt-3 text-center">
    <h1 class="h1 mt-0">Mehr digitale Power für alle.</h1>
    <p>
        Mit den besten Werkzeugen der Digitalisierung entwickeln wir gemeimsam innovative Software-Lösungen.
Für effizientere Prozesse, besser informierte Menschen und eine starke Gesellschaft.
Los geht’s!
    </p>
</Container>
<video
    class="w-100 h-auto mt-5 mb-3 coverified-video"
    src="coverified-video.mp4"
    preload="”none”"
    muted
    autoplay
    playsinline
/>
<Container class="pt-3 text-center">
    <h2 class="mt-5">
        Lasst uns die Welt <span class="green">besser besser</span> machen!
    </h2>
    <p>
        Effizienter arbeiten, schneller finden, besser verstehen – wir machen das Leben leichter für alle,
        die in und mit Regierungen, Verwaltungen, Institutionen und Unternehmen arbeiten und kommunizieren. Damit MEHR WERT entsteht.
    </p>
    <div class="grid-wrapper mt-5">
        <img
            loading="lazy"
            src="situation.png"
            alt="Die Situation"
            width="316"
            height="307"
            class="grid-image w-50"
        />
        <div class="grid-text">
            <p>
                <b>Die Situation</b><br />
                Informationen sind oft verstreut, kompliziert und unübersichtlich. Prozesse veraltet und ineffizient.
                Das digitale Potenzial bleibt ungenutzt. Das erschwert die Kommunikation mit Bürger:innen und Mitarbeitenden,
                raubt Zeit und bremst Innovationskraft. Frustrierend für alle!
            </p>
        </div>
        <img class="grid-image" loading="lazy" src="loesung.png" alt="Unsere Lösung" width="316" height="307" />
        <div class="grid-text">
            <p>
                <b>Die Lösungen</b><br />
                Wir gehen zusammen auf die Reise. Ob experimenteller Prototyp, inspirierendes Pilot-Projekt oder umfassender System-Change –
                wir analysieren gemeinsam den genauen Bedarf und kreieren iterativ und agil zusammen die passende innovative Digital-Lösung.
                Und das ist manchmal etwas ganz anderes, als am Anfang gedacht.
            </p>
        </div>
        <img class="grid-image" loading="lazy" src="vision.png" alt="Unsere Vision" width="297" height="307" />
        <div class="grid-text">
            <p>
                <b>Unsere Vision</b><br />
                Neue digitale Kanäle und Formate. Userzentrierte Inhalte und effizientere Prozesse.
                Agile, wertschätzende Zusammenarbeit. Und mit unseren Kompetenzen die Digitalisierung so zu gestalten,
                dass sie uns allen als Treiber positiver Veränderung für Gesellschaft und Wirtschaft dient.
            </p>
        </div>
    </div>
      <div class=" bg-primary text-white">
        <div class="column--1-2 row--1">
            <h2 class="text-white mt-0">Aktuelles bei CoVerified</h2>
            <p class="mb-5 mb-md-0 font-weight-300">
                Im Auftrag der Energiewende! CoVerified entwickelt die Kommunikationskampagne “DA/RE – da steckt mehr dahinter”
                für TransnetBW und macht damit "Redispatch" für alle erlebbar.
            </p>
        </div>
        <div class="row--2 column--1 d-flex justify-content-center flex-column align-items-center">
            <img loading="lazy" src="coverified-pilotprojekt.jpg" alt="Pilotprojekt" class="w-100">
        </div>
        <div
            class="row--2 column--2 order-2 order-lg-3 d-flex justify-content-center flex-column align-items-center my-5 my-lg-0"
        >
            <p>
                Komplexe Themen einfach erklärt mit interaktiver Webseite, griffigen Anzeigenmotiven und sogar einem eigenen Game.
                Unter dem Motto "#DAREKannDas Kannst du das auch?" können User versuchen, einen fiktiven Leitungs-Engpass zu regeln
                und dabei mehr über Stromnetzsicherheit, Redispatch (Stromausgleich) und die Unterstützung von DA/RE lernen.
            </p>
            <Button style="btn-secondary mt-5" label="Zur DA/RE Kampagnenseite &#8594;" href="https://www.dare-plattform.de/erleben" target="_blank" rel="noopener" />
        </div>
    </div>
    <div class="social__impact">
        <h2>
            <span class="green--light-grey">Social Impact</span> durch digitale Innovationen
        </h2>
        <p>
            Bei uns trifft anspruchsvolle Technologie auf ausgeklügelte User-Experience, kreatives Design und jede Menge Leidenschaft für Open Social Innovation.
            Wir lieben es, wenn wir mit #DigitalThinking und unserem #FullStackService #GoodTech entwickeln.
            Und wenn wir dann noch als #DigitalisierungsVorreiter:innen echten #Mehrwert erzeugen, jubelt unser #Tech4Good Herz.
        </p>
        <div>
            <figure class="grid-image">
                <img loading="lazy" src="coverified-technologie.svg" alt="WeMakeItWork" width="120" height="120" />
                <figcaption>#WeMakeItWork</figcaption>
            </figure>
        </div>
        <div>
            <figure class="grid-image">
                <img loading="lazy" src="digitalthinking.svg" alt="DigitalThinking" width="120" height="120" />
                <figcaption>#DigitalThinking</figcaption>
            </figure>
        </div>
    </div>
</Container>
<Container class="pt-3 text-center">
    <h2 class="mt-5">
        Let's <span class="green">co-create</span> !
    </h2>
    <p>
        Wir greifen das Abstrakte, formulieren eine Herausforderung und kümmern uns dann gemeinsam um die Lösung.
        Wir beflügeln da, wo Sie uns brauchen. Punktuell oder rundherum.
    </p>
      <div class="termin__box">
        <h2>Digitalisierungsbedarf? Los geht's!</h2>
        <p>
            Ineffiziente Arbeitsprozesse? Mühsame Kommunikation? Stundenlange Recherche?
            Gern schauen wir uns den konkreten Bedarf an. Dafür gibt’s unser kostenfreies Beratungsgespräch.
        </p>
        <Button
            style="btn-secondary mt-5"
            label="Termin vereinbaren"
            href="mailto:info@coverified.info?subject=Interesse%20an%20zusammenarbeit"
        />
    </div>
    <h2>
        Darum <span class="green">CoVerified</span>
    </h2>
    <div class="grid">
        <figure class="grid-image">
            <img loading="lazy" src="opensource.png" alt="OpenSocialInnovation" width="120" height="120" />
            <figcaption>#OpenSocialInnovation</figcaption>
        </figure>
        <div class="grid-content">
            <p>
                <b>Public money, public code!</b><br />
                Wir entwickeln Software-Lösungen für die Gesellschaft und sind überzeugt, dass Zusammenarbeit Innovationen
                fördert und die Qualität steigert.
            </p>
        </div>
        <figure class="grid-image">
            <img loading="lazy" src="dsvgo.png" alt="CyberSicher" width="120" height="120" />
            <figcaption>#CyberSicher</figcaption>
        </figure>
        <div class="grid-content">
            <p>
                <b>DSGVO- konform</b><br />
                Datensicherheit hat bei uns Vorrang: Wir verzichten auf alles, was möglich ist, verarbeiten notwendige Daten
                von Nutzenden DSVGO-konform und hosten unsere Services in Deutschland.
            </p>
        </div>
        <figure class="grid-image">
            <img loading="lazy" src="ki.png" alt="TrustInTech" width="120" height="120" />
            <figcaption>#TrustInTech</figcaption>
        </figure>
        <div class="grid-content">
            <p>
                <b>KI-gestützt</b><br />
                Unsere Datenaggregierung, die kontextsensitive Inhaltsanalyse und das metrikbasierte Ranking agieren KI-gestützt.
            </p>
        </div>
    </div>
    <div class="grid mt-0 mt-lg-4 pt-lg-3">
        <figure class="grid-image">
            <img loading="lazy" src="diversity.png" alt="Diversity" width="120" height="120" />
            <figcaption>#Diversity</figcaption>
        </figure>
        <div class="grid-content">
            <p>
                <b>Barrierefrei</b><br />
                Barrierefreiheit und Möglichkeiten zur Mehrsprachigkeit gehören für uns zu jeder guten digitalen Lösung dazu.
            </p>
        </div>
        <figure class="grid-image">
            <img loading="lazy" src="mobilefirst.png" alt="UsersFirst" width="120" height="120" />
            <figcaption>#UsersFirst</figcaption>
        </figure>
        <div class="grid-content">
            <p>
                <b>Mobile First</b><br />
                Desktop oder Mobil? Unser Design ist responsiv und bietet damit für jedes Device die optimale User Experience.
            </p>
        </div>
        <figure class="grid-image">
            <img loading="lazy" src="digitalisierung.png" alt="DigitalisierungGestalten" width="120" height="120" />
            <figcaption>#DigitalisierungGestalten</figcaption>
        </figure>
        <div class="grid-content">
            <p>
                <b>Full Stack - Full Service</b><br />
                Neben dem kompletten Software-Produkt mit Backend und Frontend liefern wir auf Wunsch individuelle Beratungsleistungen:
                Projektleitung, Marketing, Trainings, Support.
            </p>
        </div>
    </div>
    <h2>
        <span class="green">#digitalpioneers</span>
    </h2>
    <p class="mb-5">
        CoVerified denkt Information und Kommunikation neu. Entstanden 2020 aus dem #WirvsVirus-Hackathon der
        Bundesregierung arbeiten wir interdiziplinär an digitalen GovTech-Lösungen. Dabei punkten wir als agiles Team
        mit langjähriger Erfahrung in der Kommunikationsbranche und Softwareentwicklung.
    </p>
    <div class="digitalpioneers">
        <img loading="lazy" src="alessa_fetzer.jpg" alt="Alessa Fetzer" width="625" height="625" />
        <img loading="lazy" src="christina_vollnhals.jpg" alt="Christina Vollnhals" width="625" height="625" />
        <img loading="lazy" src="florian_schlittenbauer.jpg" alt="Florian Schlittenbauer" width="625" height="625" />
        <img loading="lazy" src="johannes_hiry.jpg" alt="Johannes Hiry" width="625" height="625" />
        <img loading="lazy" src="julia_diehl.jpg" alt="Julia Diehl" width="625" height="625" />
        <img loading="lazy" src="paula_weise.jpg" alt="Paula Weise" width="625" height="625" />
        <img loading="lazy" src="steven_killian.jpg" alt="Steven Killian" width="625" height="625" />
    </div>
    <Button style="btn-primary" label="CoVerified kennenlernen&nbsp;&#8594;" href="/about" />
</Container>

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
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 12rem 25rem;
        column-gap: 6.25rem;


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
    }

    .column--1-2 {
        grid-column: 1 / -1;
    }

    .column--1 {
        grid-column: 1 / 1;
    }

    .column--2 {
        grid-column: 2 / 2;
    }

    .grid-wrapper {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr min-content;
        grid-gap: 2rem;

        img {
            height: auto;
        }
    }

    .grid-image {
        grid-row: 1 / 1;
        width: 60%;
        margin: 0 auto;
    }

    .grid-text {
        grid-row: 2 / 2;

        b {
            font-size: 1.5rem;
            font-weight: 500;
        }
    }

    .grid {
        display: grid;
        grid-template-columns: repeat(3, auto);
        grid-template-rows: repeat(2, min-content);
        text-align: center;
        column-gap: 6.25rem;
        margin-top: 6.25rem;
    }

    .grid + .grid {
        margin-bottom: 5.625rem;
    }

    .grid-image {
        grid-row: 1 / 2;
    }

    .grid-content {
        grid-row: 2 / 3;

        b {
            font-weight: 500;
            font-size: 1.5rem;
        }
    }

    figure img {
        margin-top: -5px;
    }

    figcaption {
        background-color: var(--color-light-grey);
        border-radius: 2rem;
        padding: 0.6875rem 1.25rem;
        color: var(--color-primary);
        font-size: 0.975rem;
        height: auto;
        margin-bottom: 2.5rem;
        font-weight: 500;
        letter-spacing: 0.45px;
        max-width: 100%;
        margin-top: -0.75rem;
    }

    .digitalpioneers {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(6.25rem, 1fr));
        grid-template-rows: 1fr;
        grid-gap: 1rem;
        margin-bottom: 3rem;

        img {
            display: inline-block;
            width: 100%;
            height: auto;
        }
    }

    .termin__box {
        background-color: var(--color-primary);
        color: var(--color-white);
        border-radius: 60px;
        padding: 2.5rem 9.375rem;

        h2 {
            color: var(--color-white);
            margin-top: 0;
        }
    }

    .social__impact {
        display: grid;
        grid-template-columns: 1fr 1fr;
        column-gap: 8rem;
        background-color: var(--color-light-grey);
        position: relative;
        margin-top: 7.5rem;
        padding-bottom: 3.125rem;

        &:before {
            content: '';
            background-color: var(--color-light-grey);
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

        h2 {
            grid-column: 1 / -1;
            margin-top: 6.25rem;
        }

        p:first-of-type {
            grid-column: 1 / -1;
            margin-bottom: 3.75rem;
        }

        .coverified-tech {
            grid-column: 1 / -1;
            max-width: 100%;
        }

        figcaption {
            background-color: var(--color-white);
        }
    }

    @media (max-width: 992px) {
        h1 {
            font-size: 2rem;
        }

        .social__impact {
            display: flex;
            flex-direction: column;
        }

        .grid-wrapper {
            display: flex;
            flex-direction: column;
        }

        .bg-primary {
            display: flex;
            flex-direction: column;
            padding-top: 3.5rem;
            padding-bottom: 3.5rem;
        }

        .grid {
            display: flex;
            flex-direction: column;
            grid-gap: 0;
        }

        .grid-content {
            margin-bottom: 3rem;
        }
    }

    @media (max-width: 768px) {
        .termin__box {
            padding: 2.5rem 3.375rem;
        }
    }

    @media (max-width: 576px) {
        h1,
        .h1 {
            font-size: 2rem;
        }

        .social__impact {
            margin-top: 3rem;

            h2 {
                margin-top: 3rem;
            }
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
