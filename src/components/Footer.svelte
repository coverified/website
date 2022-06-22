<script>
    import Icon from "./Icon.svelte";
    import Col from 'sveltestrap/src/Col.svelte';
    import Row from 'sveltestrap/src/Row.svelte';
</script>

<style type="text/scss">
    footer {
        height: auto;
        max-width: 71.25rem;
        position: relative;
        margin: 7.5rem auto .5rem auto;
        padding-right: 15px;
        padding-left: 15px;
        font-family: 'Barlow Condensed', sans-serif;
        font-weight: 300;
        font-size: 1.25rem;

        &:before {
            content: "";
            position: absolute;
            display: block;
            background-color: var(--color-light-grey);
            width: 100vw;
            height: 100%;
            left: 50%;
            right: 0;
            bottom: 0;
            top: 0;
            transform: translateX(-50%);
            z-index: -1;
        }
    }

    a {
        font-weight: 300;
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

        div {
            margin-top: 3rem;
        }
    }
</style>

<footer>
    <Row class="pt-5 pb-4">
        <Col sm="12" md="8" class="d-flex flex-row align-items-end mb-5 mb-lg-0">
            <a rel="noopener"
               class="mt-3 mr-3"
               target="_blank"
               href="https://www.linkedin.com/company/coverified-startup/"
            >
                <Icon icon="linkedin" />
                <span class="sr-only">CoVerified auf LinkedIn</span>
            </a>
            <a rel="noopener"
               class="mt-3 mr-3"
               target="_blank"
               href="https://mobile.twitter.com/CoVeri_fied"
            >
                <Icon icon="twitter" />
                <span class="sr-only">CoVerified auf Twitter</span>
            </a>
            <a rel="noopener"
               class="mt-3 mr-3"
               target="_blank"
               href="https://github.com/coverified"
            >
                <Icon icon="github" />
                <span class="sr-only">CoVerified auf GitHub</span>
            </a>
            <a rel="noopener"
               class="mt-3 mr-3"
               target="_blank"
               href="mailto:info@coverified.info"
            >
                <Icon icon="mail" />
                <span class="sr-only">Mail an CoVerified</span>
            </a>
        </Col>
        <Col sm="12" md="4" class="d-flex flex-column align-items-end">
            <a rel="prefetch"
                href="impressum">
                Impressum
            </a>

            <a rel="prefetch"
                href="datenschutz">
                Datenschutz
            </a>
            <span class="copyright">
                &copy; {new Date().getFullYear()} CoVerified
            </span>
        </Col>
    </Row>
</footer>
