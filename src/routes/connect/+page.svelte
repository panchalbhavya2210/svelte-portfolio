<script>
  import "../styles.css";
  import at from "/src/lib/icons/at.svg";
  import dis from "/src/lib/icons/dc.svg";
  import call from "/src/lib/icons/call.svg";
  import red from "/src/lib/icons/red.svg";
</script>

<main>
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
      <div class="connectTitle">
        <p><span class="brightColor">Thanks</span></p>
        <p>For Viewing My Site<span class="brightColor">.</span></p>
      </div>
      <div class="detailTitle">
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
        <div class="scatterAll">
          <div class="contactMain">
            <div class="compOne">
              <div class="imgAll">
                <img src={at} alt="" />
              </div>
              <div class="detailsFocus">
                <p>Call</p>
              </div>
            </div>
            <div class="compOne">
              <div class="imgAll">
                <img src={call} alt="" />
              </div>
              <div class="detailsFocus">
                <p>Call</p>
              </div>
            </div>
            <div class="compOne">
              <div class="imgAll">
                <img src={dis} alt="" />
              </div>
              <div class="detailsFocus">
                <p>Call</p>
              </div>
            </div>
            <div class="compOne">
              <div class="imgAll">
                <img src={red} alt="" />
              </div>
              <div class="detailsFocus">
                <p>Call</p>
              </div>
            </div>
          </div>
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
    height: 100px;
  }
  .detailTitle {
    width: 70%;
    font-size: 1.7vw;
    font-weight: 300;
    margin: 0 70px 0 0;
  }
  @media only screen and (max-width: 675px) {
    .abs {
      font-size: 2rem;
    }
  }
</style>
