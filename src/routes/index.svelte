<script>
    import Button from '../components/Button.svelte';
    import Col from 'sveltestrap/src/Col.svelte';
    import Row from 'sveltestrap/src/Row.svelte';
    import Container from 'sveltestrap/src/Container.svelte';
</script>

<style type="text/scss">
    h1,
    .h1 {
        font-size: 3.125rem;
        font-weight: 400;
        color: var(--color-primary);
        line-height: 48px;
        margin-bottom: 2.625rem;        
    }

    h2,
    .h2 {
        font-size: 1.625rem;
        color: var(--color-anthracite);
        font-weight: 800;
        margin-top: 9.875rem;
        margin-bottom: 1.6875rem;
    }

    h3,
    .h3 {
        font-size: 3.75rem;
        margin-bottom: 2.75rem;
        padding-top: 9.375rem;
        
        > span {
            display: block;
            font-size: 1.5625rem;
            font-weight: 500;
            margin-right: auto;
        }
    }

    span.green {
        position: relative;
        z-index: 100;

        &::before {
            content: "";
            background-color: var(--color-green);
            position: absolute;
            height: 60%;
            bottom: -20%;
            width: 100%;      
            z-index: -10;      
        }
    }

    .mt-150 {
        margin-top: 9.375rem;
    }

    .mb-96 {
        margin-bottom: 6rem;
    }

    .bg-primary {
        position: relative;        
        background-color: var(--color-primary) !important;
        z-index: 100;
        padding-top: 7.5rem;
        padding-bottom: 7.5rem;

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
    }

    hr {
        display: inline-block;
        margin-left: 5px;
        margin-right: 5px;
        width: 30%;        
    }

    .circle-1,
    .circle-2,
    .circle-3 {
        position: relative;
        background-color: var(--color-green);
        width: 3.75rem;
        height: 3.75rem;
        border-radius: 10rem;            
        font-size: 1.875rem;
        font-weight: 600;
        margin: 0 auto;
    }

    .circle-1 {
        &:after {
            content: "1";
            position: absolute;
            left: 25px;
            top: 10px;
        }
    }
    .circle-2 {
        &:after {
            content: "2";
            position: absolute;
            left: 23px;
            top: 10px;
        }
    }

    .circle-3 {
        &:after {
            content: "3";
            position: absolute;
            left: 23px;
            top: 10px;
        }
    }

    .mission-bg {
        text-align: left;
    }

    @media (max-width: 992px) {
        h1 {
            font-size: 2rem;
        }

        button + button {
            margin-top: 2.5rem;
        }
       
    }

    @media (max-width: 768px) {

    }

    @media (max-width: 576px) {
        h1 {
            font-size: 1.5rem;
        }
    }
</style>

<svelte:head>
    <title>CoVerified</title>
    <meta name="description" content="CoVerified"/>
</svelte:head>

<h1 class="sr-only">CoVerified</h1>
<Container class="mt-5 pt-3 text-center">
    <h2 class="h1 mt-0">
        CoVerified wurde mit einem Ziel gegründet:<br />
        digitale Kommunikation neu zu denken – <br />
        für eine besser informierte Gesellschaft.
    </h2>
    <p>
        Was passiert mit einer Gesellschaft, die Fakten nicht mehr akzeptiert?  Vom ersten Tag an haben wir daran geglaubt, dass die Wahrheit zu Verbreiten wichtig ist. Wir haben uns zum Ziel gesetzt, gegen Desinformation zu kämpfen und Wissen zu verbreiten – für eine starke und informierte Gesellschaft.
    </p>
    <h2>
        Mehr Wissen <span class="green">für Alle!</span><br />
        Wir machen aus verstreuten Infos <span class="green">geballte Wissenspower.</span>
    </h2>
    <p>
        Doch was macht eigentlich die Bundesregierung, um Lösungen für diese gesellschaftlichen Herausforderungen zu finden? 
        Bisher war es mühsam aktuelle Informationen über gesellschaftlich relevante Themen zu finden. Offizielle Informationen sind verstreut auf hunderten von Seiten im Internet. Soziale Medien und andere Seiten sind voll von Desinformation. 
    </p>
    <Row>
        <Col sm="auto" lg="4" class="flex-column">
            <!-- IMAGE -->
            Wir bündeln Informationen<br />
            an einem Ort…
        </Col>
        <Col sm="auto" lg="4" class="flex-column">
            <!-- IMAGE -->
            …aus vertrauenswürdigen<br />
            Quellen…
        </Col>
        <Col sm="auto" lg="4" class="flex-column">
            <!-- IMAGE -->
            …und bereiten sie<br />
            medial auf.
        </Col>
    </Row>
    <button class="btn-primary mt-150 mb-96">Wie machen wir das?</button>
    <div class=" bg-primary text-white">
        <h2 class="text-white mt-0">
            WiKa - der Wissenskanal für offizielle Informationen
        </h2>
        <p>
            Corona, Klimaschutz, Zuwanderung, Pflege, Digitalisierung… Diese und viele weitere Themen bewegen ganz Deutschland und werden in unserem Widget gesammelt.<br />
            <b>Helfen auch Sie mit und werden Sie Teil der Wissens-Bewegung!</b>        
        </p>
        <!-- Grafiken -->
    </div>
    <h2>
        Sie haben eine Website oder einen Blog?<br />
        <span>
            Perfekt, denn mehr brauchen Sie nicht! <br />
            Helfen Sie mit: <span class="green">In 3 einfachen Schritten</span> gegen Desinformation.
        </span>
    </h2>
    <Row class="justify-content-center">
        <Col sm="auto" lg="4" class="flex-column">
            <div class="circle-1"></div>
            <!-- Image -->
            Unser Widget kostenlos<br />
            herunterladen.
        </Col>
        <Col sm="auto" lg="4" class="flex-column">
            <div class="circle-2"></div>
            <!-- Image -->
            Einfach auf Ihrer Website<br />
            installieren und individuell<br />
            konfigurieren.
        </Col>
        <Col sm="auto" lg="4" class="flex-column">
            <div class="circle-3"></div>
            <!-- Image -->
            Widget auf Ihrer Website<br />
            veröffentlichen – für eine besser<br />
            informierte Gesellschaft.
        </Col>
    </Row>
    <!-- GRafik -->
    <div class="container">
    <!-- Grau -->
        <p>
            <span>„</span>WiKa hat uns geholfen,
        </p>
    </div>
    <h2>
        Sie finden uns schon ganz gut?<br />
        Dann <span class="green">unterstützen Sie uns,</span> damit wir noch besser werden.
    </h2>
    <p>
        Um die Qualität unseres Services noch besser zu machen,
        brauchen wir Eure Hilfe! Unterstützt uns jetzt mit einer Spende oder Investition.
    </p>
    <Row class="justify-content-center">
        <Col sm="auto" lg="6">
            <button class="btn-primary">Mit einer Spende unterstützen</button>
        </Col>
        <Col sm="auto" lg="6" class="mt-3 mt-lg-0">
            <button class="btn-primary">Partner / Investor werden</button>            
        </Col>
    </Row>
    <div class="mission-bg">
        <!-- Bild als Hintergrund -->
        <h3 class="text-white">
            <span>Unsere Mission</span>
            Mehr Wissen für alle -<br />
            sicher kompakt relevant
        </h3>
        <button class="btn-primary">Wer sind wir und wie wollen wir das schaffen?</button>
    </div>
</Container>