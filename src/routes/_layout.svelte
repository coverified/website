<script>
    import Nav from '../components/Nav.svelte';

    export let segment;
</script>

<style>
    main {
        position: relative;
        max-width: 71.25rem;
        background-color: white;
        padding: 2rem 1rem;
        margin: 0 auto;
        box-sizing: border-box;
    }

    header {
        background-color: #E1E3E6;
        position: relative;
    }
</style>

<header>
    <Nav {segment}/>
</header>

<main>
    <slot></slot>
</main>
