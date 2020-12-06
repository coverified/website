<script>
  import Nav from "../components/Nav.svelte";
  import Footer from "../components/Footer.svelte";
  export let segment;
</script>

<style type="text/scss">
    @font-face {
    font-family: 'Barlow';
    font-style: normal;
    font-weight: 300;
    font-display: swap;
    src: url('/fonts/Barlow/Barlow-Light.ttf') format('truetype');
  }

  @font-face {
    font-family: 'Barlow';
    font-style: normal;
    font-weight: 400;
    font-display: swap;
    src: url('/fonts/Barlow/Barlow-Regular.ttf') format('truetype');
  }

  @font-face {
    font-family: 'Barlow';
    font-style: normal;
    font-weight: 500;
    font-display: swap;
    src: url('/fonts/Barlow/Barlow-Medium.ttf') format('truetype');    
  }

  @font-face {
    font-family: 'Barlow';
    font-style: normal;
    font-weight: 600;
    font-display: swap;
    src: url('/fonts/Barlow/Barlow-SemiBold.ttf') format('truetype');    
  }

  @font-face {
    font-family: 'Barlow';
    font-style: normal;
    font-weight: 700;
    font-display: swap;
    src: url('/fonts/Barlow/Barlow-Bold.ttf') format('truetype');
  }
  @font-face {
    font-family: 'Barlow Condensed';
    font-style: normal;
    font-weight: 500;
    font-display: swap;
    src: url('/fonts/BarlowCondensed/BarlowCondensed-Medium.ttf') format('truetype');    
  }
  :global(:root) {
    --color-primary: #3a57ff;
    --color-wika: #003366;
    --color-light-grey: #ececec;
    --color-dark-grey: #767676;
    --color-lighter-grey: #f7f8fc;
    --color-light-grey: #f6f6f6;
    --color-anthracite: #1d1d1d;
    --color-black: #000;
    --color-white: #fff;
    --body-color: #132633;
    --color-border: #ececec;
    --color-green: #49fea4;
    --color-brigt-green: #32f99a;
    overflow-x: hidden;
  }

  :global(body) {
    font-size: 1.25rem;
    line-height: 1.875rem;
    color: var(--body-color);
    font-family: 'Barlow', sans-serif;
    padding-top: 4.89375rem;
  }

  :global(h1,
    .h1) {
      font-size: 2.5rem;
      font-weight: 400;
      color: var(--color-primary);
      margin-bottom: 2.625rem;        
    }

  :global(h2,
  .h2) {
    font-size: 2.25rem;
    color: var(--color-anthracite);
    font-weight: 600;
    margin-top: 7.75rem;
    margin-bottom: 1.6875rem;
  }

  :global(h3,
  .h3) {
    font-size: 1.875rem;
    margin-bottom: 2.75rem;
    color: var(--color-primary);
    
    > span {
        display: block;
        font-size: 1.5625rem;
        font-weight: 500;
        margin-right: auto;
    }
  }

  :global(.text-black) {
    color: var(--color-black);
    font-weight: 600;
  }

  :global(span.green) {
    position: relative;        
    background: linear-gradient(#fff 50%, var(--color-green));                
  }

  :global(span.green--light-grey) {
    position: relative;        
    background: linear-gradient(var(--color-lighter-grey) 50%, var(--color-green));                
  }

  :global(.mb-120) {
    margin-bottom: 7.5rem;
  }

  :global(p) {
    font-weight: 300;
  }

  :global(b,strong) {
    font-weight: bold;
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
</style>

<header>
  <Nav {segment} />
</header>

<main>
  <slot />
</main>

<Footer />
