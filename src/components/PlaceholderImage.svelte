<script>
  import { onMount } from 'svelte';  

  export let url = '';
  export let additionalClass = '';
  export let placeholder = '';
  export let alt = 'image';
  export let imageWidth = '100%';
  export let imageHeight = '100%';
  export let styling = '';
  
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
        image.style.cssText = `width: ${imageWidth}; height ${imageHeight};` + styling;
    };
  });
</script> 

<img src="" alt="{alt}" bind:this={image} style="display: none;" class="{additionalClass}" />
{#if !loaded}
  <img src="{placeholder}" alt="{alt}" class="{additionalClass}"/>
{/if}  