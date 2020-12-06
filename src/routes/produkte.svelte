<script>
  import Button from "../components/Button.svelte";
  import Container from "sveltestrap/src/Container.svelte";
  import PlaceholderImage from "../components/PlaceholderImage.svelte";
  import { onMount } from 'svelte';

  onMount(() => {
    
    const faders = document.querySelectorAll('.fade-in');
    const appearOptions = {
        threshold: 1,
        rootMargin: '0px 0px -150px 0px'
    };
    const appearOnScroll = new IntersectionObserver(function(entries, appearOnScroll) {
      entries.forEach(entry => {        
        if (!entry.isIntersecting) {
          return;
        } else {
          entry.target.classList.add('appear');
          appearOnScroll.unobserve(entry.target);
        }
      });
    },
    appearOptions);

    faders.forEach(fader => {
      appearOnScroll.observe(fader);
    });
  });
</script>

<style type="text/scss">
    .grid-wrapper,
    .grid-wrapper-mirrored {
        display: grid;
        text-align: left;
    }

    .grid-wrapper {
        grid-template-columns: 32rem 1fr;
        grid-gap: 10.625rem;        
    }

    .grid-wrapper-mirrored {
        grid-template-columns: 1fr 32rem;
        grid-gap: 9.375rem;
        margin-top: 7.75rem;
    }

    .fade-in {
        opacity: 0;
        transition: opacity 250ms ease-in;
    }

    /* Set to global for intersectionobserver */
    :global(.appear) {
        opacity: 1 !important;
    }

    .kacheln-wrapper {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1fr 1fr;
    }
    
    .mt--40 {
        margin-top: -2.5rem;
    }

    .bg-wika {
        position: relative;
        background-color: var(--color-wika);
        z-index: 100;
        padding-top: 8rem;
        padding-bottom: 3.875rem;
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: 6rem 4.5rem 1fr;
        row-gap: 1.25rem;
        column-gap: 2.75rem;
        color: var(--color-white);
        margin-top: 6.25rem;

        .image {
            width: 23%;
            display: flex;
            margin: 0 auto;
        }

        &:before {
            content: "";
            background-color: var(--color-wika);
            position: absolute;
            display: block;
            width: 100vw;
            height: 100%;
            left: 50%;
            transform: translate(-50%);
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
            top: 0;
            border-width: 3rem 3rem 0 3rem;
            border-color: var(--color-white) transparent transparent transparent;
            left: 50%;
            transform: translate(-50%, 0);
        }
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

    .col--1-4 {
        grid-column: 1 / -1;
    }

    .col--1 {
        grid-column: 1 / 1;
    }

    .col--2 {
        grid-column: 2 / 2;
    }

    .col--3 {
        grid-column: 3 / 3;
    }
    .col--4 {
        grid-column: 4 / 4;
    }

    @media (max-width: 992px) {
        .grid-wrapper,
        .grid-wrapper-mirrored,
        .kacheln-wrapper,
        .bg-wika {
            display: flex;
            flex-direction: column;
        }

        .grid-wrapper,
        .grid-wrapper-mirrored {
            margin-top: 3rem;
            grid-gap: 2rem;
        }

        .bg-wika {
            padding-top: 0;
        }
    }

    @media (max-width: 768px) {
      .fade-in {
        opacity: 1;
      }

      .h2 {
        margin-top: 4.735rem;
      }
    }
</style>

<svelte:head>
  <title>Wika | Das Web-Widget gegen Desinformation</title>
  <meta name="description" content="Gemeinsam gegen Desinformation – Wika macht sichere
Informationen zu gesellschaftsrelevanten Themen auf
Knopfdruck webweit verfügbar."/>
</svelte:head>
<Container class="mt-5 pt-3 text-center mb-3">
  <h1>Wika –  Das Web-Widget gegen Desinformation</h1>
  <p>
    Gemeinsam gegen Desinformation – Wika nutzt das CoVerified-Prinzip und macht sichere Informationen zu gesellschaftsrelevanten Themen auf Knopfdruck auf jeder Website verfügbar.
  </p>
</Container>
<PlaceholderImage
    url="wika-header.jpg"    
    alt="Wika"
    placeholder=".jpg"
    width="2500"
    height="1572"
>
</PlaceholderImage>
  <Container class="text-center">
  <h2 class="mb-5 h2">
    <span class="green">Die Wika-Features im Überblick</span>
  </h2>
  <div class="grid-wrapper">
    <div>
      <h3 class="h2 mt-0">
        Bequemer Einstieg
        <br />
        über aktuelle Stories
      </h3>
      <p>
        So erhalten Nutzer:innen die wichtigsten Meldungen angenehm aufbereitet
        auf den ersten Blick. Von hier braucht es nur einen Fingertipp, um
        weiter ins Detail einzusteigen oder noch mehr interessante Themen zu
        entdecken.
      </p>
      <p>
        <b>Optionen bei Einbindung:</b>
      </p>
      <ul>
        <li>Priorisierung ausgewählter Stories</li>
        <li>Erstellung eigener Stories durch Templates</li>
      </ul>
    </div>
    <div>
      <img loading="lazy" src="story-element.png" width="1120" height="1318" alt="Our image">
    </div>
  </div>
  <div class="grid-wrapper-mirrored">
    <div class="kacheln-wrapper">
      <img src="themen_kachel_1.png" alt="WiKa Themenkachel" class="fade-in" width="436" height="614" />
      <img src="themen_kachel_2.png" alt="WiKa Themenkachel" class="fade-in" width="436" height="690" />
      <img src="themen_kachel_3.png" alt="WiKa Themenkachel" class="fade-in mt--40" width="436" height="722" />
      <img src="themen_kachel_4.png" alt="WiKa Themenkachel" class="fade-in" width="436" height="702" />
    </div>
    <div>
      <h2 class="mt-0">
        Gesellschaftlich relevante Themen übersichtlich gebündelt
      </h2>
      <p>
        Corona, Klimaschutz, Zuwanderung, Pflege, Digitalisierung… Diese und
        viele weitere Themen bewegen ganz Deutschland und werden in unserem
        Widget gesammelt und per Klick ausgegeben.
      </p>
      <p>
        <b>Optionen bei Einbindung:</b>
      </p>
      <ul>
        <li>Auswahl von Themen passend zum Kontext der eigenen Webseite</li>
        <li>Eigene Themen und Fragestellungen ergänzen</li>
      </ul>
      <img loading="lazy" src="themen_chips.svg" width="300" height="72" alt="Our image">
    </div>
    </div>
    <div class="bg-wika">
        <h2 class="row--1 col--1-4 mt-lg-0 text-white">
            Die 4 Wika-Wissenskategorien
        </h2>
        <p class="pt-lg-5 mb-4 row--1 col--1-4">
          Schnell und gezielt navigieren - Wika bietet für jeden Informationsbedarf den passenden Inhalt.
        </p>    
        <div class="row--2 col--1 image">
          <img loading="lazy" src="chat_bubble_outline.svg" width="154" height="150" alt="Staatus">
        </div>
        <p class="row--3 col--1">
            <b>Staatus</b><br/>
            staatliche Meldungen aus den Ministerien, aktuelle Beschlüsse und Diskussionen
        </p>
        <div class="row--2 col--2 image">
          <img loading="lazy" src="school.svg" width="186" height="150" alt="Basiswissen">
        </div>
        <p class="col--2 row--3">
          <b>Basiswissen</b><br/>
          Grundlagen zu gesellschaftsrelevanten Themen
        </p>
        <div class="row--2 col--3 image">
          <img loading="lazy" src="favorite_border.svg" width="165" height="150" alt="Engagement">
        </div>
        <p class="row--3 col--3">
          <b>Engagement</b><br/>
          Ausgewählte Initiativen werden vorgestellt, um selbst aktiv zu werden
        </p>
        <div class="row--2 col--4 image">
          <img loading="lazy" src="help_outline.svg" width="154" height="150" alt="Nachgefragt">
        </div>        
        <p class="row--3 col--4">
            <b>Nachgefragt</b><br />
            Antworten auf die drängendsten Fragen der Bürger*innen
        </p>
    </div>
    <h2 class="h2">
        <span class="green">Transparent gegen Desinformation</span>
    </h2>
    <p>
        Wir legen Wert auf unverfälschte Informationen aus erster Hand. Unsere Quellen werden nach festgelegten, transparenten Kriterien ausgewählt, beleuchtet und bei jedem Inhalt verlinkt.
    </p>
    <p>
        <b>Optionen bei Einbindung:</b>
    </p>
    <p>
        Priorisierung von Quellen passend zum Kontext der eigenen Webseite
    </p>
    <h2>
        Eine besser informierte Gesellschaft ist Dir wichtig?<br />
        <span class="green">Dann unterstütze uns</span> und unser Projekt
    </h2>
    <p>
        Derzeit arbeiten wir ehrenamtlich daran und freuen uns über Support.
    </p>
    <div class="mb-120 mt-5">
        <Button style="btn-primary mb-5" label="Partner:in/Investor:in werden" href="/contact"></Button>
    </div>
</Container>
