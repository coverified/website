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
      Impressum
  </h1>
  <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
</header>
<Row>
  <Col sm="auto" lg="12">
<p>
  <b>Angaben gemäß § 5 TMG</b>
</p>
<p>
  Julia Diehl, Alessa Fetzer, Johannes Hiry, Steven Killian, Maximilian Mayer, Florian Schlittenbauer, Simon Schweikert, Christina Vollnhals, Paula Weise GbR
</p>
<p>
  Ludwigstraße 187<br />
  c/o Schwarzraum<br />
  63067 Offenbach
</p>
<p>
  Telefon: +49 (0)176 32789572<br />
  E-Mail: <a href= "mailto:info@coverified.info" title="CoVerified E-Mail">info@coverified.info</a>
</p>
<p>
  Verantwortlich für den Inhalt nach § 55 Abs. 2 RStV<br/>
  Christian Gleitze, Verena Hochrein
</p>
<p>
  <b>EU-Streitschlichtung</b>
</p>
<p>
  Die Europäische Kommission stellt eine Plattform zur Online-Streitbeilegung (OS) bereit:<br />
  <a title="EC Europa" href="https://ec.europa.eu/consumers/odr" rel="noopener" target="_blank">https://ec.europa.eu/consumers/odr</a>. Unsere E-Mail-Adresse finden Sie oben im Impressum.
</p>
<p>
  <b>Verbraucherstreitbeilegung Universalschlichtungsstelle</b>
</p>
<p>
  Wir sind nicht bereit oder verpflichtet, an Streitbeilegungsverfahren vor einer<br />
  Verbraucherschlichtungsstelle teilzunehmen.
</p>
<p>
  <b>Haftung für Inhalte</b>
</p>
<p>
  Als Diensteanbieter sind wir gemäß § 7 Abs.1 TMG für eigene Inhalte auf diesen Seiten nach den allgemeinen Gesetzen verantwortlich. Nach §§ 8 bis 10 TMG sind wir als Diensteanbieter jedoch nicht verpflichtet, übermittelte oder gespeicherte fremde Informationen zu überwachen oder nach Umständen zu forschen, die auf eine rechtswidrige Tätigkeit hinweisen. Verpflichtungen zur Entfernung oder Sperrung der Nutzung von Informationen nach den allgemeinen Gesetzen bleiben hiervon unberührt. Eine diesbezügliche Haftung ist jedoch erst ab dem Zeitpunkt der Kenntnis einer konkreten Rechtsverletzung möglich. Bei Bekanntwerden von entsprechenden Rechtsverletzungen werden wir diese Inhalte umgehend entfernen.
<p>
  <b>Haftung für Links</b>
</p>
<p>
  Unser Angebot enthält Links zu externen Websites Dritter, auf deren Inhalte wir keinen Einfluss haben. Deshalb können wir für diese fremden Inhalte auch keine Gewähr übernehmen. Für die Inhalte der verlinkten Seiten ist stets der jeweilige Anbieter oder Betreiber der Seiten verantwortlich. Die verlinkten Seiten wurden zum Zeitpunkt der Verlinkung auf mögliche Rechtsverstöße überprüft. Rechtswidrige Inhalte
  waren zum Zeitpunkt der Verlinkung nicht erkennbar. Eine permanente inhaltliche Kontrolle der verlinkten Seiten ist jedoch ohne konkrete Anhaltspunkte einer Rechtsverletzung nicht zumutbar. Bei Bekanntwerden von Rechtsverletzungen werden wir derartige Links
  umgehend entfernen.
</p>
<p>
  <b>Urheberrecht</b>
</p>
<p>
  Die durch die Seitenbetreiber erstellten Inhalte und Werke auf diesen Seiten unterliegen dem deutschen Urheberrecht. Die Vervielfältigung, Bearbeitung, Verbreitung und jede Art der Verwertung außerhalb der Grenzen des Urheberrechtes bedürfen der schriftlichen Zustimmung des jeweiligen Autors bzw. Erstellers. Downloads und Kopien dieser Seite sind nur für den privaten, nicht kommerziellen Gebrauch gestattet. Soweit die Inhalte auf dieser Seite nicht vom Betreiber erstellt wurden, werden die Urheberrechte Dritter beachtet. Insbesondere werden Inhalte Dritter als solche gekennzeichnet. Sollten Sie trotzdem auf eine Urheberrechtsverletzung aufmerksam werden, bitten wir um einen entsprechenden Hinweis. Bei Bekanntwerden von Rechtsverletzungen werden wir derartige Inhalte umgehend entfernen.
</p>
<p>
  <b>Quelle:</b>
</p>
<p>
  <a title="e-recht24.de" rel="nofollow" target="_blank" href="https://www.e-recht24.de/impressum-generator.html">https://www.e-recht24.de/impressum-generator.html</a>
</p>
</Col>
</Row>















