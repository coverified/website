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
    height: 14.6875rem;
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

    .wirvsvirus__logo {
        position: absolute;
        width: 20rem;
        bottom: 37%;
        right: 1.125rem;
    }

  p {
    margin-bottom: 2.5rem;
  }

  h1 {
    font-size: 2rem;
    color: var(--color-primary);
  }

  h2 {
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

  .project-heading {
    width: 13rem;
    position: absolute;
    top: 2rem;
    left: 0;
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
    height: 16.6875rem;
    justify-content: flex-start;
    
      > h1 {
          top: 0;
      }

      > .wirvsvirus__logo {
          bottom: unset;
          top: .3125rem;
          right: auto;
          width: 20rem;
      }
    }
    .project-heading {
      width: 11rem;
      top: 7rem;
      left: unset;
    }
  }
  
  @media (max-width: 576px) {
    
    h1 {
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
    <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
    <img src="project-header.svg" alt="das Projekt" class="project-heading">
</header>
<main>
  <h1>
    Ein Projekt des #WirVsVirus Hackathons <br class="d-none d-lg-block"/> der Bundesregierung im März 2020.
  </h1>
  <h2>
    Wir sind ein von der Bundesregierung gefördertes Projekt
  </h2>
  <p>
    Die Idee zu unserem Informations-Tool ist beim von der Bundesregierung initiierten #WirVsVirus Hackathon entstanden. Hier wurden Lösungen für die aktuelle Covid-19 Krise entworfen, programmiert und umgesetzt – komplett remote und organisiert in Teams aus engagierten Bürger*innen. CoVerified ist die Idee unseres Teams. Unseren Code können Sie in Ihre Websites einbinden, um Besucher*innen aktuelle Informationen zu Covid-19 bereitzustellen – aus verifizierten Quellen und mit nur einem Klick. So helfen Sie mit, die Verbreitung von Falschmeldungen zu verhindern.
  </p>
  <p>
    Nach dem Hackathon ist vor dem Hackathon: Wir arbeiten weiter an unserem Projekt und freuen uns über Feedback, Anregungen oder auch WoMan-Power. Damit wir zusammen noch besser werden und verlässliche Informationen für alle bereitstellen.
  </p>
  <p>
    Unser Projekt ist eine Non-Profit-Lösung, unser Code wurde in OpenSource geschrieben.
  </p>
  <p>
    Unsere Projektbeschreibung und die Dokumentation beim #WirVsVirus Hackathon finden Sie hier: 
    <a href="https://devpost.com/software/1_039_c_staatlichekommunikation_webinfowidget" title="Projektbeschreibung" target=“_blank“ rel=“noopener“>
      Devpost
    </a>
  </p>
  <h2>
    Unsere Motivation
  </h2>
  <p>
    Unser Ziel ist es, proaktiv gegen Falschmeldungen zu arbeiten. Daher haben wir das CoVerified Tool entwickelt. Es bringt Informationen aus seriösen Quellen zusammen und bündelt diese in einem Widget. So schaffen wir es, umfänglich zu Covid-19 zu informieren. Im Detail heißt das: Es werden Informationen aus den einzelnen Bundesländern, sowie medizinische Ratschläge, Erkenntnisse aus der Forschung oder Verhaltensratschläge gebündelt und aktuell zur Verfügung gestellt. Dabei geht es uns vor allem um das Bereitstellen von wissenschaftlich überprüften Fakten in Ausnahmesituationen wie der Covid-19 Krise. Es ist allerdings auch möglich, das Widget zu einem späteren Zeitpunkt auf andere Krisen anzupassen, zum Beispiel beim Ausbruch von Naturkatastrophen wie Waldbränden oder Überschwemmungen.
  </p>
  <h2>
    So funktioniert es
  </h2>
  <p>
    CoVerified sammelt Daten aus verifizierten Quellen im Internet, bündelt diese in einer Datenbank und gibt sie als News-Vorschau über unser Informations-Tool (der Button auf Ihrer Website unten rechts) aus. Es gibt noch kein vergleichbares Angebot, das zentral die wichtigsten, validierten Daten bündelt wie zum Beispiel vom Robert-Koch-Institut, der Bundesregierung und dem Ministerium für Gesundheit. Wir wollen sicher gehen, dass wirklich nur Informationen aus wissenschaftlichen oder staatlichen Quellen genutzt werden.
  </p>
  <p>
    Unsere Datenbank wird gefüttert mit allen aktuellen Daten aus den RSS-Feeds offizieller Stellen. Diese Informationen werden als News-Vorschau in unserem Tool dargestellt. Klickt oder tippt der Nutzer auf ein solches Vorschau-Feld, wird er direkt zur aktuellen Meldung auf die Seite der jeweiligen Quelle weitergeleitet.
  </p>
</main>


