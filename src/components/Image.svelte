<script>
  import { onMount } from 'svelte';
  
  export let src;
  export let alt;

  let loaded = false
  let thisImage

  onMount(() => {
    thisImage.onload = () => {
      loaded = true
    }
  });
</script>

<style type="text/scss">
  img {    
    opacity: 0;
    transition: opacity 1200ms ease-out;

    &.loaded {
      opacity: 1;
    }
  }
</style>

<img {src} {alt} class:loaded bind:this={thisImage} />