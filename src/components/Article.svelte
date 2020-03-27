<script>
  import Button from "../components/Button.svelte";
</script>

<style type="text/scss">
  article {
    color: var(--color-anthracite);
    padding: 1rem;
    margin: 0;
    border: 1px solid var(--color-light-grey);
    border-radius: 5px;
    box-shadow: 0 1px 6px -3px rgba(var(--color-light-grey), 0.2);
    > a {
      > h2 {
        font-weight: 700;
      }
    }
  }
</style>

<article>
  <a href=".">
    <h2>Headline</h2>
  </a>
  <p>
    An dieser Stelle dokumentieren wir die bestätigte Anzahl aller Personen, bei
    denen seit Beginn der Epidemie in Deutschland eine Infektion mit dem
    neuartigen Coronavirus nachgewiesen wurde.
  </p>
  <button>Weiterlesen</button>
</article>
