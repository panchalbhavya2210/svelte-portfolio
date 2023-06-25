<script>
  import { page } from "$app/stores";
  import navigationSvg from "../lib/images/navigation.svg";
  import linksSvg from "../lib/images/links.svg";
  import resourceSvg from "../lib/images/resources.svg";

  import "./styles.css";
</script>

<main>
  <div class="footerMain">
    <div class="footerFlex">
      <div class="madeByLogo">
        <p>Created By</p>
        <p />
        <p>Bhavya</p>
        <p>Panchal<span class="brightColor">.</span></p>
      </div>
      <div class="letMainDiv">
        <img src={navigationSvg} alt="navigation-svg" class="imgWidthAdj" />
        <div class="listOfNav">
          <p>Home</p>
          <p>About Me</p>
          <p>My Projects</p>
          <p>Connect</p>
        </div>
      </div>
      <div class="letMainDiv">
        <img src={linksSvg} alt="links-svg" class="imgWidthAdj listAdjust" />
        <div class="listOfLinks">
          <p>Home</p>
          <p>About Me</p>
          <p>My Projects</p>
          <p>Connect</p>
        </div>
      </div>
      <div class="letMainDiv">
        <img
          src={resourceSvg}
          alt="resources-svg"
          class="imgWidthAdj resAdjust"
        />
        <div class="listOfRes">
          <p>Home</p>
          <p>About Me</p>
          <p>My Projects</p>
          <p>Connect</p>
        </div>
      </div>
    </div>
  </div>
</main>

<style>
  .footerMain {
    position: relative;
    width: 100%;
    height: 300px;
    font-family: Outfit;
    color: #fff;
    margin: 80px 0 0 0;
  }
  .footerFlex {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
  }
  .madeByLogo {
    font-size: 3vw;
    font-weight: 500;
    margin: 0 0 0 30px;
    line-height: 60px;
  }
  .letMainDiv {
    position: relative;
    width: 70%;
    height: 70%;
  }
  .imgWidthAdj {
    width: 100%;
    height: 100%;
  }
  .listOfNav,
  .listOfLinks,
  .listOfRes {
    position: absolute;
    top: 28px;
    left: 30%;
    line-height: 40px;
  }
  .listOfLinks {
    left: 43%;
  }
  .listOfRes {
    left: 33%;
  }
  @media only screen and (max-width: 675px) {
    .madeByLogo {
      font-size: 1.5rem;
      font-weight: 500;
      line-height: 30px;
      margin: 30px;
    }
    .footerFlex {
      width: 100%;
      height: 100%;
      display: block;
    }
    .imgWidthAdj {
      width: 200px;
      height: 200px;
    }
    .letMainDiv {
      position: relative;
      width: 100%;
      height: 70%;
      left: 0;
      margin: 0 0 0 30px;
    }
    .listAdjust {
      margin: 0 0 0 -45px;
    }
    .resAdjust {
      margin: 0 0 0 -10px;
    }
    .listOfNav,
    .listOfLinks,
    .listOfRes {
      position: absolute;
      top: 25px;
      left: 35px;
      font-size: 1.1rem;
      line-height: 39px;
    }
  }
</style>
