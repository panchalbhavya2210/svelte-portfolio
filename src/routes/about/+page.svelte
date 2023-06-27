<script>
  import "../styles.css";
  import blueLine from "/src/lib/images/about-me-blob.svg";
</script>

<main>
  <div class="margin">
    <div class="aboutMeCent">
      <div class="rectAbt">
        <img src={blueLine} alt="" srcset="" class="rotate" />
        <p class="abtIndex">ABOUT ME...</p>
      </div>
    </div>
  </div>
</main>

<style>
  .margin {
    position: relative;
    top: 80px;
    color: #fff;
    font-family: Outfit;
  }
  .aboutMeCent {
    width: 100%;
    height: 500px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .rectAbt {
    width: 95%;
    height: 400px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #002d46;
    border-radius: 10px;
    font-size: 5vw;
    font-weight: 600;
    overflow: hidden;
    letter-spacing: 2px;
    box-shadow: 0 0 5px var(--dim-blue);
  }
  .abtIndex {
    z-index: 2;
    color: #fff;
    mix-blend-mode: color-dodge;
  }
  .rotate {
    animation: rotate 7s cubic-bezier(0.785, 0.135, 0.15, 0.86) infinite;
    /* animation: rotate 10s cubic-bezier(0.86, 0, 0.07, 1) infinite; */
    z-index: 1;
  }
</style>
