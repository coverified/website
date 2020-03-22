<script>
    export let segment;
</script>

<style>
    nav {
        font-weight: 300;
        display: flex;
        flex-direction: row;
        max-width: 71.25rem;
        margin: 0 auto;
        padding: 0 1rem;
        align-items: center;
    }

    nav > a {
        margin-right: auto;
        font-weight: 700;
        font-size: 20px;
        line-height: 1;
    }

    ul {
        margin: 0;
        padding: 0;
    }

    /* clearfix */
    ul::after {
        content: '';
        display: block;
        clear: both;
    }

    li {
        display: block;
        float: left;
    }

    [aria-current] {
        box-shadow: inset 0 -2px 0 #3753ff;
    }

    a {
        text-decoration: none;
        padding: 1.25rem 1rem;
        display: block;
        line-height: 20px;
    }
</style>

<nav>
    <a href=".">CoVerified</a>
    <ul>
        <li><a href='https://github.com/coverified/webcomponent' rel="noopener" target="_blank">Tech Docs</a></li>

        <!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
             the blog data when we hover over the link or tap it on a touchscreen -->
        <!--		<li><a rel=prefetch aria-current='{segment === "blog" ? "page" : undefined}' href='blog'>Blog</a></li>-->
    </ul>
</nav>
