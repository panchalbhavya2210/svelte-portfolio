<script>
  import lines from "/src/lib/images/lines.svg";
  import dot from "/src/lib/images/dot.svg";
</script>

<main>
  <div class="schoolling">
    <div class="workTill">
      <p class="highLight">
        Schooling <span class="brightColor">&</span> Education<span
          class="brightColor">.</span
        >
      </p>
      <p>
        This is where i went to school, college and learned things i know today.
      </p>
    </div>
    <div class="linesOfBlueness">
      <div class="componentOne">
        <img src={lines} alt="blue line" class="transform" />
        <div class="detail">
          <p class="highLight">
            Akshar School<span class="brightColor">.</span>
          </p>
          <p class="highLightDim">
            HSC (Higher Secondary school Certificate) 12th Pass
          </p>
          <p class="highLightDim italic">2017</p>
        </div>
      </div>
      <div class="componentOne">
        <img src={lines} alt="blue line" class="transform" />
        <div class="detail">
          <p class="highLight">
            NV Patel College<span class="brightColor">.</span>
          </p>

          <p class="highLightDim">B.com (Drop Out 3rd Sem)</p>
          <p class="highLightDim italic">2019 - Currently Working</p>
        </div>
      </div>
      <div class="componentOne">
        <img src={lines} alt="blue line" class="transform" />
        <div class="detail">
          <p class="highLight">
            Mimo (Online Study)<span class="brightColor">.</span>
          </p>

          <p class="highLightDim">Learned HTML5, CSS3, JS From Mimo.</p>
          <p class="highLightDim italic">2020</p>
        </div>
      </div>
      <div class="componentOne">
        <img src={lines} alt="blue line" class="transform" />
        <div class="detail">
          <p class="highLight">
            Hasmukh Goswami College Of Engineering<span class="brightColor"
              >.</span
            >
          </p>

          <p class="highLightDim">BCA (5th Sem)</p>
          <p class="highLightDim italic">2021 - Ongoing Study</p>
        </div>
      </div>
      <div class="componentOne">
        <img src={dot} alt="blue line" class="transform" />
        <div class="detail">
          <p class="highLight">
            InfoLabz Technologies<span class="brightColor">.</span>
          </p>

          <p class="highLightDim">Internship + Training</p>
          <p class="highLightDim italic">2023</p>
        </div>
      </div>
    </div>
  </div>
</main>

<style>
  .schoolling {
    width: 100%;
    display: flex;
    align-items: flex-start;
    margin: 80px 0;
    height: 500px;
  }

  .linesOfBlueness {
    width: 75%;
    margin: 0 30px 0 0;
  }
  .componentOne {
    margin: -2px 0;
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
  }
  .detail {
    margin: -2px 0 0 10px;
  }
  .highLight {
    font-size: 2vw;
    font-weight: 400;
    margin: 0 0 5px 0;
  }
  .highLightDim {
    font-weight: 300;
    margin: 4px 0;
    color: #d0d0d0;
  }
  .transform {
    pointer-events: none;
  }
  .workTill {
    width: 25%;
    height: 200px;
    margin: 0 20px 0 30px;
    font-weight: 300;
  }
  .italic {
    font-style: italic;
    color: #c6c6c6;
  }
  @media only screen and (max-width: 675px) {
    .schoolling {
      display: none;
    }
  }
</style>
