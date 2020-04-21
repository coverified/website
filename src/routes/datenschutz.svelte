<script>
  import Header from "../components/Header.svelte";
  import Col from 'sveltestrap/src/Col.svelte';
  import Row from 'sveltestrap/src/Row.svelte';
</script>

<style type="text/scss">
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

  h1 {
    font-size: 2rem;
    position: absolute;
    color: var(--color-white);
    top: 8rem;
    left: 10rem;
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

  @media (max-width: 768px) {
    header {
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
        
      > h1 {
        top: 3.5rem;
        left: unset;
      }

      > .wirvsvirus__logo {
        bottom: 1rem;
        right: auto;
        width: 15rem;
      }
    }
  }

  @media (max-width: 576px) {
 
  }
</style>

<svelte:head>
	<title>Impressum</title>
</svelte:head>
<header>
  <h1 class="sr-only">Impressum</h1>
  <h1>
      Datenschutz
  </h1>
  <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
</header>
<Row>
  <Col sm="auto" lg="12">
<p>
  <b>Anmerkung der Verantwortlichen</b>
</p>
<p>
  Weder bei der Nutzung unseres Widgets, noch bei dem Besuch unseres Internetauftrittes verarbeiten, tracken oder speichern wir personenbezogenen Daten.<br />
  Da unser Netlify-Server allerdings, worauf die Website liegt, im Hintergrund personenbezogene Daten in Form von Server-Logfiles erstellt finden Sie anbei unsere Datenschutzerklärung. <br />
  Wir möchten gerne aber noch einmal darauf hinweisen, dass wir keinerlei Daten erheben, verarbeiten und kommerziell nutzen. Unser Ziel ist es, mit unserem Angebot Informationen bereitzustellen. <br />
  Durch das Nutzen unseres Widgets können Sie auf die Seiten von anderen Anbietern weitergeleitet werden. Sobald Sie sich auf deren Webseiten befinden, gilt deren Datenschutzerklärung. 
</p>
<p>
  <b>Datenschutzerklärung</b>
</p>
<p>
Personenbezogene Daten (nachfolgend zumeist nur „Daten“ genannt) werden von uns nur im Rahmen der Erforderlichkeit sowie zum Zwecke der Bereitstellung eines funktionsfähigen und nutzerfreundlichen Internetauftritts, inklusive seiner Inhalte und der dort angebotenen Leistungen, verarbeitet.
Gemäß Art. 4 Ziffer 1. der Verordnung (EU) 2016/679, also der Datenschutz-Grundverordnung (nachfolgend nur „DSGVO“ genannt), gilt als „Verarbeitung“ jeder mit oder ohne Hilfe automatisierter Verfahren ausgeführter Vorgang oder jede solche Vorgangsreihe im Zusammenhang mit personenbezogenen Daten, wie das Erheben, das Erfassen, die Organisation, das Ordnen, die Speicherung, die Anpassung oder Veränderung, das Auslesen, das Abfragen, die Verwendung, die Offenlegung durch Übermittlung, Verbreitung oder eine andere Form der Bereitstellung, den Abgleich oder die Verknüpfung, die Einschränkung, das Löschen oder die Vernichtung.
Mit der nachfolgenden Datenschutzerklärung informieren wir Sie insbesondere über Art, Umfang, Zweck, Dauer und Rechtsgrundlage der Verarbeitung personenbezogener Daten, soweit wir entweder allein oder gemeinsam mit anderen über die Zwecke und Mittel der Verarbeitung entscheiden. Zudem informieren wir Sie nachfolgend über die von uns zu Optimierungszwecken sowie zur Steigerung der Nutzungsqualität eingesetzten Fremdkomponenten, soweit hierdurch Dritte Daten in wiederum eigener Verantwortung verarbeiten.<br />
Unsere Datenschutzerklärung ist wie folgt gegliedert:<br />
I. Informationen über uns als Verantwortliche<br />
II. Rechte der Nutzer und Betroffenen<br />
III. Informationen zur Datenverarbeitung<br />
</p>
<p>
  <b>I. Informationen über uns als Verantwortliche</b>
</p>
<p>
Verantwortlicher Anbieter dieses Internetauftritts im datenschutzrechtlichen Sinne ist:<br />
Alessa Fetzer, Andrea Nienhaus, Christian Gleitze, Florian Schlittenbauer, Johannes Hiry, Paula Weise, Simon Schweikert, Steven Killian, Verena Hochrein GbR
</p>
<p>
℅ Schwarzraum<br /><br />
Luiwgstraße 187<br /><br />
63071 Offenbach<br /><br />
Telefon: +49 176 32789572<br /><br />
E-Mail: <a href= "mailto:info@coverified.info" title="CoVerified E-Mail">info@coverified.info</a>
</p>
<p>
  Datenschutzbeauftragte/r sind alle oben genannten Gesellschafter der GbR. 
</p>
<p>
  <b>II. Rechte der Nutzer und Betroffenen</b>
</p>
<p>
  Mit Blick auf die nachfolgend noch näher beschriebene Datenverarbeitung haben die Nutzer und Betroffenen das Recht
</p>
<ul>
  <li>
    auf Bestätigung, ob sie betreffende Daten verarbeitet werden, auf Auskunft über die verarbeiteten Daten, auf weitere Informationen über die Datenverarbeitung sowie auf Kopien der Daten (vgl. auch Art. 15 DSGVO);
  </li>
  <li>
    auf Berichtigung oder Vervollständigung unrichtiger bzw. unvollständiger Daten (vgl. auch Art. 16 DSGVO);
  </li>
  <li>
    auf unverzügliche Löschung der sie betreffenden Daten (vgl. auch Art. 17 DSGVO), oder, alternativ, soweit eine weitere Verarbeitung gemäß Art. 17 Abs. 3 DSGVO erforderlich ist, auf Einschränkung der Verarbeitung nach Maßgabe von Art. 18 DSGVO;
  </li>
  <li>
    auf Erhalt der sie betreffenden und von ihnen bereitgestellten Daten und auf Übermittlung dieser Daten an andere Anbieter/Verantwortliche (vgl. auch Art. 20 DSGVO);
  </li>
  <li>
    auf Beschwerde gegenüber der Aufsichtsbehörde, sofern sie der Ansicht sind, dass die sie betreffenden Daten durch den Anbieter unter Verstoß gegen datenschutzrechtliche Bestimmungen verarbeitet werden (vgl. auch Art. 77 DSGVO).
  </li>
</ul>
<p>
  Darüber hinaus ist der Anbieter dazu verpflichtet, alle Empfänger, denen gegenüber Daten durch den Anbieter offengelegt worden sind, über jedwede Berichtigung oder Löschung von Daten oder die Einschränkung der Verarbeitung, die aufgrund der Artikel 16, 17 Abs. 1, 18 DSGVO erfolgt, zu unterrichten. Diese Verpflichtung besteht jedoch nicht, soweit diese Mitteilung unmöglich oder mit einem unverhältnismäßigen Aufwand verbunden ist. Unbeschadet dessen hat der Nutzer ein Recht auf Auskunft über diese Empfänger.
</p>
<p>
  <b>
    Ebenfalls haben die Nutzer und Betroffenen nach Art. 21 DSGVO das Recht auf Widerspruch gegen die künftige Verarbeitung der sie betreffenden Daten, sofern die Daten durch den Anbieter nach Maßgabe von Art. 6 Abs. 1 lit. f) DSGVO verarbeitet werden. Insbesondere ist ein Widerspruch gegen die Datenverarbeitung zum Zwecke der Direktwerbung statthaft.
  </b>
</p>
<p>
  <b>
    III. Informationen zur Datenverarbeitung
  </b>
</p>
<p>
  Ihre bei Nutzung unseres Internetauftritts verarbeiteten Daten werden gelöscht oder gesperrt, sobald der Zweck der Speicherung entfällt, der Löschung der Daten keine gesetzlichen Aufbewahrungspflichten entgegenstehen und nachfolgend keine anderslautenden Angaben zu einzelnen Verarbeitungsverfahren gemacht werden.
</p>
<p>
  Quelle: <a title="Recht ratgeber" rel="nofollow" target="_blank" href="https://www.ratgeberrecht.eu/leistungen/muster-datenschutzerklaerung.html#Generator">https://www.ratgeberrecht.eu/leistungen/muster-datenschutzerklaerung.html#Generator</a> 
</p>
</Col>
</Row>
 