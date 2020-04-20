<script>
    import Button from '../components/Button.svelte';
</script>

<style type="text/scss">
    :root {
        overflow-x: hidden;
    }
    h1 {
        font-size: 2rem;
        font-weight: 700;
        color: var(--color-white);
        line-height: 48px;
        max-width: 645px;
    }
    h2 {
        font-weight: 700;
        margin: 0 0 3.25rem 0;
        color: var(--color-primary);
    }
    .container {
        position: relative;
        height: 14.6875rem;
        margin-bottom: 6.5em;
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
        > div:not(.info__box) {
            position: relative;
            display: flex;
            align-items: center;
            top: 42%;

            h1 {
                margin: 0 auto;
            }
        }

        .coverified__informationgraphic {
            max-width: 24rem;
            position: absolute;
            top: 1.5rem;
        }

        .wirvsvirus__logo {
            width: 20rem;
            height: auto;
            position: absolute;
            right: 0;
            top: 10%;
        }
        .info__box {
            right: 0;
            bottom: 0;
            transform: translateY(50%);
            background-color: var(--color-white);
            border: 2px solid var(--color-light-grey);
            box-shadow: 0 1px 6px -3px rgba(0, 0, 0, 0.11);
            display: block;
            position: absolute;
            border-radius: .33rem;
            padding: 1rem 1.75rem;
        }
    }

    .news {
        background-color: #fff;
        position: relative;
    }

    coverified-articles {
        --open-padding: 1rem;
    }

    @media (max-width: 992px) {

        h1 {
            font-size: 2rem;
        }

        
        .container {
            display: flex;
            height: 25rem;
            justify-content: center;
            margin-bottom: 8.5rem;

            > div:not(.info__box) {
                right: unset;
                bottom: 4.5rem;
                top: unset;
            }

            > .info__box {
                right: unset;
            }

            .wirvsvirus__logo {
                left: 0;
                margin: 0 auto;
                top: 5px;
                width: 20rem;
            }

            .coverified__informationgraphic {
                top: 7rem;
            }
        }
    }
    @media (max-width: 768px) {
        h1 {
            font-size: 1.8rem;
        }
        .container {
            > div:not(.info__box) {
                bottom: 5rem;
            }
            
        }
    }
    @media (max-width: 576px) {
        h1 {
            font-size: 1.575rem;
            line-height: 33.6px;
        }
        h2 {
            font-size: 1.575rem;
        }
        .container {

            > .info__box {
                right: 0;
            }

            .wirvsvirus__logo {
                width: 16rem;
            }

            .coverified__informationgraphic {
                max-width: 22rem;
                top: 5.75rem;
            }
        }
    }
</style>

<svelte:head>
    <title>CoVerified</title>
    <meta name="description" content="CoVerified"/>
</svelte:head>

<h1 class="sr-only">CoVerified</h1>
<div class="container">
    <img class="coverified__informationgraphic" src="news-header.svg"
         alt="Coverified Information graphic"> 
    <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
    <div class="info__box">
        <coverified-cases></coverified-cases>
    </div>
</div>

<h2>Wir bündeln Informationen von <br class="d-none d-lg-block"/>verifizierten Quellen an einem Ort.</h2>
<h3>Aktuelle News</h3>
<div class="news">
    <coverified-articles></coverified-articles>
</div>