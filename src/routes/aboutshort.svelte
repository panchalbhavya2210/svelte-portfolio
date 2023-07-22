<script>
  import B from "../lib/images/my-image-removed-bg.png";
  import "./styles.css";
  import bigArrow from "../lib/icons/big-arrow.svg";
</script>

<main>
  <div class="aboutMeInShort">
    <div class="firstPhoto">
      <img src={B} alt="" srcset="" class="b" />
    </div>

    <div class="secondDivDetails">
      <h1>
        Full-Stack<span class="brightColor"> &nbsp;// </span>Developer<span
          class="brightColor">.</span
        >
      </h1>
      <br />
      <p>
        I am a full-stack web developer with a passion for creating unique
        websites.
      </p>
      <br />

      <p>
        I want to develop a creative website while also providing a unique
        experience to users.
      </p>
      <br />

      <p>
        I look forward to working with an experienced team to gain experience
        too.
      </p>

      <button class="designBtn">
        <a class="flex" href="/about">
          <img src={bigArrow} alt="right-arrow" class="btnBlue" />
          <span>About Me</span>
        </a>
      </button>
      <button class="designBtn">
        <a class="flex" href="/myprojects">
          <img src={bigArrow} alt="right-arrow" class="btnBlue" />
          <span>My Projects</span>
        </a>
      </button>
    </div>
  </div>
</main>

<style>
  .aboutMeInShort {
    font-family: Outfit;
    color: #fff;
    font-weight: 300;
    width: 100%;
    height: 300px;
    display: flex;
    justify-content: space-between;
    margin: 100px 0 0 0;
  }
  .brightColor {
    color: var(--bright-blue);
  }

  .firstPhoto {
    margin: 0 0 0 120px;
  }
  .secondDivDetails {
    width: 60%;
    margin: 0 12% 0 0;
  }
  .secondDivDetails h1 {
    font-weight: 500;
  }
  .secondDivDetails p {
    font-size: 1.7vw;
    line-height: 30px;
  }
  .b {
    width: 130px;
    height: 130px;
    object-fit: cover;
    border-radius: 100%;
    filter: brightness(95%) saturate(100%);
    pointer-events: none;
    background: linear-gradient(-45deg, rgb(1, 49, 55), rgb(11, 0, 137));
    pointer-events: none;
  }

  @media only screen and (max-width: 675px) {
    .aboutMeInShort {
      display: block;
      margin: 100px 0 0 0;
      width: 100%;
    }
    .firstPhoto {
      margin: 30px;
    }
    .b {
      border-radius: 30px 30px;
    }
    .secondDivDetails {
      width: 100%;

      margin: 0px 0 0 0;
    }
    .secondDivDetails h1 {
      margin: 0 0 0 30px;
    }
    .secondDivDetails p {
      font-size: 1.3rem;
      margin: 0 0 0 30px;
    }
    .flex {
      display: flex;
      align-items: center;
    }
    .designBtn a span {
      font-size: 1.2rem;
    }
    .designBtn {
      display: flex;
      margin: 30px;
    }
  }
</style>
