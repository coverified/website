<script>  
  import Col from "sveltestrap/src/Col.svelte";
  import Row from "sveltestrap/src/Row.svelte";
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

  .btn-primary {
    --btn-primary-bg-color: var(--color-primary);
    --btn-primary-text-color: var(--color-white);
    --btn-primary-border-color: var(--color-primary);
    --btn-primary-border-width: 1px;
    --btn-primary-border-style: solid;
    --btn-primary-border-radius: 2rem;
    --btn-padding: 0.75rem 4.6875rem;
    --btn-font-weight: 300;
    --text-decoration: none;
    
    background-color: var(--btn-primary-bg-color);
    color: var(--btn-primary-text-color) !important;
    padding: var(--btn-padding);
    border-color: var(--btn-primary-border-color);
    border-width: var(--btn-primary-border-width);
    border-style: var(--btn-primary-border-style);
    border-radius: var(--btn-primary-border-radius);
    font-weight: var(--btn-font-weight);
    text-decoration: var(--text-decoration);
  }

  .mt-80 {
    margin-top: 5rem;
  }

  .mb-lg-80 {
    margin-bottom: 5rem;
  }

  @media (min-width: 992px) {
    .bg-secondary {
      margin-bottom: 16rem;
    }
  }

  @media (max-width: 992px) {
    .mb-lg-80 {
      margin-bottom: 2rem;
    }
  }
</style>

<svelte:head>
  <title>CoVerified kennenlernen?</title>
  <meta name="description" content="CoVerified – Redefining Communication. Gemeinsam
gestalten wir Digitalisierung. Jetzt Kontakt aufnehmen." />
</svelte:head>
<Container>
  <h1 class="text-center mt-80">Wir freuen uns auf Ihre Nachricht</h1>
  <div class="bg-secondary">
    <Row class="align-items-center">
      <Col sm="auto" lg="6">
        <p class="text-black">
          Sie haben Interesse an einer Zusammenarbeit oder möchten mehr über
          CoVerified erfahren? Schreiben Sie uns oder rufen Sie uns an.
        </p>
        <p class="text-muted mb-lg-80">
          CoVerified – Diehl, Fetzer, Hiry, Kilian, Mayer, Schlittenbauer,
          Schweikert, Vollnhals, Weise GbR
          <br />
          c/o Schwarzraum
          <br />
          Ludwigstr. 187
          <br />
          63067 Offenbach am Main
        </p>      
      </Col>
      <Col sm="auto" lg="6">
        <Row class="d-flex align-items-center justify-content-center">
          <Col xs="8" sm="5" lg="4">
            <img src="alessa_fetzer.png" alt="Alessa Fetzer" class="mb-3 mb-md-0" width="625" height="625">
          </Col>
          <Col sm="auto" lg="8">
            <div class="mx-auto d-flex flex-column">
              <p class="mb-0 text-black">Ansprechpartnerin</p>
              <p class="h3 my-2 text-black">Alessa Fetzer</p>
              <a
                href="mailto:info@coverified.info?subject=Interesse%20an%20zusammenarbeit"
                class="mb-2 d-block font-weight-light h3">
                info@coverified.info
              </a>
              <a href="tel:+4917632789572" class="font-weight-light h3 mb-0">
                +49 176 32789572
              </a>
            </div>
          </Col>
        </Row>
      </Col>
    </Row>
  </div>
</Container>
