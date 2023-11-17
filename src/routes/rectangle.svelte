<script defer>
  // @ts-nocheck

  import "./styles.css";
  export let src;
  export let languageName;
  export let alt;
</script>

<main>
  <div class="rect">
    <div class="flexMain">
      <img {src} {alt} srcset="" class="img" />
      <p class="bottomTxt">{languageName}</p>
    </div>
  </div>
</main>

<style>
  .rect {
    width: 80%;
    height: 130%;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: rgba(0, 26, 81, 0.215);
    border: 0.5px solid #727272;
    border-radius: 5px;
    cursor: default;
  }
  .flexMain {
    width: 100%;
    text-align: center;
  }
  .img {
    width: 20%;
    height: 20%;
    margin: 0 0 20px 0;
    pointer-events: none;
  }
  @media only screen and (max-width: 675px) {
    .rect {
      width: 150px;
      height: 120px;
    }
  }
</style>
