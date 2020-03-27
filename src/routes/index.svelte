<script>
  import Button from "../components/Button.svelte";
  import Article from "../components/Article.svelte";
</script>

<style type="text/scss">
  h1,
  p {
    margin: 0 auto;
  }

  h1 {
    font-size: 2.8rem;
    font-weight: 700;
    margin: 0 0 0.5rem 0;
  }

  h2 {
    font-size: 1.75rem;
    font-weight: 700;
    margin: 0 0 1rem 0;
  }

  img {
    width: 100%;
    margin: 0 0 1em 0;
  }

  @media (min-width: 480px) {
    h1 {
      font-size: 4em;
    }
  }
  .news {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(345px, 1fr));
    justify-content: space-between;
    background-color: #fff;
    position: relative;
  }
</style>

<svelte:head>
  <title>CoVerified</title>
  <meta name="description" content="CoVerified" />
</svelte:head>

<h1 class="sr-only">CoVerified</h1>
<img
  src="cover.jpg"
  alt="CoVerified"
  width="2560"
  height="1440"
  loading="lazy" />

<h2>Current News</h2>
<div class="news">
  <Article />
  <Article />
  <Article />
  <Article />
  <Article />
  <Article />
</div>
