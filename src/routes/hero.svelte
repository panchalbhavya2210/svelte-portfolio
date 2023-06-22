<script>
  import "./styles.css";
  import flowerPic from "../lib/images/esther-lewis-yP0ntBuVcVA-unsplash.jpg";
  import blueGrad from "../lib/images/blue-gradient.svg";
  import arrow from "../lib/images/arrow.svg";
  import blueBorder from "../lib/images/blob-haikei.svg";

  let greetDay = new Date();

  let whichGreet = greetDay.getHours();

  function getHours() {
    if (whichGreet == 0) {
      return "Good Evening 👋,";
    } else if (whichGreet >= 5 && whichGreet <= 11) {
      return "Good Morning 👋,";
    } else if (whichGreet >= 12 && whichGreet <= 16) {
      return "Good Afternoon 👋,";
    } else if (whichGreet >= 17 && whichGreet <= 23) {
      return "Good Evening 👋,";
    }
  }
</script>

<svelte:head>
  <title>Home</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="margin">
  <img src={blueBorder} class="blueBorder" alt="blue-border" />
  <div class="positonAbsoluteImg">
    <img src={blueGrad} alt="blob" class="imgBlob" />
  </div>
  <div class="heroSection">
    <div class="mainDisplayFlex">
      <div class="anotherChild">
        <h1 class="myDetailsInShort">
          <span>{getHours()}</span><br />
          I Am <span class="brightColor">Bhavya</span>&nbsp;Panchal.
          <br />
          A Web Developer.
        </h1>
        <p class="myDetailsInSummary">
          A web developer and UI designer who loves turning ideas into reality.
          Always looking for ways to improve and grow in my craft!
        </p>
        <button class="exploreBtn"
          ><span class="black">EXPLORE <br /> IT.</span>
          <img src={arrow} alt="down-rotated-arrow" class="arrow" />
        </button>
      </div>
      <div class="detailsContainer" />
      <div class="imageContainer">
        <img src={flowerPic} alt="flowers-vertical" />
      </div>
    </div>
  </div>
</section>

<style>
  .margin {
    width: 100%;
    height: 100vh;
    font-family: Outfit;
    position: relative;
    top: 70px;
  }
  .positonAbsoluteImg {
    pointer-events: none;
    position: absolute;
    left: -25%;
    top: -30%;
    transform: scale(0.8);
    z-index: -5;
  }
  .mainDisplayFlex {
    width: 100%;
    height: 88vh;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 2;
  }
  .detailsContainer {
    position: relative;
    width: 70%;
    height: 80vh;
    background: #013075;
    background: radial-gradient(at right bottom, #013075, #001c43);
    color: #fff;
    z-index: 5;
    margin: 0 10px 0 50px;
    border-radius: 10px;
    opacity: 0.49;
  }
  .anotherChild {
    width: 70%;
    height: 80vh;
    position: absolute;
    left: 50px;
    opacity: 1;
    color: #fff;
    z-index: 6;
  }
  .myDetailsInShort {
    font-size: 4vw;
    font-weight: 500;
    line-height: 60px;
    margin: 30px 0 0 40px;
    letter-spacing: 0.6px;
  }
  .myDetailsInSummary {
    width: 60%;
    font-size: 2vw;
    margin: 20px 0 0 40px;
    font-weight: 300;
  }
  .imageContainer img {
    position: relative;
    width: 75%;
    object-fit: cover;
    height: 80vh;
    border-radius: 10px;
    margin: 0 0 0 30px;
    pointer-events: none;
    cursor: pointer;
    z-index: 66;
  }
  .exploreBtn {
    margin: 30px 0 0 40px;
    text-align: left;
    padding: 10px 15px;
    background-color: var(--bright-blue);
    border: none;
    outline: none;
    font-weight: 800;
    font-size: 1.4rem;
    font-family: Outfit;
    border-radius: 10px;
    cursor: pointer;
  }
  .arrow {
    widows: 20px;
    height: 18px;
    margin: 0 0 0 5px;
    pointer-events: none;
  }
  .brightColor {
    background: -webkit-linear-gradient(45deg, #35ffda, #3c9aff);
    -webkit-background-clip: text;
    background-clip: text;
    -webkit-text-fill-color: transparent;
    font-weight: 600;
  }
  .blueBorder {
    display: none;
  }
  @media only screen and (max-width: 675px) {
    .mainDisplayFlex {
      display: block;
      width: 100%;
    }
    .detailsContainer {
      display: none;
      margin: auto;
      width: 110%;
    }
    .myDetailsInShort {
      width: 100%;
      margin: 90px 0 0 -20px;
      font-size: 2rem;
      line-height: 50px;
    }
    .myDetailsInSummary {
      width: 100%;
      font-size: 1.5rem;
      margin: 50px 0 0 -20px;
    }
    .exploreBtn {
      margin: 50px 0 0 -20px;
    }
    .anotherChild {
      width: 100%;
    }
    .positonAbsoluteImg,
    .imageContainer {
      display: none;
    }
    .blueBorder {
      display: block;
      width: 100%;
      height: 100%;
      position: absolute;
      top: -50%;
      left: -50%;
      animation: rotate 30s ease-in-out infinite;
    }
    @keyframes rotate {
      0% {
        transform: rotate(0deg) scale(0.8);
      }
      50% {
        transform: rotate(360deg) scale(0.8);
      }
      100% {
        transform: rotate(0deg) scale(0.8);
      }
    }
  }
</style>
