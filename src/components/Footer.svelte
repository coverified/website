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
        }

        > div {
            display: flex;
            justify-content: space-between;

            > p {
                display: none;
                position: relative;
            }

            > img {
                position: relative;
                width: 9.375rem;
                padding-top: 2rem;
                padding-bottom: 3rem;
            }
        }
    }
    @media (max-width: 1200px) {
        footer {
            max-width: 60rem;
        }

        div {
            > img {
                width: 7.375rem;
            }
        }
    } 

    @media (max-width: 992px) {
        footer {
            max-width: 45rem;
        }
        
        div {
            > img {
                width: 5.375rem;
            }
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
            flex-direction: column;
            justify-content: center;
            > img {
                display: none;
            }

            > p {
                display: block;
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
        <img  src="bmg-logo.svg" alt="Bundesministerium für Gesundheit Logo">
        <p>
            Bundesministerium für Gesundheit
        </p>
        <img  src="bundesregierung-logo.svg" alt="Bundesregierung Logo">
        <p>
            Bundesregierung Deutschland
        </p>
        <img  src="rki-logo.svg" alt="Robert Koch Institut Logo">
        <p>
            Robert Koch Institut
        </p>
        <img  src="charite-logo.svg" alt="Charité Universitätsmedizin Berlin Logo">
        <p>
            Charité Universitätsmedizin Berlin
        </p>
        <img  src="john-hopkins-logo.svg" alt="John Hopkins Unviversity Logo">
        <p>
            John Hopkins Unviversity
        </p>
    </div>
</footer>
