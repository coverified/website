<script>
    import Button from '../components/Button.svelte';
</script>

<style type="text/scss">
    :root {
        overflow-x: hidden;
    }

    h1 {
        font-size: 2.25rem;
        font-weight: 700;
        color: var(--color-white);
        line-height: 48px;
        max-width: 645px;
    }

    h2 {
        font-size: 2.25rem;
        font-weight: 700;
        margin: 0 0 1rem 0;
    }

    .container {
        position: relative;
        height: auto;
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
            position: absolute;
            right: 0;
            bottom: 1rem;
            display: flex;
            align-items: center;
        }

        .coverified__informationgraphic {
            position: relative;
            width: 50%;
            padding-top: 2rem;
            padding-bottom: .5rem;
        }

        .wirvsvirus__logo {
            width: 26rem;
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
            justify-content: center;
            margin-bottom: 8.5rem;

            > div:not(.info__box) {
                right: unset;
                bottom: 4.5rem;
            }

            > .info__box {
                right: unset;
            }

            .wirvsvirus__logo {
                left: 0;
                margin: 0 auto;
                top: 56%;
                width: 22rem;
            }

            .coverified__informationgraphic {
                width: 58%;
                padding-bottom: 18.5rem;
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

            .coverified__informationgraphic {
                width: 69%;
                padding-bottom: 21.5rem;
            }

            .wirvsvirus__logo {
                top: 48%;
            }
        }
    }


    @media (max-width: 576px) {
        h1 {
            font-size: 1.575rem;
            line-height: 33.6px;
        }

        .container {
            > div:not(.info__box) {
                bottom: 6.25rem;
                padding-left: .5rem;
                padding-right: .5rem;
            }

            > .info__box {
                right: 0;
            }

            .coverified__informationgraphic {
                width: 90%;
            }

            .wirvsvirus__logo {
                width: 16rem;
                top: 47%;
                right: 0;
                left: 0;
                margin: 0 auto;
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
    <img class="coverified__informationgraphic" src="coverified-information-graphic.svg"
         alt="Coverified Information graphic">
    <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
    <div>
        <h1>
            Verifizierte Informationen zu Covid19. <br>
            Überall im Netz, auf einen Klick verfügbar.
        </h1>
    </div>
    <div class="info__box">
        <coverified-cases></coverified-cases>
    </div>
</div>

<h2>Aktuelle Neuigkeiten</h2>
<div class="news">
    <coverified-articles></coverified-articles>
    <p>
        Wir arbeiten gerade an unserer Website, daher ist noch nicht alles perfekt, aber zumindest funktionstüchtig!
    </p>
</div>
