<script>
    export let pageName = 'CoVerified';
</script>

<style type="text/scss">
    header {
        background-color: var(--color-primary);
        height: 18vh;
        position: relative;
        justify-content: center;
        display: flex;
        margin-bottom: 3rem;
        
        &:before {
            content: "";
            position: absolute;
            background: var(--color-primary);
            display: block;
            width: 100vw;
            height: 100%;
            left: 50%;
            right: 0;
            bottom: 0;
            top: 0;
            transform: translateX(-50%);
            }
    }

    h1 {
        font-size: 2rem;
        position: relative;
        color: var(--color-white);
        top: 68%;
        left: 1.8%;
    }

    .wirvsvirus__logo {
        position: absolute;
        width: 20rem;
        bottom: 37%;
        right: 1.125rem;
    }

    @media (max-width: 768px) {
        header {
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
            
            > h1 {
                top: 0;
            }

            > .wirvsvirus__logo {
                bottom: 1rem;
                right: auto;
                width: 20rem;
            }
        }
    }

</style>

<header>
    <h1 class="sr-only">{pageName}</h1>
    <h1>
        {pageName}
    </h1>
    <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
</header>





