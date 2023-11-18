<script>
  import "../styles.css";
  import at from "/src/lib/icons/at.svg";
  import dis from "/src/lib/icons/dc.svg";
  import call from "/src/lib/icons/call.svg";
  import red from "/src/lib/icons/red.svg";
  import { blur } from "svelte/transition";

  import twitter from "/src/lib/icons/twitter.svg";
</script>

<svelte:head>
  <title>Connect - Bhavya Panchal</title>
  <meta name="description" content="Bhavya Panchal's Portfolio" />
</svelte:head>
<main
  transition:blur={{
    duration: 600,
    amount: 50,
  }}
>
  <div class="margin">
    <div class="aboutMeCent">
      <div class="rectAbt">
        <svg
          width="706"
          height="705"
          viewBox="0 0 706 705"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect
            x="70.1573"
            y="422"
            width="400"
            height="400"
            transform="rotate(-45 70.1573 422)"
            fill="#00E1D3"
          />
          <rect
            x="60.771"
            y="403.421"
            width="413.274"
            height="413.274"
            transform="rotate(-45 60.771 403.421)"
            stroke="#00E1D3"
            stroke-width="13"
          />
          <rect
            x="43.271"
            y="385.921"
            width="438.023"
            height="438.023"
            transform="rotate(-45 43.271 385.921)"
            stroke="#00E1D3"
            stroke-width="13"
          />
          <rect
            x="26.271"
            y="368.921"
            width="462.065"
            height="462.065"
            transform="rotate(-45 26.271 368.921)"
            stroke="#00E1D3"
            stroke-width="13"
          />
          <rect
            x="9.771"
            y="352.421"
            width="485.399"
            height="485.399"
            transform="rotate(-45 9.771 352.421)"
            stroke="#00E1D3"
            stroke-width="13"
          />
        </svg>
        <p class="abs">Contact Me</p>
      </div>
    </div>
    <div class="finalConnect">
      <div class="connectTitle on">
        <p><span class="brightColor">Thanks</span></p>
        <p>For Viewing My Site<span class="brightColor">.</span></p>
      </div>
      <div class="detailTitleN">
        <p>
          Thanks for spending your valuable time to view my site. If you've made
          it this far and you liked the work i did, you can contact me on below
          given details.
        </p>
        <br />
        <p>This portfolio was created using svelte, css, js and figma.</p>
      </div>
    </div>
    <div class="detailsMain">
      <div class="connectTitle">
        <p>Details<span class="brightColor">.</span></p>
      </div>
      <div class="detailTitle">
        <div class="contactMain">
          <a href="mailto:panchalbhavya2210@gmail.com">
            <div class="compOne">
              <div class="imgAll">
                <img src={at} alt="" class="icon" />
              </div>
              <div class="detailsFocus">
                <p class="whichCont">E-mail</p>
                <p class="thisCont">panchalbhavya2210@gmail.com</p>
              </div>
            </div>
          </a>
          <a href="tel:+919081865254">
            <div class="compOne">
              <div class="imgAll">
                <img src={call} alt="" class="callIcon" />
              </div>
              <div class="detailsFocus">
                <p class="whichCont">Call</p>
                <p class="thisCont">+91 90818 65254</p>
              </div>
            </div>
          </a>
          <a
            href="https://discord.com/users/705665317799591996"
            target="_blank"
          >
            <div class="compOne">
              <div class="imgAll">
                <img src={dis} alt="" class="icon" />
              </div>
              <div class="detailsFocus">
                <p class="whichCont">Discord</p>
                <p class="thisCont">#panchalbhavya2210</p>
              </div>
            </div>
          </a>
          <a
            href="https://www.reddit.com/user/agent-47---"
            target="_blank"
            rel="noopener noreferrer"
          >
            <div class="compOne">
              <div class="imgAll">
                <img src={red} alt="" class="icon" />
              </div>
              <div class="detailsFocus">
                <p class="whichCont">Reddit</p>
                <p class="thisCont">u/agent-47---</p>
              </div>
            </div>
          </a>
          <a
            href="https://twitter.com/panchalbhavya22"
            target="_blank"
            rel="noopener noreferrer"
          >
            <div class="compOne">
              <div class="imgAll">
                <img src={twitter} alt="" class="icon" />
              </div>
              <div class="detailsFocus">
                <p class="whichCont">Twitter</p>
                <p class="thisCont">@panchalbhavya22</p>
              </div>
            </div>
          </a>
        </div>
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
  @keyframes rotate {
    0% {
      transform: rotate(0deg) scale(3);
    }
    50% {
      transform: rotate(0deg) scale(1);
    }
    100% {
      transform: rotate(0deg) scale(3);
    }
  }
  .rectAbt svg {
    animation: rotate 7s infinite;
  }
  .abs {
    position: absolute;
    color: #000;
  }
  .finalConnect {
    width: 100%;
    height: 200px;
    display: flex;
    justify-content: flex-start;
    align-items: center;
  }
  .connectTitle {
    width: 25%;
    margin: 0 0 0 50px;
    font-size: 2vw;
    font-family: 400;
    height: 60px;
  }
  .on {
    height: 100px;
  }
  .detailTitleN {
    width: 80%;
    font-size: 1.7vw;
    font-weight: 300;
    margin: 0 60px 0 0;
  }
  .detailTitle {
    width: 90%;
    margin: 0 0 0 50px;
  }
  .contactMain {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 0px;
  }
  .icon {
    width: 40px;
    height: 40px;
    margin: 10px;
  }
  .callIcon {
    width: 30px;
    height: 30px;
    margin: 10px;
  }
  .compOne {
    display: flex;
    align-items: center;
    border-radius: 10px;
    margin: 0 10px;
    transition: 0.5s;
    height: 100px;
  }
  .whichCont {
    font-size: 1.5vw;
  }
  .thisCont {
    font-size: 1.2vw;
    font-weight: 300;
  }

  a {
    text-decoration: none;
    color: #fff;
    transition: 0.3s;
  }
  a:hover {
    filter: invert(0%) sepia(69%) saturate(6288%) hue-rotate(118deg)
      brightness(103%) contrast(102%);
  }
  @media only screen and (max-width: 675px) {
    .connectTitle p {
      width: 200px;
    }
    .on {
      width: 70%;
      height: 60px;
      margin: 30px 0 0 30px;
      font-size: 1.2rem;
    }
    .detailTitleN {
      width: 90%;
      font-size: 1rem;
      margin: 0;
      margin: 0 0 0 20px;
    }
    .abs {
      font-size: 2rem;
    }
    .contactMain {
      display: grid;
      grid-template-columns: repeat(1, 1fr);
      grid-template-rows: repeat(5, 1fr);
      grid-column-gap: 0px;
      grid-row-gap: 0px;
      margin: 0;
    }
    .whichCont,
    .thisCont {
      font-size: 0.8rem;
    }
    .callIcon {
      margin: 15px;
    }
    .detailTitle {
      margin: 0;
    }
    .finalConnect {
      width: 100%;
      height: 200px;
      display: block;
    }
    .connectTitle {
      margin: 30px 0 0 20px;
      font-size: 1.2rem;
    }
  }
</style>
