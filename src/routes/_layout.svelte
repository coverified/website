<script>
    import Nav from '../components/Nav.svelte';

    export let segment;
</script>

<style>
    main {
        position: relative;
        max-width: 71.25rem;
        background-color: white;
        padding: 2rem;
        margin: 0 auto;
        box-sizing: border-box;
    }

    header {
        background-color: #E1E3E6;
        position: relative;
        margin-bottom: 3px;
    }

    header::after {
        content: '';
        display: block;
        width: 100%;
        height: 3px;
        position: absolute;
        left: 0;
        top: 0;
        background: linear-gradient(to right, #000000 33%, #de0000 33.001%, #de0000 66%, #ffcf00 66.001%);
    }
</style>

<header>
    <Nav {segment}/>
</header>

<main>
    <slot></slot>
</main>
