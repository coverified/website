<script>
    import Nav from '../components/Nav.svelte';
    import Footer from '../components/Footer.svelte';

    export let segment;
</script>

<style type="text/scss">
    main {
        position: relative;
        max-width: 71.25rem;
        background-color: white;
        padding: 2rem 1rem;
        margin: 0 auto;
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

<Footer/>
