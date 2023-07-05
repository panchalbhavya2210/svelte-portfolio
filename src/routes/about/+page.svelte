<script>
  import "../styles.css";
  import blueLine from "/src/lib/images/about-me-blob.svg";
  import B from "/src/lib/images/my-image-removed-bg.png";
  import bigArrow from "/src/lib/icons/big-arrow.svg";
  import gitIcon from "/src/lib/icons/github.svg";
  // import chartJs from "/src/lib/iconsSKill/chart.svg";
  import css from "/src/lib/iconsSKill/css.svg";
  import figma from "/src/lib/iconsSKill/figma.svg";
  import firebase from "/src/lib/iconsSKill/firebase.svg";
  import git from "/src/lib/iconsSKill/git.svg";
  import html from "/src/lib/iconsSKill/html.svg";
  import node from "/src/lib/iconsSKill/node.svg";
  import php from "/src/lib/iconsSKill/php.svg";
  import react from "/src/lib/iconsSKill/react.svg";
  import socket from "/src/lib/iconsSKill/socket.svg";
  import svelte from "/src/lib/iconsSKill/svelte.svg";
  import js from "/src/lib/iconsSKill/js.svg";
  import Rectangle from "../rectangle.svelte";
</script>

<main>
  <div class="margin">
    <div class="aboutMeCent">
      <div class="rectAbt">
        <img src={blueLine} alt="" srcset="" class="rotate" />
        <p class="abtIndex">ABOUT ME...</p>
      </div>
    </div>

    <div class="lengthMyAbt">
      <div class="myImgLinks">
        <div class="imageHolder">
          <img src={B} alt="my img" class="b" />
        </div>
        <div class="linkHolder">
          <button class="designBtn">
            <a class="flex" href="/about">
              <img src={gitIcon} alt="right-arrow" class="gitIcon" />
              <span>Github Profile</span>
            </a>
          </button>
          <br />
          <button class="designBtn">
            <a class="flex" href="/myprojects">
              <img src={bigArrow} alt="right-arrow" class="btnBlue" />
              <span>Contact Me</span>
            </a>
          </button>
        </div>
      </div>

      <div class="aboutMe">
        <div class="aboutMePas">
          <p class="titleO">
            Hello, I Am Bhavya<span class="brightColor">.</span>
          </p>
          <p class="myDetails">
            I am a 22-year-old front-end website developer from India. And I am
            learning the backend. Currently, I am in college, doing the 5th
            semester of the BCA (Bachelor of Computer Application) Course at
            Monark University. I started programming as a hobby. I got into
            programming in lockdown and started learning it from the Mimo app
            and various YouTube channels.
            <br /><br />
            Beside working part-time at a pharmacy and doing college, I created some
            side projects that gave me a lot of experience. And I am also eager to
            learn new things. I have learned a lot from practicals.
          </p>
          <p class="titleO">
            Coding Journey<span class="brightColor">.</span>
          </p>
          <p class="myDetails">
            I started learning front-end website development in 2020. I did most
            of the learning from the Mimo App and YouTube Videos. After learning
            the basics, I got into creating various projects. I created some
            basic projects and improved them over time. I started coding on my
            phone, and I created various projects using the SPCK editor.
            <br /><br />
            After coding in mobile for a long time. I bought a laptop and started
            coding on it. I mostly use Visual Studio Code for programming. I am still
            learning the basics of the backend so I can become a full-stack developer.
          </p>
        </div>
      </div>
    </div>

    <div class="iconsMania">
      <div class="skillNexp">
        <p class="titleOfExp">
          Skills <span class="brightColor">&</span> Experience<span
            class="brightColor">.</span
          >
        </p>
        <br />
        <p class="detailOfexp">
          I've been programming for more than a year, and there is a lot I've
          learned from creating projects.
          <br /><br />
          These are the languages, frameworks, and services I have experience in.
        </p>
      </div>
      <div class="iconsContainer">
        <Rectangle src={html} languageName={"HTML5"} alt={"Html Logo"} />
        <Rectangle src={css} languageName={"CSS3"} alt={"Css Logo"} />
        <Rectangle
          src={js}
          languageName={"JavaScript"}
          alt={"Javascript Logo"}
        />
        <Rectangle src={figma} languageName={"Figma"} alt={"Figma Logo"} />
        <Rectangle
          src={firebase}
          languageName={"Firebase"}
          alt={"Firebase Logo"}
        />
        <Rectangle
          src={svelte}
          languageName={"Svelte Kit"}
          alt={"Svelte Logo"}
        />
        <Rectangle src={git} languageName={"GIT"} alt={"Git Logo"} />
        <Rectangle
          src={chartJs}
          languageName={"Chart JS"}
          alt={"Chart Js Logo"}
        />
        <Rectangle src={node} languageName={"Node JS"} alt={"Node Js Logo"} />
        <Rectangle src={php} languageName={"PHP"} alt={"Php Logo"} />
        <Rectangle
          src={react}
          languageName={"React JS (Basics)"}
          alt={"React Logo"}
        />
        <Rectangle
          src={socket}
          languageName={"Socket IO"}
          alt={"Socket iO Logo"}
        />
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
    z-index: 1;
    pointer-events: none;
  }

  .b {
    width: 130px;
    height: 130px;
    object-fit: cover;
    border-radius: 100%;
    filter: brightness(105%) saturate(100%);
    pointer-events: none;
    background: linear-gradient(-45deg, rgb(93, 255, 204), rgb(149, 139, 255));
    pointer-events: none;
  }
  .gitIcon {
    width: 24px;
    height: 24px;
  }
  .designBtn a:hover .gitIcon {
    filter: invert(0%) sepia(69%) saturate(6288%) hue-rotate(118deg)
      brightness(103%) contrast(102%);
  }
  .lengthMyAbt {
    width: 100%;
    height: 500px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .myImgLinks {
    height: 400px;
    margin: 0 0 0 90px;
  }
  .aboutMe {
    width: 65%;
    height: 400px;
    margin: 0 50px 0 0;
  }
  .titleO {
    font-size: 2vw;
    font-weight: 500;
    margin: 0 0 15px 0;
  }
  .myDetails {
    font-size: 1.3vw;
    font-weight: 300;
    margin: 0 0 30px 0;
    /* line-height: 28px; */
  }
  .iconsMania {
    display: flex;
    justify-content: space-between;
    flex-direction: row-reverse;
  }
  .iconsContainer {
    width: 70%;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(3, 1fr);
    grid-column-gap: 12px;
    grid-row-gap: 40px;
    margin: 0 0 0 50px;
  }
  .skillNexp {
    width: 25%;
    margin: 0 40px 0 0;
  }
  .titleOfExp {
    font-size: 2vw;
  }
  .detailOfexp {
    font-weight: 300;
    font-size: 1.4vw;
  }
</style>
