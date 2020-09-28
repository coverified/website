<script>
  import Nav from "../components/Nav.svelte";
  import Footer from "../components/Footer.svelte";
  export let segment;
</script>

<style type="text/scss">
  :global(:root) {
    --color-primary: #3a57ff;
    --color-light-grey: #ececec;
    --color-dark-grey: #767676;
    --color-lighter-grey: #f6f6f6;
    --color-anthracite: #1d1d1d;
    --color-white: #fff;
    --body-color: #132633;
    --color-border: #ececec;
    --color-green: #49fea4;
    overflow-x: hidden;
  }

  :global(body) {
    font-size: 1.5625rem;
    line-height: 1.875rem;
    color: (--body-color);
    font-family: 'Barlow', sans-serif;
  }

  :global(h2) {
    font-size: 2rem;
    font-weight: 800;
    margin-top: 3rem;
    margin-bottom: 1.5rem;
  }

  :global(p) {
    font-family: 'Barlow-light', sans-serif;
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
