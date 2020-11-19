<script>
  import Header from "../components/Header.svelte";
  import Col from 'sveltestrap/src/Col.svelte';
  import Row from 'sveltestrap/src/Row.svelte';
  import Container from "sveltestrap/src/Container.svelte";
</script>

<style type="text/scss">
  .bg-secondary {
    position: relative;
    background-color: var(--color-lighter-grey) !important;
    z-index: 100;
    margin-top: 3.75rem;
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

  .mt-80 {
    margin-top: 5rem;
  }

  @media (min-width: 992px) {
    .bg-secondary {
      margin-bottom: 16rem;
    }
  }
</style>

<svelte:head>
	<title>Kontakt</title>
</svelte:head>
<Container>
  <h1 class="text-center mt-80">
    Wir freuen uns auf Ihre Nachricht
  </h1>
  <div class="bg-secondary">
  <Row>
    <Col sm="auto" lg="6">
      <p class="text-black">
        Sie haben Interesse an einer Zusammenarbeit oder möchten mehr über CoVerified erfahren? Schreiben Sie uns oder rufen Sie uns an.
      </p>
      <p class="text-muted">
        CoVerified – Diehl, Fetzer, Hiry, Kilian, Mayer,
        Schlittenbauer, Schweikert, Vollnhals, Weise GbR<br />
        c/o Schwarzraum<br />
        Ludwigstr. 187<br />
        63067 Offenbach am Main
      </p>
      <Row>
        <Col sm="auto" lg="4">
        </Col>
        <Col sm="auto" lg="8">
          <p class="mb-0 text-black mt-80">
            Anpsrechpartnerin
          </p>
          <p class="h3 my-2 text-black"> 
            Alessa Fetzer
          </p>
          <a href="mailto:info@coverified.de" class="mb-2 d-block font-weight-light h3">
            info@coverified.de
          </a>
          <a href="+49+17632789572" class="font-weight-light h3">+49 176 32789572</a>
        </Col>
      </Row>
    </Col>
    <Col sm="auto" lg="6">

    </Col>
  </Row>
  </div>
</Container>