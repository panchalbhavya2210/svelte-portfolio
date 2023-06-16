<script>
  import B from "../lib/images/b.jpeg";
  import "./styles.css";
</script>

<main>
  <div class="aboutMeInShort">
    <div class="firstPhoto">
      <img src={B} alt="" srcset="" class="b" />
    </div>

    <div class="secondDivDetails">
      <h1>Full-Stack<br />Developer<span class="brightColor">.</span></h1>
      <br />
      <p>
        I am a fullstack web developer. with passion of creating unique
        websites.
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
        <a href="/about">About ME</a>
      </button>
      <button class="designBtn">My Projects</button>
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
</style>
