<script>
  import Nav from "../components/Nav.svelte";
  import Footer from "../components/Footer.svelte";

  export let segment;
</script>

<style type="text/scss">
  :global(:root) {
    --color-primary: #3753ff;
    --color-light-grey: #ececec;
    --color-dark-grey: #767676;
    --color-anthracite: #1c1c1c;
    --color-white: #fff;
    --color-border: #ececec;
    --color-green: #3fb63f;
  }
  main {
    position: relative;
    max-width: 71.25rem;
    background-color: white;
    margin: 0 auto;
  }

  header {
    background-color: white;
    border-bottom: 2px solid #e1e3e6;
    position: relative;
  }
</style>

<header>
  <Nav {segment} />
</header>

<main>
  <slot />
</main>

<Footer />
