<script>
    import IntersectionObserver from './IntersectionObserver.svelte'    ;
    import Image from './Image.svelte';

    export let src;   
    export let alt;
    export let width;
    export let height;
    
</script>

<IntersectionObserver once={true} let:intersecting={intersecting}>
    {#if intersecting}
        <Image {alt} {src} {width} {height} />
    {/if}
</IntersectionObserver>