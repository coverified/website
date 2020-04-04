<script>
    export let pageName = 'CoVerified';
</script>

<style type="text/scss">
    header {
        background-color: var(--color-primary);
        height: 29vh;
        position: relative;
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
        font-size: 3.375rem;
        position: relative;
        color: var(--color-white);
        top: 38%;
        left: 1.8%;
        margin-bottom: 1.56rem;
    }

    small {
        font-size: 1rem;
        position: absolute;
        top: 3.125rem;
        right: 15%;
        color: var(--color-white);
    }

    .wirvsvirus__logo {
        position: absolute;
        width: 22rem;
        bottom: 11%;
        right: 0;
    }

    @media (max-width: 768px) {
        header {
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
            
            > h1 {
                top: 0;
            }

            > small {
                top: 6.125rem;
                right: auto;
            }

            > .wirvsvirus__logo {
                bottom: 0;
                top: 55%;
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
    <small>
        Ein Hackathon-Projekt
    </small>
    <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">

</header>





