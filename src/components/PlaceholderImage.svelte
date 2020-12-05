<script>
  import { onMount } from 'svelte';  

  export let url = '';
  export let additionalClass = '';
  export let placeholder = '';
  export let alt = 'Image';
  export let styling = '';
  export let width;
  export let height;
  
  let image;
  let loaded = false;

  $: {
      if (loaded) {
          image.src = url;
      }
  }

  onMount(() => {    
    image.src = url;
    image.onload = () => {
        loaded = true;
        image.style.cssText = styling;
    };
  });
</script> 

<img src="" alt="{alt}" bind:this={image} style="display: none;" {width} {height} class="{additionalClass}" />

{#if !loaded}
  <img src="{placeholder}" alt="{alt}" class="{additionalClass}"/>
{/if}  