<script>
  import Header from "../components/Header.svelte";
  import List from "../components/List.svelte";
</script>

<style type="text/scss">
  main {
    padding-left: 1.5rem;
    padding-right: 1.5rem;
  }

  header {
    background-color: var(--color-primary);
    height: 18vh;
    position: relative;
    justify-content: center;
    display: flex;
    margin-bottom: 3rem;
    
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
    }

    h1 {
        font-size: 2rem;
        position: relative;
        color: var(--color-white);
        top: 68%;
        left: 1.8%;
    }

    .wirvsvirus__logo {
        position: absolute;
        width: 20rem;
        bottom: 37%;
        right: 1.125rem;
    }

  p {
    margin-bottom: 2.5rem;
  }

  h2 {
    font-size: 2rem;
    color: var(--color-primary);
  }

  h3 {
    font-size: 1.625rem;
    margin-top: 5.0625rem;
    margin-bottom: .6875rem;  
  }

  div {
    display: flex;
    justify-content: space-between;
    margin-bottom: 3rem;

    > .coverified__informationgraphic {
      width: 45%;
      background-color: var(--color-primary);
      padding: 1.5rem;
      margin-right: 2rem;
      margin-bottom: 1rem;
      margin-top: 1rem;
    }
  }

  @media (max-width: 992px) {
    main {
      padding-left: 0;
      padding-right: 0;
    }
  }
  @media (max-width: 768px) {
    header {
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    
      > h1 {
          top: 0;
      }

      > .wirvsvirus__logo {
          bottom: 1rem;
          right: auto;
          width: 20rem;
      }
    }
  }

  @media (max-width: 576px) {
    
    h2 {
            font-size: 1.575rem;
        }

    div {
      flex-direction: column;
      align-items: center;

      > .coverified__informationgraphic {
        width: 100%;
        margin-right: 0rem;
      }
    }
  }
</style>

<svelte:head>
	<title>Information</title>
</svelte:head>

<header>
    <h1 class="sr-only">das Projekt</h1>
    <h1>
        das Projekt
    </h1>
    <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
</header>
<main>
  <h2>
    Ein Projekt entstanden beim Hackathon<br class="d-none d-lg-block"/> der Bundesregierung im März 2020.
  </h2>
  <h3>
    Wir sind ein von der Bundesregierung gefördertes Projekt
  </h3>
  <p>
    Die Idee zu unserem Informations-Tool ist beim #WirvsVirus Hackathon entstanden. Der Hackathon wurde von der Bundesregierung initiiert. Es wurden Lösungen für die aktuelle Covid19-Krise via Internet von neu gebildeten Teams aus interessierten Bürger*innen erarbeitet und programmiert. CoVerified war die Idee unseres Teams. Unser Code-Schnipsel kann in Websites eingebunden werden, um Besucher*innen aktuelle Informationen verifizierter Quellen aus unserer Datenbank bereitzustellen.
  </p>
  <p>
    Wir arbeiten stetig weiter an unserem Projekt und freuen uns über Lob, gleich wohl wie Kritik, Feedback, Anregungen oder auch WoMan-Power.
  </p>
  <p>
    Unser Projekt ist eine Non-Profit Lösung, unser Code wurde in OpenSource geschrieben.
  </p>
  <p>
    Unsere Projektbeschreibung und die Dokumentation beim #WirvsVirus Hackathon finden Sie hier: 
    <a href="https://devpost.com/software/1_039_c_staatlichekommunikation_webinfowidget" title="Projektbeschreibung" target=“_blank“ rel=“noopener“>
      Devpost
    </a>
  </p>
  <h3>
    Unsere Motivation
  </h3>
  <p>
    Unser Ziel ist es, proaktiv gegen Falschmeldungen zu arbeiten in dem wir ein Tool zur Verfügung stellen, welches Informationen aus seriösen Quellen zieht und in einem Widget bündelt. So schaffen wir es, mit nur einem Tool, umfängliche Informationen zu Covid-19 bereitzustellen. Es werden Informationen aus den einzelnen Bundesländern, medizinische Ratschläge, Erkenntnisse aus der Forschung oder Verhaltensratschläge gebündelt und aktuell zur Verfügung gestellt. Dabei geht es uns vor allem um das Bereitstellen von wissenschaftl. überprüften Fakten in Ausnahmesituationen. So kann das Widget auch zu einem späteren Zeitpunkt auf andere Krisen angepasst werden z. B. bei Naturkatastrophen.
  </p>
  <h3>
    So funktioniert es
  </h3>
  <p>
    CoVerified sammelt Daten aus verifizierten Quellen im Internet, bündelt diese in einer Datenbank und gibt sie als News-Vorschau über unser Informations-Tool (der Button auf Ihrer Website unten rechts) aus. Es gibt noch kein vergleichbares Angebot, das zentral die wichtigsten, validierten Daten bündelt wie zum Beispiel vom Robert-Koch-Institut, der Bundesregierung und dem Ministerium für Gesundheit. Wir wollen sicher gehen, dass wirklich nur Informationen aus wissenschaftlichen oder staatlichen Quellen genutzt werden.
  </p>
  <p>
    Unsere Datenbank wird gefüttert mit allen aktuellen Daten aus den RSS-Feeds offizieller Stellen. Diese Informationen werden als News-Vorschau in unserem Tool dargestellt. Klickt oder tippt der Nutzer auf ein solches Vorschau-Feld, wird er direkt zur aktuellen Meldung auf die Seite der jeweiligen Quelle weitergeleitet.
  </p>
</main>


