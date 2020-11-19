<script>
    export let segment;

    let open = false;
</script>

<style type="text/scss">
    nav {
        display: flex;
        flex-direction: row;
        max-width: 71.25rem;
        margin: 0 auto;
        align-items: center;

        > a {
            display: flex;
            flex-direction: column;
            color: var(--color-primary);
            margin-right: auto;
            padding-top: .8rem;
            padding-bottom: .8rem;

            &:first-child {
                padding-left: 0;
            }

            > p {
                font-size: .75rem;
                line-height: normal;
                margin-bottom: 0;
            }

        }

        button {
            display: none;
        }

        .logo {
            width: 165px;
            height: auto;
        }
    }

    ul {
        margin: 0;
        padding: 0;

        &:after {
            content: "";
            display: block;
            clear: both;
        }
    }

    li {
        display: block;
        float: left;
    }

    [aria-current] {
        box-shadow: inset 0 -2px 0 0 var(--color-primary);
    }

    a {
        text-decoration: none;
        padding: 0.45rem .75rem 1rem .75rem;
        display: block;
        line-height: 20px;
        margin-left: 1rem;
        margin-right: 1rem;

        &:hover,
        &:focus {
            box-shadow: inset 0 -2px 0 0 var(--color-primary);
        }
    }

    @media (min-width: 992px) {
        .contact {
        --btn-primary-bg-color: var(--color-primary);
        --btn-primary-text-color: var(--color-white);
        --btn-primary-border-color: var(--color-primary);
        --btn-primary-border-width: 1px;
        --btn-primary-border-style: solid;
        --btn-primary-border-radius: 2rem;
        --btn-padding: 0.75rem 2.5rem;
        --text-decoration: none;

        background-color: var(--btn-primary-bg-color);
        color: var(--btn-primary-text-color) !important;
        padding: var(--btn-padding);
        border-color: var(--btn-primary-border-color);
        border-width: var(--btn-primary-border-width);
        border-style: var(--btn-primary-border-style);
        border-radius: var(--btn-primary-border-radius);
        text-decoration: var(--text-decoration);
        }
    }

    @media (max-width: 1200px) {
        nav {
            max-width: 60rem;
        }
    }

    @media (max-width: 992px) {
        nav {
            max-width: 45rem; 
            display: flex;
            flex-direction: column;
            position: relative;

            button {
                display: flex;
                flex-direction: column;
                justify-content: space-around;
                width: 2.5rem;
                height: 2.2rem;
                position: absolute;
                right: 0;
                top: 1.25rem;
                margin-right: 1rem;
                appearance: none;
                border: 0;
                padding: 0;
                background: transparent;

                span {
                    display: block;
                    width: 2.5rem;
                    height: 4px;
                    border-radius: 3px;
                    background-color: var(--color-dark-grey);
                }

                &.open {
                    span {
                        &:nth-child(2) {
                            opacity: 0;
                        }

                        &:nth-child(1) {
                            transform: translateY(.725rem) rotate(45deg);
                        }

                        &:nth-child(3) {
                            transform: translateY(-.725rem) rotate(-45deg);
                        }
                    }
                }
            }

            ul {
                display: none;
                flex-direction: column;
                width: 100%;

                &.open {
                    display: flex;
                }

                li {
                    margin-top: .33rem;
                    margin-bottom: .33rem;
                }
            }        
        }    
        [aria-current] {
            box-shadow: 0;
            background-color: var(--color-primary);
            color: var(--color-white);
            padding: .75rem;
            font-weight: 400;
        }    
    }


    @media (max-width: 768px) {
        nav {
            max-width: 33.75rem;
        }  
    }

    @media (max-width: 576px) {
        nav {
            max-width: 22.5rem;
        }
    }
</style>

<nav>
    <a href=".">
        <img  class="logo" src="coverified_logo.svg" alt="CoVerified" width="475" height="111"/>
        <p>
            Redefining Communication
        </p>
    </a>
    <ul class={open ? 'open' : ''}>
        <li>
            <a rel="prefetch"
               aria-current={segment === 'technology' ? 'page' : undefined}
               href="technology">
                Technologie
            </a>
        </li>
        <li>
            <a rel="prefetch"
               aria-current={segment === 'wika' ? 'page' : undefined}
               href="wika">
                Projekt Wika
            </a>
        </li>
        <li>
            <a rel="prefetch"
               aria-current={segment === 'about' ? 'page' : undefined}
               href="about">
                Über CoVerified
            </a>
        </li>
        <li>
            <a rel="prefetch"
               class="contact"
               aria-current={segment === 'contact' ? 'page' : undefined}
               href="contact">
                Kontakt
            </a>
        </li>
    </ul>
    <button class={open ? 'open' : ''} on:click={() => {open = !open}}>
        <span></span>
        <span></span>
        <span></span>
    </button>
</nav>
