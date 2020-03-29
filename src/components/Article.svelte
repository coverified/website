<script>
</script>

<style type="text/scss">
  article {
    color: var(--color-anthracite);
    padding: 1rem;
    margin: 0;
    border: 1px solid var(--color-light-grey);
    border-radius: 5px;
    box-shadow: 0 1px 6px -3px rgba(var(--color-light-grey), 0.2);
    
    > a {
      display: flex;
      align-items: center;
      text-decoration: none;

      > h2 {
        font-size: 20px;
        font-weight: 700;
        margin-bottom: 0;
        margin-left: .75rem;
      }

      >img {
        width: 2rem;
        height: auto;
      }
    }

    > p {
      margin-bottom: .625rem;
    }

    div {
      display: flex;
      justify-content: space-between;
      margin-top: 5px;

      > p {
        font-size: .875em;
        color: var(--color-dark-grey);
        margin: 0;
      }

      > img {
        width: .9375rem;
        height: auto;
        margin-right: .375rem;
      }
    }
    
    p + a {
      position: relative;
      padding-left: 2.05em;
      font-size: 0.875em;
      text-decoration: underline !important;

      &:before {
        content: "→";
        display: block;
        font-weight: 300;
        border-radius: 50%;
        background-color: var(--color-primary);
        color: var(--color-white);
        position: absolute;
        left: 0;
        width:1.25em;
        height: 1.25em;
        text-align: center;
        z-index: 1;
        padding-top: 0.15em;
        line-height: 1;
      }
    }
  }
</style>

<article>
  <a href=".">
    <img src="favicon-32x32.png" alt="CoVerified Logo">
    <h2>
      Headline
    </h2>
  </a>
  <div>
    <div>
      <img src="source-icon.svg" alt="Source Icon">
      <p>
        Pressestelle Landesregierung Bayern
      </p>
    </div>
    <div>
      <img src="clock-icon.svg" alt="Clock Icon">
      <p>
        13:37h
      </p>
    </div>
  </div>
  <p>
    An dieser Stelle dokumentieren wir die bestätigte Anzahl aller Personen, bei
    denen seit Beginn der Epidemie in Deutschland eine Infektion mit dem
    neuartigen Coronavirus nachgewiesen wurde.
  </p>
  <a href="." title="Weiterlesen">
    Weiterlesen
  </a>
</article>
