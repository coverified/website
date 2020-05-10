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
    margin-bottom: 2rem;
  }

  h2,
  .h2 {
    font-size: 1.625rem;
    margin-top: 5.0625rem;
    margin-bottom: .6875rem;  
    font-weight: 800;
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
  <h1 class="h2">
   Im Hackathon der Bundesregierung geboren
  </h1>
  <p>
    Die Idee entstand beim #WirVsVirus Hackathon, der vom 20. bis 22. März 2020 stattfand. Die Bundesregierung rief im Rahmen des Hackathons dazu auf, Lösungen für die Covid-19 Krise zu entwickeln. In remote arbeitenden Teams aus ganz Deutschland wurden Lösungen zu den unterschiedlichsten Problemen der Krise entworfen und bis heute umgesetzt.
  </p>
  <p>
    <u>Das Problem:</u> Woher bekommt die Bevölkerung zuverlässige, seriöse und aktuelle Informationen in der Coronakrise?
  </p>
  <p>
    <u>Unsere Lösung:</u> Das CoVerified Widget bietet einen effizienten, zuverlässigen Informationskanal von Regierung und Wissenschaftsinstitutionen zur Bevölkerung.
  </p>
  <p>
    <u>Das Ziel:</u> CoVerified auf möglichst vielen Websites zu integrieren, damit so viele Menschen wie möglich die aktuellsten verifizierten Informationen zur Coronakrise erhalten.
  </p>
  <p>
    Das Projekt ist eine Non-Profit-Lösung. Der Code ist Open Source. Die Projektbeschreibung und die Dokumentation beim #WirVsVirus Hackathon finden Sie hier:
    <a href="https://devpost.com/software/1_039_c_staatlichekommunikation_webinfowidget" title="Projektbeschreibung" target="_blank" rel="noopener">
      Devpost
    </a>
  </p>
  <h2>
    Unsere Motivation
  </h2>
  <p>
    Fakten statt Fake News: Mit CoVerified arbeiten wir und Sie proaktiv gegen Falschmeldungen. Es treibt uns an, einen Beitrag zur besseren Krisenkommunikation zu leisten, von dem möglichst viele Menschen profitieren. Denn wir bewältigen die Krise besser mit wissenschaftlich belegten Daten und Expertentipps. Zusammen mit Ihnen möchten wir erreichen, dass die aktuellsten verifizierten Informationen zu Covid-19 auf jeder Website immer nur einen Klick entfernt sind. Wenn alle mitmachen sind alle informiert!
  </p>
  <h2>
    Unsere Vision
  </h2>
  <p>
    Die Idee von CoVerified ist in der Coronakrise geboren, aber Weiterentwicklung und Umsetzung der Idee nicht auf diese beschränkt. Wir wollen CoVerified auch bei weiteren Krisen, wie z.B. Hochwasser, einsetzen. Denn darin liegt ein großer Vorteil von CoVerified:
  </p>
  <p>
    Das Widget lässt sich in Krisensituationen unterschiedlichster Art verwenden. Verified communication &ndash; verifizierte Kommunikation &ndash; ist auch in Zukunft unsere Leitidee in der Krisenbekämpfung. Mit dieser wollen wir Krisensituationen solidarisch und inklusiv bewältigen.
  </p>
  <h2>
    In wie fern verifiziert?
  </h2>
  <p>
    Die Zahlen und Informationen des Widgets zu Covid-19 kommen nicht aus Wirtschaftsunternehmen oder von Medienhäusern. Weder Profitmaximierung noch Verkaufs- und  Klickzahlen sollen die Verlässlichkeit und Richtigkeit von CoVerified beeinträchtigen. Der Unsicherheit und Angst in Krisenzeiten begegnen wir mit einem verlässlichen, stabilen Informationsfluss.
  </p>
</main>


