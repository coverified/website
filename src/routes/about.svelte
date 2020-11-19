<script>
  import Button from '../components/Button.svelte';
  import Col from "sveltestrap/src/Col.svelte";
  import Row from "sveltestrap/src/Row.svelte";
  import Container from "sveltestrap/src/Container.svelte";
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

  .author {
    font-weight: bold;
    margin-top: 1.875rem;
  }

  @media (max-width: 992px) {
    .zitat {
      font-size: 2.25rem;
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
  <!-- Bilder einfügen -->
  <div class="bg-secondary ">
    <h2 class="mt-0">
      <span class="green">#Unser Leistungsprofil</span>
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
    <Button label="Jetzt Kontakt aufnehmen&nbsp;&#8594;" style="btn-primary"></Button>
  </div>
  <div class="bg-primary text-center">
    <h3 class="text-white h1">
      Werde Teil unserer Mission und folge uns auf Twitter
    </h3>
    <Button style="btn-secondary" label="CoVerified auf Twitter folgen"></Button>
  </div>
</Container>