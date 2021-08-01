<script>
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

    img {
        height: auto;
    }

    div {
        display: flex;
        flex-direction: column;        
        align-items: flex-end;
        margin-left: auto;
        width:fit-content; 

        a {
            font-weight: 300;
        }
    
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

        div {
            margin-top: 3rem;
        }
    }
</style>

<footer>
    <p class="pt-3">Unterstützt durch:</p>
    <Row>        
        <Col sm="auto" lg="4" class="mb-md-4">
            <img loading="lazy" src="logo-accelerator.png" alt="Saarland Accelerator" width="261" height="202" class="pt-3">
        </Col>
        <Col sm="auto" lg="4" class="mb-md-4">
            <img loading="lazy" src="logo-kwt.png" alt="KWT" width="290" height="207" class="pt-3">
        </Col>
        <Col sm="auto" lg="4" class="mb-md-4 pt-0">
        <div>
            <a rel="prefetch"
                href="impressum">
                Impressum
            </a>

            <a rel="prefetch"
                href="datenschutz">
                Datenschutz
            </a>
            <a rel="noopener"
                target="_blank"
                href="https://github.com/coverified"
            >
                GitHub
            </a>
            <span class="copyright">
                &copy; {new Date().getFullYear()} CoVerified
            </span>
        </div>
        </Col>
    </Row>
</footer>
