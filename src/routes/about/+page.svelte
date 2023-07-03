<script>
  import "../styles.css";
  import blueLine from "/src/lib/images/about-me-blob.svg";
  import B from "/src/lib/images/my-image-removed-bg.png";
  import bigArrow from "/src/lib/icons/big-arrow.svg";
  import gitIcon from "/src/lib/icons/github.svg";
  import chartJs from "/src/lib/iconsSKill/chart.svg";
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
  import vercel from "/src/lib/iconsSKill/vercel.svg";
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
            I am 22 year old <span class="brightColor"
              >frontend website developer from India. And i am learning backend.</span
            >
            Currently i am in college doing 5th semester of BCA(Bachelor Of Computer
            Application) Course at Monark University. I started programming as hobby.
            I got into programming in lockdown and started learning it from mimo
            app and various youtube channels.

            <br /><br />
            Beside working part-time at pharmacy and doing college i created some
            side project that gave me alot of experience. And i am also eager to
            learn new thing. I have learned a lot from practical.
          </p>
          <p class="titleO">
            Coding Journey<span class="brightColor">.</span>
          </p>
          <p class="myDetails">
            I started learning frontend website development in 2020. I did
            learning from Mimo App and Youtube Videos. After learning basics i
            got into creating various project. I created some basic project and
            improved them time by time. I started coding in phone and i created
            various project using spck editor.
            <br /> <br />
            After coding in mobile for a long time. I bought laptop and started coding
            in it. I mostly use visual stodio code for programming. I am stil learning
            basics of backend so i can become a fullstack developer.
          </p>
        </div>
      </div>
    </div>

    <div class="iconsMania">/</div>
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
</style>
