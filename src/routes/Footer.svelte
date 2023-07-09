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
          <p class="hoverP">
            <a href="/">Home</a>
          </p>
          <p class="hoverP">
            <a href="/about">About Me</a>
          </p>
          <p class="hoverP">
            <a href="/myprojects">My Projects</a>
          </p>
          <p class="hoverP">
            <a href="/connect">Connect</a>
          </p>
        </div>
      </div>
      <div class="letMainDiv">
        <img src={linksSvg} alt="links-svg" class="imgWidthAdj listAdjust" />
        <div class="listOfLinks">
          <p class="hoverP">
            <a href="https://github.com/panchalbhavya2210" target="_blank"
              >Github Profile</a
            >
          </p>
          <p class="hoverP">
            <a href="https://twitter.com/panchalbhavya22" target="_blank"
              >Twitter</a
            >
          </p>
          <p class="hoverP">
            <a href="https://www.reddit.com/user/agent-47---" target="_blank"
              >Reddit</a
            >
          </p>
          <p class="hoverP">
            <a href="mailto:panchalbhavya2210@gmail.com">G-Mail</a>
          </p>
        </div>
      </div>
      <div class="letMainDiv">
        <img
          src={resourceSvg}
          alt="resources-svg"
          class="imgWidthAdj resAdjust"
        />
        <div class="listOfRes">
          <p class="hoverP">
            <a href="https://unsplash.com/@_esther_" target="_blank"
              >Wallpaper</a
            >
          </p>
          <p class="hoverP">
            <a href="https://figma.com" target="_blank">Figma(Designing)</a>
          </p>
          <p class="hoverP">
            <a href="https://fonts.google.com" target="_blank">Outfit(Font)</a>
          </p>
          <p class="hoverP">
            <a href="https://iconify.design" target="_blank">Iconify(Icons)</a>
          </p>
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
    background-color: rgba(0, 0, 42, 0.534);
  }
  .footerFlex {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
  }
  .madeByLogo {
    font-size: 2.5vw;
    font-weight: 500;
    margin: 30px 0 0 30px;
    /* line-height: 60px; */
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
    cursor: pointer;
    position: absolute;
    top: 34px;
    left: 30%;
    line-height: 40px;
  }
  .listOfLinks {
    left: 43%;
  }
  .listOfRes {
    left: 33%;
  }
  .listOfNav a,
  .listOfLinks a,
  .listOfRes a {
    position: relative;
    text-decoration: none;
    color: #fff;
    transition: 0.5s;
  }
  a:after {
    position: absolute;
    content: "";
    left: 0;
    bottom: -2px;
    width: 0px;
    height: 2px;
    background-color: var(--bright-blue);
    border-radius: 10px;
    transition: 0.2s cubic-bezier(0.25, 0.46, 0.45, 0.94);
  }
  .hoverP:hover a:after {
    height: 2px;
    width: 100%;
  }

  @media only screen and (max-width: 675px) {
    .footerMain {
      width: 90%;
      background-color: rgba(255, 0, 0, 0);
      margin: 100px 0 0 0;
    }
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

  @media screen and (min-width: 1024px) and (min-height: 1310px) {
    .listOfNav {
      position: absolute;
      top: 25px;
      left: 140px;
      font-size: 1.1rem;
      line-height: 39px;
    }

    .listOfLinks {
      left: 190px;
    }

    .listOfRes {
      left: 160px;
    }
  }
</style>
