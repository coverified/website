<script>
  import Button from "../components/Button.svelte";
  import Article from "../components/Article.svelte";
</script>

<style type="text/scss">
  :root {
    overflow-x: hidden;
  }
  
  h1 {
    font-size: 2.25rem;
    font-weight: 700;
    color: var(--color-white);
    line-height: 48px;
  }

  h2 {
    font-size: 2.25rem;
    font-weight: 700;
    margin: 0 0 1rem 0;
  }

  .container {  
    position: relative;
    height: auto;
    margin-bottom: 6.5em;
    
  
    &:before {
      content: "";
      position: absolute;
      background: var(--color-primary);
      display: block;
      width: 100vw;
      height: 100%;
      left: 50%;
      right: 0;
      bottom: 0;
      top: 0;
      transform: translateX(-50%);
    }
    
    > div:not(.info__box) {
      position: absolute;
      right: 0;
      top: 53%;
      display: flex;
      align-items: center;
      
      > h1 {
        margin-right: 4rem;
      }

      > div {
        > p {
          margin-top: 0;
          margin-bottom: .5rem;
          font-size: .875rem;
          position: relative;
          font-weight: 800;
          padding-left: 1.7rem;
          
          &:before {
            content: "✓";
            position: absolute;
            width: 20px;
            height: 20px;
            font-weight: 400;
            text-align: center;
            border: 1.8px solid var(--color-white);
            border-radius: 50%;
            left: 0;
            top: 2px;
            line-height: 1;
            padding-top: .13em;
          }
        }
      }
    }
    
    .coverified__informationgraphic {
      position: relative;
      width: 50%;
      padding-top: 2rem;
      padding-bottom: .5rem;
    }
    
    .wirvsvirus__logo {
      width: 19rem;
      height: auto;
      position: absolute;
      right: 0;
      top: 10%;
    }

    p {
      color: var(--color-white);
    }
    
    .info__box {
      display: flex;
      flex-direction: column;
      position: absolute;
      padding: 1rem 1.75rem;
      right: 0;
      bottom: 0;
      transform: translateY(50%);
      background-color: var(--color-white);
      border: 1px solid var(--color-light-grey);
      box-shadow: 0px 1px 6px -3px rgba(0,0,0,0.11);
      

      > table {
        > tr {
          > td {
            padding-right: 11px;

          }
        }
      }

      > .footnote {
        font-size: 12px;
        color: var(--color-dark-grey);
        margin-left: 0;
        margin-right: 0;
        margin-top: .8rem;
      }
    }
  }

  .text__color--green {
    color: var(--color-green);
  }

  .news {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(345px, 1fr));
    grid-gap: 2rem;
    background-color: #fff;
    position: relative;
  }

  @media (max-width: 992px) {
    h1 {
      font-size: 2rem;
    }

    .container {
      display: flex;
      justify-content: center;
      margin-bottom: 8.5rem;
      
      > div:not(.info__box) {
      right: unset;
      top: 0;
      
        > h1 {
          padding-top: 1.75rem;
          margin-right: 0;
        }
      }
      > .info__box {
        right: unset;
      }

      .desktop__only {
        display: none;
      }
      .wirvsvirus__logo {
        top: 20%;
      }
    
      .coverified__informationgraphic {
        width: 58%;
        padding-top: 14rem;
        padding-bottom: 7.5rem;
      }
    }

  }

  @media (max-width: 768px) {
    h1 {
      font-size: 1.8rem;
    }
    .container {
      > .info__box {
        
      }

      .coverified__informationgraphic {
        width: 69%;
      }
    }  
  }
  

  @media (max-width: 576px) {
    h1 {
      font-size: 1.575rem;
      line-height: 33.6px;
    }

    .container {
      > .info__box {
        
      }
      
      .coverified__informationgraphic {
        width: 90%;
        padding-top: 11rem;
        padding-bottom: 7rem;
      }

      .wirvsvirus__logo {
        width: 16rem;
        top: 18.5%;
      }
    }  
  }
</style>

<svelte:head>
  <title>CoVerified</title>
  <meta name="description" content="CoVerified" />
</svelte:head>

<h1 class="sr-only">CoVerified</h1>
<div class="container">
  <img class="coverified__informationgraphic" src="coverified-information-graphic.svg" alt="Coverified Information graphic">
  <img class="wirvsvirus__logo" src="wirvsvirus-weiss.svg" alt="Wir vs Virus Projekt">
  <div>
    <h1>
      Valid Information about the<br /> Covid-19 Disease Outbreak.
    </h1>
    <div class="desktop__only">
      <p>Verified Sources</p>
      <p>Only current news</p>
      <p>Good accesability</p>
    </div>
  </div>
  <div class="info__box">
    <table>
      <tr>
        <td>
          <b>431.337</b>
        </td>
        <td>
          Covid-19 Erkrankte in Deutschland
        </td>
      </tr>
      <tr>
        <td>
          <b>92</b>
        </td>
        <td>
          Todesfälle in Deutschland
        </td>
      </tr>
      <tr>
        <td class="text__color--green">
          <b>295</b>
        </td>
        <td>
          Genesungen in Deutschland
        </td>
      </tr>
    </table>
    <p class="footnote">Stand 28. März 2020, Quelle John Hopkins University</p>
  </div>
</div>

<h2>Current News</h2>
<div class="news">
  <Article />
  <Article />
  <Article />
  <Article />
  <Article />
  <Article />
</div>
