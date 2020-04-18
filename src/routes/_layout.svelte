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
    --color-anthracite: #1d1d1d;
    --color-white: #fff;
    --color-border: #ececec;
    --color-green: #3fb63f;
  }

  :global(h2) {
    font-size: 2rem;
    font-weight: 800;
    margin-top: 3rem;
    margin-bottom: 1.5rem;
  }

  :global(a) {
    color: #333;

    &:hover {
      color: #333;
    }
  }

  :global(main a) { 
    font-weight: 700;
    color: var(--color-primary);

    &:hover {
      text-decoration: none;
      color: var(--color-anthracite);
    }
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

  @media (max-width: 1200px) {
    main {
      max-width: 60rem;
    }
  }

  @media (max-width: 992px) {
    main {
      max-width: 45rem;
    }
  }


  @media (max-width: 768px) {
    main {
      max-width: 33.75rem;
    }
  }

  @media (max-width: 576px) {
    main {
      max-width: 22.5rem;
    }
  }
</style>

<header>
  <Nav {segment} />
</header>

<main>
  <slot />
</main>

<Footer />
