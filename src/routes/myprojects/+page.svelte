<script>
  import Myprojects from "./myprojects.svelte";
  import "../styles.css";
  import blueLine from "/src/lib/images/project-blob.svg";
</script>

<main>
  <div class="margin">
    <div class="aboutMeCent">
      <div class="rectAbt">
        <img src={blueLine} alt="" srcset="" class="rotate" />
        <p class="abtIndex">MY PROJECTS</p>
      </div>
    </div>
    <Myprojects />
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

  @keyframes rotate {
    0% {
      transform: rotate(0deg) scale(4);
    }
    50% {
      transform: rotate(360deg) scale(1);
    }
    100% {
      transform: rotate(360deg) scale(4);
    }
  }
  .rotate {
    animation: rotate 7s cubic-bezier(0.785, 0.135, 0.15, 1) infinite;
    z-index: 1;
    pointer-events: none;
  }
  @media only screen and (max-width: 675px) {
    .aboutMeCent {
      width: 100%;
      height: 100%;
      justify-content: center;
    }
    .rectAbt {
      width: 90%;
      height: 90%;
      /* background: linear-gradient(rgb(3, 0, 46), rgb(0, 157, 255)); */
    }
    .abtIndex {
      position: absolute;
      font-size: 2.5rem;
    }
    @keyframes rotate {
      0% {
        transform: rotate(0deg) scale(2);
      }
      50% {
        transform: rotate(360deg) scale(1);
      }
      100% {
        transform: rotate(360deg) scale(2);
      }
    }
    .rotate {
      animation: rotate 7s cubic-bezier(0.785, 0.135, 0.15, 1) infinite;
      z-index: 1;
      pointer-events: none;
    }
  }
</style>
