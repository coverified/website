<script>
  import { onMount } from "svelte";

  let el = null;
  let visible = false;
  let hasBeenVisible = false;
  let observer = null;

  onMount(() => {
    observer = new IntersectionObserver(
      entries => {
        visible = entries[0].isIntersecting;
        hasBeenVisible = hasBeenVisible || visible;
      },
      { rootMargin: "0px 0px 200px 0px" }
    );
    observer.observe(el);

    return () => {
      if (!hasBeenVisible) {
        observer.unobserve(el);
      }
    };
  });

  $: if (hasBeenVisible) {
    observer.unobserve(el);
  }
</script>

<div bind:this={el} style="position: relative;">
  <slot {visible} {hasBeenVisible} />
</div>