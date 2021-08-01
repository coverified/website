<script>
  let label;
  let href;
  let target;
  let style;
  let rel;
  export { label, href, target, rel, style};
</script>

<style type="text/scss">

  .btn-primary,
  .btn-primary--border,
  .btn-secondary {
    display: inline-block;
    --btn-font-weight: 300;
    --text-decoration: none;
    transition: transform .2s;

    &:active {
      transform: translate(0, 2px);
    }
  }

  .btn-primary,
  .btn-secondary {
    --btn-padding: 0.75rem 4.6875rem;
  }

  .btn-primary--border {
    --btn-padding: 0.75rem 3.6875rem;
  }

  .btn-primary {
    --btn-primary-bg-color: var(--color-primary);
    --btn-primary-text-color: var(--color-white);
    --btn-primary-border-color: var(--color-primary);
    --btn-primary-border-width: 1px;
    --btn-primary-border-style: solid;
    --btn-primary-border-radius: 2rem;
    
    background-color: var(--btn-primary-bg-color);
    color: var(--btn-primary-text-color) !important;
    padding: var(--btn-padding);
    border-color: var(--btn-primary-border-color);
    border-width: var(--btn-primary-border-width);
    border-style: var(--btn-primary-border-style);
    border-radius: var(--btn-primary-border-radius);
    font-weight: var(--btn-font-weight);
    text-decoration: var(--text-decoration);

    &:hover {
      background-color: var(--color-white);
      color: var(--color-primary) !important;
    }
  }

  .btn-secondary {
    --btn-secondary-bg-color: var(--color-white);
    --btn-secondary-text-color: var(--color-primary);
    --btn-secondary-border-color: var(--color-white);
    --btn-secondary-border-width: 1px;
    --btn-secondary-border-style: solid;
    --btn-secondary-border-radius: 2rem;

    background-color: var(--btn-secondary-bg-color);
    color: var(--btn-secondary-text-color) !important;
    padding: var(--btn-padding);
    border-color: var(--btn-secondary-border-color);
    border-width: var(--btn-secondary-border-width);
    border-style: var(--btn-secondary-border-style);
    border-radius: var(--btn-secondary-border-radius);
    font-weight: var(--btn-font-weight);
    text-decoration: var(--text-decoration);    

    &:active {
      background-color: var(--color-light-grey) !important;
      border-color: var(--color-light-grey) !important;
    }

    &:hover {
      background-color: var(--color-primary);
      color: var(--color-white) !important;
    }
  }

  .btn-primary--border {
    --btn-primary-bg-color: var(--color-primary);
    --btn-primary-text-color: var(--color-white);
    --btn-primary-border-color: var(--color-white);
    --btn-primary-border-width: 1px;
    --btn-primary-border-style: solid;
    --btn-primary-border-radius: 2rem;
    
    background-color: var(--btn-primary-bg-color);
    color: var(--btn-primary-text-color) !important;
    padding: var(--btn-padding);
    border-color: var(--btn-primary-border-color);
    border-width: var(--btn-primary-border-width);
    border-style: var(--btn-primary-border-style);
    border-radius: var(--btn-primary-border-radius);
    font-weight: var(--btn-font-weight);
    text-decoration: var(--text-decoration);

    &:hover {
      background-color: var(--color-white);
      color: var(--color-primary) !important;
    }
  }

  @media (max-width: 992px) {
    .btn-primary,
    .btn-secondary {
      --btn-padding: 0.75rem 1rem;    
    }
  }
</style>

<a href="{href}" class="{style}" target="{target}" rel="{rel}">
  {label}
</a>

