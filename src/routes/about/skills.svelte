<script>
  import chartJs from "/src/lib/iconsSkill/chart.svg";
  import css from "/src/lib/iconsSkill/css.svg";
  import figma from "/src/lib/iconsSkill/figma.svg";
  import firebase from "/src/lib/iconsSkill/firebase.svg";
  import git from "/src/lib/iconsSkill/git.svg";
  import html from "/src/lib/iconsSkill/html.svg";
  import node from "/src/lib/iconsSkill/node.svg";
  import php from "/src/lib/iconsSkill/php.svg";
  import react from "/src/lib/iconsSkill/react.svg";
  import socket from "/src/lib/iconsSkill/socket.svg";
  import svelte from "/src/lib/iconsSkill/svelte.svg";
  import js from "/src/lib/iconsSkill/js.svg";
  import Rectangle from "../rectangle.svelte";
</script>

<main>
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
      <Rectangle src={js} languageName={"JavaScript"} alt={"Javascript Logo"} />
      <Rectangle src={figma} languageName={"Figma"} alt={"Figma Logo"} />
      <Rectangle
        src={firebase}
        languageName={"Firebase"}
        alt={"Firebase Logo"}
      />
      <Rectangle src={svelte} languageName={"Svelte Kit"} alt={"Svelte Logo"} />
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
</main>

<style>
  .iconsMania {
    display: flex;
    justify-content: space-between;
    /* flex-direction: row-reverse; */
  }
  .iconsContainer {
    width: 70%;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(3, 1fr);
    grid-column-gap: 12px;
    grid-row-gap: 50px;
    margin: 0 0 80px 30px;
  }
  .skillNexp {
    width: 20%;
    margin: 0 00px 0 60px;
  }
  .titleOfExp {
    font-size: 2vw;
  }
  .detailOfexp {
    font-weight: 300;
    font-size: 1.4vw;
  }
  @media only screen and (max-width: 675px) {
    .iconsMania {
      width: 100%;
      display: block;
    }

    .iconsContainer {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-template-rows: repeat(6, 1fr);
      grid-column-gap: 15px;
      grid-row-gap: 35px;
      margin: 20px;
    }
    .skillNexp {
      width: 90%;
      margin: 0 0 0 30px;
    }
    .titleOfExp {
      font-size: 1.5rem;
    }
    .detailOfexp {
      width: 90%;
      font-size: 1rem;
    }
  }
</style>
