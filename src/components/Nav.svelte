<script>
    export let segment;
</script>

<style type="text/scss">
    nav {
        font-weight: 300;
        display: flex;
        flex-direction: row;
        max-width: 71.25rem;
        height: 3.75rem;
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
        <!--    TODO: change to svg-->
        <img src="favicon-32x32.png" alt="CoVerified Logo">
        CoVerified
    </a>
    <ul>
        <li>
            <a class="highlight"
               rel="prefetch"
               aria-current={segment === 'integration' ? 'page' : undefined}
               href="integration">
                Einbinden
            </a>
        </li>
        <li>
            <a rel="prefetch"
               aria-current={segment === 'about' ? 'page' : undefined}
               href="about">
                Information
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
</nav>
