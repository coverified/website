<script>
  import Header from "../components/Header.svelte";
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

  form {
    font-size: 1.25rem;        
    
    label {
      display: none;
    }

    div {
      margin-bottom: 1.25rem;
    }
    
    input {
      width: 100%;
      height: 4rem;
      padding-left: 1.625rem;
    }

    textarea {
      width: 100%;
      height: 14.75rem;
      padding-left: 1.625rem;
      padding-top: .75rem;
    }
  }

  @media (min-width: 992px) {
    .bg-secondary {
      margin-bottom: 16rem;
    }
  }

  @media (max-width: 992px) {
    form {
      margin-top: 4rem;
    }
  }
</style>

<svelte:head>
  <title>Kontakt</title>
</svelte:head>
<Container>
  <h1 class="text-center mt-80">Wir freuen uns auf Ihre Nachricht</h1>
  <div class="bg-secondary">
    <Row>
      <Col sm="auto" lg="6">
        <p class="text-black">
          Sie haben Interesse an einer Zusammenarbeit oder möchten mehr über
          CoVerified erfahren? Schreiben Sie uns oder rufen Sie uns an.
        </p>
        <p class="text-muted">
          CoVerified – Diehl, Fetzer, Hiry, Kilian, Mayer, Schlittenbauer,
          Schweikert, Vollnhals, Weise GbR
          <br />
          c/o Schwarzraum
          <br />
          Ludwigstr. 187
          <br />
          63067 Offenbach am Main
        </p>
        <Row>
          <Col sm="auto" lg="4" />
          <Col sm="auto" lg="8">
            <p class="mb-0 text-black mt-80">Anpsrechpartnerin</p>
            <p class="h3 my-2 text-black">Alessa Fetzer</p>
            <a
              href="mailto:info@coverified.de"
              class="mb-2 d-block font-weight-light h3">
              info@coverified.de
            </a>
            <a href="+49+17632789572" class="font-weight-light h3">
              +49 176 32789572
            </a>
          </Col>
        </Row>
      </Col>
      <Col sm="12" lg="6">
        <form
          name="contact"
          method="POST"
          data-netlify="true"
          netlify-honeypot="bot-field">
          <p class="d-none">
              <label>Don’t fill this out if you're human: <input name="bot-field" /></label>
          </p>
          <div>
            <label>
              Name<sup>*</sup>
            </label>
            <input type="text" name="name" placeholder="Name*" required/>
          </div>
          <div>
            <label>
              Firma
            </label>
              <input type="firma" name="firma" placeholder="Firma"/>
          </div>
          <div>
            <label>
              Betreff
            </label>
              <input type="text" name="betreff" placeholder="Betreff"/>
          </div>
          <div>
            <label>
              Ihre Nachricht<sup>*</sup>
            </label>
              <textarea name="message" placeholder="Ihre Nachricht*" required/>
          </div>
          <div>
            <button class="btn-primary" type="submit">Absenden</button>
          </div>
        </form>
      </Col>
    </Row>
  </div>
</Container>
