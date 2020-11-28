<script>
    import Col from 'sveltestrap/src/Col.svelte';
    import Row from 'sveltestrap/src/Row.svelte';  
</script>

<style type="text/scss">
    footer {
        height: auto;
        max-width: 71.25rem;
        position: relative;
        margin: 1.875rem auto .5rem auto;
        padding-right: 15px;
        padding-left: 15px;        
        font-family: 'Barlow Condensed', sans-serif;
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

    .bundesregierung-logo {
        width: 12rem;
    }

    div {
        display: flex;
        flex-direction: column;        
        align-items: flex-end;
        padding-top: 3rem;
        margin-left: auto;
        width:fit-content; 
    
        > span {
            margin-top: 2.375rem;
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
    }
</style>

<footer>
    <Row>
        <Col sm="auto" lg="3" class="mb-md-4">
            <img class="bundesregierung-logo pt-5" src="bmbf-logo.svg" alt="Bundesministerium für Bildung und Forschung">
        </Col>
        <Col sm="auto" lg="3" class="mb-md-4">
            <img class="bundesregierung-logo pt-5" src="unterstuetzt-von-bundesregierung.svg" alt="Die Bundesregierung">
        </Col>
        <Col sm="auto" lg="3" class="mb-md-4">
            <img class="bundesregierung-logo pt-5" src="wirvsvirus-logo.png" alt="Wir vs Virus Hackathon">
        </Col>
        <Col sm="auto" lg="3" class="mb-md-4">
        <div>
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
        </div>
        </Col>
    </Row>
</footer>
