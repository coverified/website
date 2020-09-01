<script>
    export let segment;

    let open = false;
</script>

<style type="text/scss">
    nav {
        font-weight: 300;
        display: flex;
        flex-direction: row;
        max-width: 71.25rem;
        margin: 0 auto;
        align-items: center;

        > a {
            display: flex;
            align-items: center;
            color: var(--color-primary);
            margin-right: auto;
            font-weight: 700;
            font-size: 1.25rem;
            line-height: 2.25rem;
            padding-top: .8rem;
            padding-bottom: .8rem;

            &:hover {
                color: #767676;
            }

            &:first-child {
                padding-left: 0;
            }

            > img {
                width: 2rem;
                height: auto;
                margin-right: .625rem;
            }
        }

        button {
            display: none;
        }

        .logo {
            width: 120px;
            height: 28px;
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

    .highlight {
        background-color: var(--color-primary);
        border: 1px solid var(--color-primary);
        border-radius: 5px;
        color: var(--color-white);
        padding: 0.45rem 1.75rem;
    }

    [aria-current] {
        box-shadow: inset 0 -3px 0 0 var(--color-primary);
        font-weight: bold;
    }

    a {
        text-decoration: none;
        padding: 0.45rem 1.5625rem;
        display: block;
        line-height: 20px;
        margin-left: 1rem;
        margin-right: 1rem;
    }

    @media (max-width: 1200px) {
        nav {
            max-width: 60rem;
        }
    }

    @media (max-width: 992px) {
        nav {
            max-width: 45rem;
        }
    }


    @media (max-width: 768px) {
        nav {
            max-width: 33.75rem;
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
                top: .875rem;
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
    </a>
    <ul class={open ? 'open' : ''}>
        <!-- <li>
            <a class="highlight"
               rel="prefetch"
               aria-current={segment === 'integration' ? 'page' : undefined}
               href="integration">
                Einbinden
            </a>
        </li> -->
        <li>
            <a rel="prefetch"
               aria-current={segment === 'news' ? 'page' : undefined}
               href="news">
                Covid-19 News
            </a>
        </li>
        <li>
            <a rel="prefetch"
               aria-current={segment === 'about' ? 'page' : undefined}
               href="about">
                das Projekt
            </a>
        </li>
        <li>
            <a rel="prefetch"
               aria-current={segment === 'contact' ? 'page' : undefined}
               href="contact">
                Kontakt
            </a>
        </li>

        <!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
                 the blog data when we hover over the link or tap it on a touchscreen -->
        <!--		<li><a rel=prefetch aria-current='{segment === "blog" ? "page" : undefined}' href='blog'>Blog</a></li>-->
    </ul>
    <button class={open ? 'open' : ''} on:click={() => {open = !open}}>
        <span></span>
        <span></span>
        <span></span>
    </button>
</nav>
