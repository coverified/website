<script>
  export let segment;
</script>

<style type="text/scss">
  nav {
    font-weight: 300;
    display: flex;
    flex-direction: row;
    max-width: 71.25rem;
    margin: 0 auto;
    padding: 0 1rem;
    align-items: center;

    > a {
      margin-right: auto;
      font-weight: 700;
      font-size: 1.25rem;
      line-height: 1.25rem;
      &:hover {
        color: #767676;
      }
      &:active {
        color: #3753ff;
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

  [aria-current] {
    box-shadow: inset 0 -3px 0 var(--color-primary);
  }

  a {
    text-decoration: none;
    padding: 1.25rem 0.75rem;
    display: block;
    line-height: 20px;
  }
</style>

<nav>
  <a href=".">CoVerified</a>
  <ul>
    <li>
      <a
        rel="prefetch"
        aria-current={segment === 'about' ? 'page' : undefined}
        href="about">
        About
      </a>
    </li>
    <li>
      <a
        rel="prefetch"
        aria-current={segment === 'integration' ? 'page' : undefined}
        href="integration">
        Integration
      </a>
    </li>
    <li>
      <a href="https://github.com/coverified/" rel="noopener" target="_blank">
        <svg class="icon icon-github">
          <use xlink:href="#icon-github" />
        </svg>
      </a>
    </li>

    <!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
             the blog data when we hover over the link or tap it on a touchscreen -->
    <!--		<li><a rel=prefetch aria-current='{segment === "blog" ? "page" : undefined}' href='blog'>Blog</a></li>-->
  </ul>
</nav>
