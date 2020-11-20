<script>
    import Button from '../components/Button.svelte';
    import Col from 'sveltestrap/src/Col.svelte';
    import Row from 'sveltestrap/src/Row.svelte';
    import Container from 'sveltestrap/src/Container.svelte';
</script>

<style type="text/scss">
    .mt-150 {
        margin-top: 9.375rem;
    }

    .mt-120 {
        margin-top: 7.5rem;
    }

    .mt-150 {
        margin-top: 9.375rem;
    }

    .mb-96 {
        margin-bottom: 6rem;
    }

    .mb-120 {
        margin-bottom: 7.5rem;
    }

    .bg-primary {
        position: relative;        
        background-color: var(--color-primary) !important;
        z-index: 100;
        padding-top: 7.5rem;
        padding-bottom: 7.5rem;
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

        img {
            width: 60%;
        }
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

        h2 br {
            display: none;
        }

        button + button {
            margin-top: 2.5rem;
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

            img {
                width: 30% !important;
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
</style>

<svelte:head>
    <title>CoVerified</title>
    <meta name="description" content="CoVerified"/>
</svelte:head>
<Container class="mt-5 pt-3 text-center">
    <h1 class="h1 mt-0">
        #fightingDesinformation – <br />
        Wir denken digitale Information neu.
    </h1>
    <p>
         Denn eine gut informierte Gesellschaft ist die Basis einer starken Demokratie.
    </p>
    <h2>
        Mehr Wissen <span class="green">für alle</span>.        
    </h2>
    <p>
        Sichere Informationen gebündelt, ansprechend und webweit verfügbar
    </p>
    <div class="grid-wrapper mt-5">
        <div class="grid-image">
            <img src="diesituation.png" alt="Die Situation" class="w-50">
        </div>
        <div class="grid-text">
            <p>
                <b>Die Situation:</b><br />
                Verlässliche Informationen sind im Netz verstreut und mühsam zu finden
            </p>
        </div>    
        <div class="grid-image">
            <img src="unsereloesung.png" alt="Unsere Lösung">                
        </div>
        <div class="grid-text">
            <p>
                <b>Unsere Lösung:</b><br />
                Wir bündeln Infos sicherer Quellen in einer zentralen Datenbank und machen sie kompakt, ansprechend und einfach verfügbar
            </p>
        </div>
        <div class="grid-image">
            <img src="unserevision.png" alt="Unsere Vision">
        </div>    
        <div class="grid-text">
            <p>
                <b>Unsere Vision:</b><br /> 
                eine informierte, faktensichere, breite Öffentlichkeit mit mehr Verständnis, Weitsicht und Toleranz
            </p>
        </div>    
    </div>
    <div class=" bg-primary text-white mt-120">
        <div class="column--1-3 row--1">
            <h2 class="text-white mt-0">
                Die CoVerified Lösung für mehr Wissen im Netz:
            </h2>
            <img src="logo-wika.svg" alt="Wika Logo" class="w-25 mb-4">
            <p class="mb-5 mb-md-0 font-weight-300">
                Corona, Klimaschutz, Zuwanderung, Pflege, Digitalisierung... diese und viele weitere Themen bewegen ganz Deutschland. Aber wo kann man verlässliche Informationen dazu finden? Wika bündelt unverfälschte Meldungen aus erster Hand und macht sie bequem und ansprechend webweit verfügbar.    
            </p>
        </div>
        <div class="row--2 column--1 d-flex justify-content-center flex-column align-items-center">
            <img src="icon_story.png" alt="Story Elemente" class="w-50 mb-4">
            <p>
                Bequemer Einstieg über attraktives Story-Element
            </p>
        </div>        
        <div class="row--3 column--1 d-flex justify-content-center flex-column align-items-center">
            <img src="icon_themenauswahl.png" alt="Themenauswahl" class="mb-4">
            <p>
                Gezieltes Informieren über Auswahl von Themen
            </p>
        </div>
        <div class="column--2 row--2-3">
            <video class="animation mx-auto my-5" src="widgetanimation.mov" preload=”none” controls></video>        
            <Button style="btn-secondary" label="Demo-Version testen!"></Button>        
        </div>
        <div class="row--2 column--3 d-flex justify-content-center flex-column align-items-center mt-5 mt-md-0">
            <img src="icon_kuratieren.svg" alt="Kuratierte Inhalte" class="mb-4 w-75">
            <p>
                Kuratierte Inhalte zu nutzer*innen-zentrierten Fragestellungen
            </p>
        </div>
        <div class="row--3 column--3 d-flex justify-content-center flex-column align-items-center">
            <img src="icon_trends.svg" alt="Automatische Relevanzsortierung" class="w-50 mb-4">
            <p>
                Automatische Relevanz-Sortierung nach Themen-Trends im Netz
            </p>
        </div>
    </div>
    <h2>
        Wika <span class="green">bringt Wissen zu den Menschen</span> - ohne zusätzlichen Aufwand
    </h2>
    <div class="grid-wrapper mb-5">
        <div class="grid-image">
            <img src="rss-feed.png" alt="Die Situation" class="w-50">
        </div>
        <div class="grid-text">
            <p>
                Wir nutzen bestehende RSS Feeds – somit entsteht <b>kein zusätzlicher redaktioneller Aufwand</b>
            </p>        
        </div>        
        <div class="grid-image align-items-center d-flex justify-content-center">
            <img src="webeinbindung.png" alt="Unsere Lösung"> 
        </div>
        <div class="grid-text">
            <p>
                Unser Widget ist webweit einbindbar – Informationen bekommen damit eine <b>enorme Reichweite</b>
            </p>
        </div>
        <div class="grid-image">
            <img src="nutzerinzentriert.png" alt="Unsere Vision">
        </div>
        <div class="grid-text">
            <p>
                Unsere Lösung ist <b>nutzer:innen-zentriert</b> entwickelt – somit erreichen wir eine <b>höhere Akzeptanz</b> breiten Bevölkerung
            </p>
        </div>
    </div>
    <Button style="btn-primary" label="Unsere Technologie&nbsp;&#8594;"></Button>
    <h2>
        <span class="green">#digitalpioneers</span>        
    </h2>
    <p class="mb-5">Hinter CoVerified stehen 9 Expert:innen mit Leidenschaft für Open Social Innovation</p>
    <div class="digitalpioneers">
        <img src="baerbel.png" alt="Bärbel">
        <img src="baerbel.png" alt="Bärbel">
        <img src="baerbel.png" alt="Bärbel">
        <img src="baerbel.png" alt="Bärbel">
        <img src="baerbel.png" alt="Bärbel">
        <img src="baerbel.png" alt="Bärbel">
        <img src="baerbel.png" alt="Bärbel">
        <img src="baerbel.png" alt="Bärbel">
        <img src="baerbel.png" alt="Bärbel">
    </div>
    <Button style="btn-primary" label="CoVerified kennenlernen&nbsp;&#8594;"></Button>
    <h2>
        Eine besser informierte Gesellschaft ist Ihnen wichtig?
    </h2>
    <p>
        <span class="green">Dann unterstützen Sie unser Projekt</span> und werden Sie Teil der Wissens-Bewegung.
    </p>
    <div class="mb-120 mt-5">
        <Button style="btn-primary mb-5" label="Partner:in/Invesotr:in werden"></Button>
    </div>
</Container>