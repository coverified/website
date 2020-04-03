<script>
  export let label;
  export let firstItem;
  export let secondItem;
  export let thirdItem;
</script>

<style type="text/scss">  
  .list__container {
    display: flex;
    justify-content: space-between;

    > h2 {
      font-weight: 700;
      font-size: 2rem;
      margin-bottom: 2rem;
    }

    > ul {
      max-width: 28.125rem;
      margin-top: 0;
      list-style: none;
      margin-right: 5rem;

      > li {
        position: relative;
        padding-left: 1.825rem;
        font-weight: 700;
        margin-bottom: 1rem;

        &:before {
          content: "✓";
          position: absolute;
          width: 20px;
          height: 20px;
          font-weight: 400;
          text-align: center;
          color: var(--color-white);
          background-color: var(--color-primary);
          border: 1.8px solid var(--color-primary);
          border-radius: 50%;
          left: 0;
          top: 3px;
          line-height: 1;
        }
      }
    }
  }

  @media (max-width: 768px) {
    .list__container {
      flex-direction: column;
      align-items: center;

      > ul {
        margin-right: 0;
      }
    }
  }

</style>

 <div class="list__container">
    <h2>
      {label}
    </h2>
    <ul>
      <li>
        {firstItem}
      </li>
      <li>
        {secondItem}
      </li>
      <li>
        {thirdItem}
      </li>
    </ul>
  </div>
