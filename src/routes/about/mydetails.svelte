<script>
  import B from "/src/lib/images/my-image-removed-bg.png";
  import bigArrow from "/src/lib/icons/big-arrow.svg";
  import gitIcon from "/src/lib/icons/github.svg";
</script>

<main>
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
      <p class="titleO">
        Hello, I Am Bhavya<span class="brightColor">.</span>
      </p>
      <p class="myDetails">
        I am a 22-year-old front-end website developer from India. And I am
        learning the backend. Currently, I am in college, doing the 5th semester
        of the BCA (Bachelor of Computer Application) Course at Monark
        University. I started programming as a hobby. I got into programming in
        lockdown and started learning it from the Mimo app and various YouTube
        channels.
        <br /><br />
        Beside working part-time at a pharmacy and doing college, I created some
        side projects that gave me a lot of experience. And I am also eager to learn
        new things. I have learned a lot from practicals.
      </p>
      <p class="titleO">
        Coding Journey<span class="brightColor">.</span>
      </p>
      <p class="myDetails">
        I started learning front-end website development in 2020. I did most of
        the learning from the Mimo App and YouTube Videos. After learning the
        basics, I got into creating various projects. I created some basic
        projects and improved them over time. I started coding on my phone, and
        I created various projects using the SPCK editor.
        <br /><br />
        After coding in mobile for a long time. I bought a laptop and started coding
        on it. I mostly use Visual Studio Code for programming. I am still learning
        the basics of the backend so I can become a full-stack developer.
      </p>
    </div>
  </div>
</main>

<style>
  .lengthMyAbt {
    margin: 50px 0;
  }
  .b {
    width: 70%;
    height: 70%;
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
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .myImgLinks {
    height: 300px;
    margin: 0 0 0 5%;
  }
  .aboutMe {
    width: 65%;
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
  @media only screen and (max-width: 675px) {
    .lengthMyAbt {
      display: block;
    }
    .b {
      width: 100px;
      height: 100px;
      margin: 0 0 10px 0;
    }
    .myImgLinks {
      height: 230px;
      margin: 60px 0 0 30px;
    }
    .titleO {
      font-size: 1.5rem;
      font-weight: 500;
      margin: 0 0 10px 0;
    }
    .aboutMe {
      width: 90%;
      margin: 0 0px 0 30px;
    }
    .myDetails {
      font-size: 1rem;
      font-weight: 300;
      margin: 0 0 30px 0;
      /* line-height: 28px; */
    }
  }
</style>
