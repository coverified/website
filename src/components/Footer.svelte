<script>
</script>

<style type="text/scss">
    footer {
        height: auto;
        max-width: 71.25rem;
        position: relative;
        margin: 7rem auto 0 auto;

        &:before {
            content: "";
            position: absolute;
            background: var(--color-light-grey);
            display: block;
            width: 100vw;
            height: 100%;
            left: 50%;
            right: 0;
            bottom: 0;
            top: 0;
            transform: translateX(-50%);
        }


        > h3 {
            position: relative;
            font-size: 1.625rem;
            color: var(--color-anthracite);
            font-weight: 700;
            padding-top: 3rem;
            margin-bottom: 1.5rem;
        }

        > div {
            display: flex;
            flex-direction: column;
            justify-content: center;
            padding-bottom: 2rem;

            > p {
                position: relative;
            }
        }
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
    }

</style>

<footer>
    <h3>
        Quellen
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
</footer>

<p class="meta-bar">
    <span class="copyright">
        &copy; {new Date().getFullYear()} CoVerified
    </span>
    <a href="https://github.com/coverified/" rel="noopener" target="_blank">
        <svg class="icon icon-github">
            <use xlink:href="#icon-github"/>
        </svg>
    </a>
</p>
