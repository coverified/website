<script>
  import Button from '../components/Button.svelte';
  import Col from "sveltestrap/src/Col.svelte";
  import Row from "sveltestrap/src/Row.svelte";
  import Container from "sveltestrap/src/Container.svelte";
  import { onMount } from "svelte";

</script>

<style type="text/scss">
  .bg-primary {
    position: relative;
    background-color: var(--color-primary) !important;
    z-index: 100;
    padding-top: 7.5rem;
    text-align: left;
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

    &--twitter {
      padding-top: 5.4375rem;
      img {
        width: 5%;
      }
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
        opacity: .8;
      }

      &-popup {
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        opacity: 0;
        transition: .25s ease-in;    
        background-color: var(--color-primary);    
        width: 100%;
        height: auto;
        border-radius: 10rem;
        color: var(--color-white);

        &--name {
          font-weight: 500;
          position: absolute;
          top: 2.1875rem;
          left: 0;
          right: 0;          
        }

        &--title,
        &--hashtag {
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

        &--hashtag {
          position: absolute;
          bottom: 0;
          left: 0;
          right: 0;
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

  @media (max-width: 992px) {
    .zitat {
      font-size: 2.25rem;
    } 

    .digitalpioneers {
      grid-template-columns: repeat(auto-fit, 12rem);
      
      .overlay__container {
        &-popup {     
          opacity: .7;

          &--name {
            font-size: 1.15rem;
            top: 1.75rem;
            line-height: 1.5;
          }

          &--title,
          &--hashtag {      
            font-size: 1rem;
          }
       }
      }
    }

    .bg-secondary {
      margin-top: 1.75rem;
    }

    .bg-primary {
      &--twitter {
        img {
          width: 10%;
        }
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

    .bg-primary {
      &--twitter {
        img {
          width: 15%;
        }
      }
    }
  }
  
</style>

<svelte:head>
  <title>Information</title>
</svelte:head>
<Container class="mt-5 pt-3 text-center">
  <h1>Wir sind CoVerified</h1>
  <p>
    Ein Wochenende im März war die Geburtsstunde von CoVerified: 3 Entwickler
    aus Bayern stürzten sich mit knapp 30.000 anderen in den #WirvsVirus
    Hackathon. Im Kopf die Idee, aktiv gegen Desinformation und die Spaltung
    der Gesellschaft vorgehen. Das Wochenende endete nicht nur mit neuen
    Team-Membern und einem funktionsfähigen Prototypen, sondern mit dem
    unglaublichen Gefühl, Teil einer besonderen Community zu sein und als
    Zivilgesellschaft an Lösungen aktiv mitwirken zu können.
  </p>
  <div class="bg-primary text-white mt-5">
    <p class="zitat">
      „Nach unserer Überzeugung gibt es kein größeres und wirksameres Mittel
      zu wechselseitiger Bildung als das Zusammenarbeiten.“
    </p>
    <p>Johann Wolfgang von Goethe</p>
  </div>
  <h2 class="mt-5">
    <span class="green">Unsere Mission</span>
  </h2>
  <p>
    CoVerified denkt staatliche Kommunikation neu.
  </p>
  <Row class="text-left mt-5">
    <Col sm="auto" lg="4">
      <p class="text-primary">
        #Demokratie
      </p>
      <p>
        Wir glauben, dass eine gut
        informierte Bevölkerung der
        Schlüssel zu einer funktionierenden
        Gesellschaft ist und Bildung das
        Vertrauen in staatliche
        Entscheidungen fördert.
        Gesichertes Wissen leicht
        zugänglich machen und in der
        Breite der Bevölkerung für
        Faktensicherheit sorgen, ist das
        Ziel von Coverified.
        Denn Wissen fördern und
        Demokratie stärken sind wichtiger
        denn je.
      </p>
    </Col>
    <Col sm="auto" lg="4" class="mt-3 mt-md-0">
      <p class="text-primary">
        #OpenSocialInnovation
      </p>
      <p>
        Mit der Idee im Kopf und Leidenschaft
        im Herzen sind wir in den Hackathon
        #WirvsVirus 2020 gestartet. Seite an
        Seite mit knapp 150 Projekten haben
        wir Lösungen für die Probleme im
        Zuge der COVID-19-Pandemie
        entwickelt.
        Wir sind überzeugt, dass Open Social
        Innovation dem großen
        Innovationspotential der
        Zivilgesellschaft die Tür öffnet und
        gelebte Partizipation wunderbare
        Lösungen für viele gesellschaftliche
        Herausforderungen bereithält.
      </p>
    </Col>
    <Col sm="auto" lg="4" class="mt-3 mt-md-0">
      <p class="text-primary">
        #Digitalisierung
      </p>
      <p>
        Eine breit informierte Öffentlichkeit
        erreichen wir, wenn neue digitale
        Kanäle eine schnelle und
        niedrigschwellige Information der
        Bevölkerung ermöglichen. Wir bei
        CoVerified arbeiten daran, den
        Herausforderungen unserer Zeit mit
        innovativen Kommunikationswegen
        zu begegnen und neue
        Informationsstandards zu setzen.
      </p>
    </Col>
  </Row>
  <h2>
    <span class="green">#digitalpioneers</span>
  </h2>
  <p>
    Das ist das interdisziplinäre Team, das mit Herzblut hinter
    CoVerified steht. 9 Expert:innen, die sich remote gefunden haben,
    um gemeinsam etwas zu bewirken und Open Social Innovation von
    der Idee bis zur Umsetzung zu gestalten.
  </p>
  <div class="digitalpioneers">
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    <div class="overlay__container">
      <img src="baerbel.png" alt="Bärbel" class="turn ">
      <div class="overlay__container-popup">
        <p class="overlay__container-popup--name">
          Johannes Hiry<br />
          <span class="overlay__container-popup--title">Webentwickler</span>
        </p>
        <div class="overlay__container-popup--links">
          <a href="#">
            <img src="xing.svg" alt="Xing Logo">
          </a>
          <a href="#">
            <img src="linkedin.svg" alt="linkedIn Logo">
          </a>
        </div>
        <p class="overlay__container-popup--hashtag">
          #kitesurfass
        </p>
      </div>
    </div>  
    
  </div>
  <div class="bg-secondary">
    <h2 class="mt-0">
      <span class="green--light-grey">#Unser Leistungsprofil</span>
    </h2>
    <p>
      Wir begleiten Kommunikationsprojekte von der Idee bis zur Umsetzung
    </p>
    <Row class="text-left my-5">
      <Col sm="auto" lg="3">
        <p class="text-primary">
          Software-Entwicklung
        </p>
        <p>
          Von Strategie und Konzeption über Design und Programmierung bis zur Implementierung.
        </p>
      </Col>
      <Col sm="auto" lg="3">
      <p class="text-primary">
          Projektmanagement
        </p>
        <p>
          Beratung, Projektleitung und Abstimmung mit allen Beteiligten
        </p>
      </Col>
      <Col sm="auto" lg="3">
      <p class="text-primary">
          Marketing & Kommunikation
        </p>
        <p>
          Planung, Gestaltung und Umsetzung von Kommunikations-Maßnahmen z.B. Kampagne
        </p>
      </Col>
      <Col sm="auto" lg="3">
      <p class="text-primary">
          Service & Maintainance
        </p>
        <p>
          Betreuung von Einbindung und Betrieb der Kommunikations-Lösungen
        </p>
      </Col>
    </Row>
    <Button label="Jetzt Kontakt aufnehmen&nbsp;&#8594;" href="/contact" style="btn-primary"></Button>
  </div>
  <div class="bg-primary bg-primary--twitter text-center">
    <img src="twitter.svg" alt="twitter logo">
    <h3 class="text-white h1">
      Werde Teil unserer Mission und folge uns auf Twitter
    </h3>
    <Button style="btn-secondary" href="https://twitter.com/CoVeri_fied" target="_blank" rel="noopener" label="CoVerified auf Twitter folgen"></Button>
  </div>
</Container>