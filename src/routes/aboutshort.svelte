<script>
  import B from "../lib/images/b.jpeg";
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
        I am a fullstack web developer with passion of creating unique websites.
      </p>
      <p>
        I want to develop creative website while also providing a unique
        experience to users.
      </p>
      <p>
        Looking forward to work with a experienced team to gain my experience
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
    margin: 50px 0 0 0;
  }
  .brightColor {
    color: var(--bright-blue);
  }

  .firstPhoto {
    margin: 0 0 0 180px;
  }
  .secondDivDetails {
    width: 60%;
    margin: 0 12vw 0 0;
  }
  .secondDivDetails h1 {
    font-weight: 500;
  }
  .secondDivDetails p {
    font-size: 1.7vw;
    line-height: 30px;
  }
  .b {
    width: 100px;
    height: 100px;
    object-fit: cover;
    border-radius: 100%;
    filter: brightness(110%) saturate(80%);
  }
  .designBtn {
    background: none;
    color: #fff;
    border: none;
    margin: 20px 30px 0 0px;
    /* display: flex;
    align-items: center; */
    height: 30px;
    font-family: Outfit;
    font-weight: 500;
  }
  .designBtn a img {
    margin: 0 10px 0 0;
    transition: 0.2s;
  }
  .designBtn a {
    text-decoration: none;
    color: #fff;
    font-size: 1.5vw;
    transition: 0.2s;
  }
  .flex {
    display: flex;
    align-items: center;
  }
  .designBtn a:hover {
    color: var(--bright-blue);
  }
  .designBtn a:hover .btnBlue {
    filter: invert(0%) sepia(69%) saturate(6288%) hue-rotate(118deg)
      brightness(103%) contrast(102%);
    transform: translatex(5px);
  }

  @media only screen and (max-width: 675px) {
    .aboutMeInShort {
      display: block;
      margin: 50px 0 0 0;
      width: 100%;
    }
    .firstPhoto {
      margin: 20px;
    }
    .secondDivDetails {
      width: 100%;

      margin: 0 0 0 0;
    }
    .secondDivDetails h1 {
      margin: 0 0 0 20px;
    }
    .secondDivDetails p {
      font-size: 1.2rem;
      margin: 0 0 0 20px;
    }
    .flex {
      display: block;
      align-items: center;
    }
    .designBtn a {
      font-size: 1rem;
    }
  }
</style>
