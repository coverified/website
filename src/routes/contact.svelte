<script>
  import Header from "../components/Header.svelte";
  import Col from 'sveltestrap/src/Col.svelte';
  import Row from 'sveltestrap/src/Row.svelte';
</script>

<style type="text/scss">
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
  
  h2 {
    font-size: 2rem;
    color: var(--color-primary);
    margin-bottom: 2.5rem;
  }

  h3 {
    margin-bottom: .9375rem;
  }

  p {
    margin-bottom: 2.5rem;
  }

  @media (max-width: 768px) {
    header {
        flex-direction: column;
        align-items: center;
        justify-content: flex-start;
        // height: 24vh;
        
        > h1 {
            top: 3px;
        }

        > .wirvsvirus__logo {
            bottom: 1rem;
            right: auto;
            width: 15rem;
        }
    }
  }
</style>

<svelte:head>
	<title>Kontakt</title>
</svelte:head>
<header>
  <h1 class="sr-only">Kontakt</h1>
  <h1>
      Kontakt
  </h1>
  <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
</header>
<Row>
  <Col sm="auto" lg="5">
<h2>
  Ideen? Kooperationen? Fragen?
</h2>

<h3>
  Einfach eine mail schreiben!
</h3>
<p>
  Unser neunköpfiges Team, steht Euch gerne Rede und Antwort! Meldet Euch gerne mit Feedback, Anfragen und Anregungen.
</p>
<p>
  Wir sind erreichbar unter <a href= "mailto:info@coverified.info" title="CoVerified E-Mail">info@coverified.info</a>
</p>
</Col>
</Row>




