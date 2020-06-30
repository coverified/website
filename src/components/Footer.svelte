<script>
    import Col from 'sveltestrap/src/Col.svelte';
    import Row from 'sveltestrap/src/Row.svelte';  
</script>

<style type="text/scss">
    footer {
        height: auto;
        max-width: 71.25rem;
        position: relative;
        margin: 7rem auto .5rem auto;
        padding-right: 15px;
        padding-left: 15px;

        &:before {
            content: "";
            position: absolute;
            display: block;
            width: 100vw;
            height: 100%;
            box-shadow: 0 4px 3px rgba(0, 0, 0, 0.2);
            left: 50%;
            right: 0;
            bottom: 0;
            top: 0;
            transform: translateX(-50%);
            z-index: -1;
        }

        h3 {
            position: relative;
            font-size: 1rem;
            color: var(--color-dark-grey);
            font-weight: 400;
            padding-top: 3rem;
            margin-bottom: 2.5rem;
        }
    }

    .bundesregierung-logo {
        width: 19rem;
    }

    .meta-bar {
        max-width: 71.25rem;
        margin: 0 auto;
        padding: 1rem;
        display: flex;
        flex-direction: row;
        justify-content: space-between;

        > a {
            margin-left: 1rem;
        }
    }

    @media (max-width: 1200px) {
        footer {
            max-width: 60rem;
        }
    }

    @media (max-width: 992px) {
        footer {
            max-width: 45rem;
        }
    }


    @media (max-width: 768px) {
        footer {
            max-width: 33.75rem;
        }
    }

    @media (max-width: 576px) {
        footer {
            max-width: 22.5rem;
            padding: 0 2rem;
        }

        .bundesregierung-logo {
            width: 16rem;
        }

        div {
            > p {
                margin-top: .5rem;
                margin-bottom: .5rem;

                &:last-of-type {
                    margin-bottom: 3rem;
                }
            }
        }
        .meta-bar {
            > a:not(:last-child) {
                font-size: .85rem;
            }
        }
    }

</style>

<footer>
    <Row>
        <Col sm="auto" lg="4" class="mb-md-4">
            <h3>
                Gefördert von
            </h3>
            <img class="bundesregierung-logo" src="bmbf-logo.svg" alt="Bundesministerium für Bildung und Forschung">
        </Col>
        <Col sm="auto" lg="4" class="mb-md-4">
            <h3>
                Unterstützt von 
            </h3>
            <img class="bundesregierung-logo" src="bundesregierung-logo.svg" alt="Die Bundesregierung">
        </Col>
        <Col sm="auto" lg="4" class="mb-md-4">
        <h3>
            Unsere Datenbank bündelt folgende Quellen:
        </h3>
        <div>
            <p>
                Bundesministerium für Gesundheit
            </p>
            <p>
                Bundesregierung Deutschland
            </p>
            <p>
                Robert Koch Institut
            </p>
            <p>
                Charité Universitätsmedizin Berlin
            </p>
            <p>
                Johns Hopkins University
            </p>
        </div>
        </Col>
    </Row>
</footer>

<p class="meta-bar">
    <span class="copyright">
        &copy; {new Date().getFullYear()} CoVerified
    </span>
    <a rel="prefetch"
        href="impressum">
        Impressum
    </a>

    <a rel="prefetch"
        href="datenschutz">
        Datenschutz
    </a>
    <a href="https://github.com/coverified/" rel="noopener" target="_blank">
        <svg class="icon icon-github">
            <use xlink:href="#icon-github"/>
        </svg>
    </a>
</p>
