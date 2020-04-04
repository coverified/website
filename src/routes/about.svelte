<script>
  import Header from "../components/Header.svelte";
  import List from "../components/List.svelte";
</script>

<style type="text/scss">
  main {
    padding-left: 1.5rem;
    padding-right: 1.5rem;
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
    
  }

  @media (max-width: 576px) {
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

<Header pageName={'Informationen'}/>
<main>
  <h2>
    So funktioniert CoVerfied
  </h2>
  <p>
    CoVerified sammelt Daten aus verifizierten Quellen im Internet, bündelt diese in einer Datenbank 
    und gibt sie als News-Vorschau über unser Informations-Tool (der Button auf Ihrer Website unten rechts) 
    aus. Es gibt noch kein vergleichbares Angebot, das zentral die wichtigsten, validierten Daten bündelt 
    wie zum Beispiel vom Robert-Koch-Institut, der Bundesregierung und dem Ministerium für Gesundheit. 
    Wir wollen sicher gehen, dass wirklich nur Informationen aus wissenschaftlichen oder staatlichen 
    Quellen genutzt werden.
  </p>
  <div>
    <img class="coverified__informationgraphic" src="coverified-information-graphic.svg" alt="Coverified Information graphic">
    <p>
      Unsere Datenbank wird gefüttert mit allen aktuellen Daten aus den RSS-Feeds offizieller Stellen. Diese 
      Informationen werden als News-Vorschau in unserem Tool dargestellt. Klickt oder tippt der Nutzer auf ein 
      solches Vorschau-Feld, wird er direkt zur aktuellen Meldung auf die Seite der jeweiligen Quelle weitergeleitet. 
    </p>
  </div>
  <h2>
    Proaktiv gegen Falschmeldungen (Fake News) im Netz
  </h2>
  <p>
    Unser Ziel ist es, proaktiv gegen Falschmeldungen zu arbeiten in dem wir auf (möglichst) vielen Internetangeboten 
    verifizierte Informationen zur Verfügung stellen. Damit schaffen wir eine umfängliche Information der Bevölkerung 
    und damit Vertrauen in politische Entscheidungen. Es geht dabei nicht um die kontinuierliche Information der 
    Bürger*innen über das polit. Zeitgeschehen, sondern ausdrücklich um das Bereitstellen von wissenschaftl. überprüften 
    Fakten in Ausnahmesituationen. Das Widget kann auch zu einem späteren Zeitpunkt auf andere Krisen angepasst werden 
    wie z.B. Naturkatastrophen. 
  </p>
  <h2>
    Wir sind ein Projekt des #WirvsVirus Hackathons
  </h2>
  <p>
    Die Idee zu unserem Informations-Tool ist beim #WirvsVirus Hackathon entstanden. Der Hackathon war eine Veranstaltung im 
    Internet der Bundesregierung. Dort wurden Lösungen für die aktuelle Covid19-Krise erarbeitet und programmiert. Sie sehen 
    hier unsere Idee und den aktuellen Stand. Unser Code-Schnipsel kann bereits in Websites eingebunden werden und unsere 
    Datenbank sammelt aktuelle Informationen. 
  </p>
  <p>
    Wir arbeiten stetig weiter an unserem Projekt und freuen uns über Lib, gleich wohl wie Kritik, Feedback, Anregungen 
    oder auch WoMan-Power. 
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
</main>


