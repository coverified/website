<script>
  export let label;
</script>

<style type="text/scss">
  .button-primary {
    --btn-primary-bg-color: var(--color-primary);
    --btn-primary-text-color: var(--color-white);
    --btn-primary-padding: 0.75rem 2rem;
    --btn-primary-border-color: var(--color-primary);
    --btn-primary-border-width: 1px;
    --btn-primary-border-style: solid;
    --btn-primary-border-radius: 5px;

    background-color: var(--btn-primary-bg-color);
    color: var(--btn-primary-text-color);
    padding: var(--btn-primary-padding);
    border-color: var(--btn-primary-border-color);
    border-width: var(--btn-primary-border-width);
    border-style: var(--btn-primary-border-style);
    border-radius: var(--btn-primary-border-radius);
  }

  /* .secondary {
    --btn-secondary-bg-color: var(--color-light-secondary);
    --btn-secondary-text-color: (--color-anthracite);
    --btn-secondary-padding: 0.75rem 2rem;
    --btn-secondary-border-color: var(--color-light-secondary);
    --btn-secondary-border-width: 1px;
    --btn-secondary-border-style: solid;
    --btn-secondary-border-radius: 5px;

    background-color: var(--btn-secondary-bg-color-primary);
    color: var(--btn-secondary-text-color);
    padding: var(--btn-secondary-padding);
    border-color: var(--btn-secondary-border-color);
    border-width: var(--btn-secondary-border-width);
    border-style: var(--btn-secondary-border-style);
    border-radius: var(--btn-secondary-border-style);
  }*/
</style>

<button class="button-primary">{label}</button>
