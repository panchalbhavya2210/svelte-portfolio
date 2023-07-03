<script>
  import "../styles.css";
  import blueLine from "/src/lib/images/about-me-blob.svg";
  import B from "/src/lib/images/my-image-removed-bg.png";
  import bigArrow from "/src/lib/icons/big-arrow.svg";
  import gitIcon from "/src/lib/icons/github.svg";
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
              >fullstack website developer from India.</span
            >
            Currently i am in college doing 5th semester of BCA(Bachelor Of Computer
            Application) Course at Monark University. I sta

            <br /><br />
            Besides working full time, I also have a few open source projects that
            can be found on my work page. My most recent project is called Meteocons,
            a free-to use set of animated weather icons.
          </p>
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
    /* line-height: 28px; */
  }
</style>
