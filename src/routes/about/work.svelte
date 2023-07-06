<script>
  import lines from "/src/lib/images/lines.svg";
  import dot from "/src/lib/images/dot.svg";
</script>

<main>
  <div class="linesBlue">
    <div class="workTill">
      <p class="highLight">
        Work <span class="brightColor">&</span> Experience<span
          class="brightColor">.</span
        >
      </p>
      <p>
        This is where i work and gain experience in real life. Not found any
        technical job yet but doing an internship now.
      </p>
    </div>
    <div class="linesOfBlueness">
      <div class="componentOne">
        <img src={lines} alt="blue line" class="transform" />
        <div class="detail">
          <p class="highLight">
            Param Enterprise<span class="brightColor">.</span>
          </p>
          <p class="highLightDim">
            Stock Manager | Here i worked more than 2 years and i did management
            of the company stock and other works.
          </p>
          <p class="highLightDim italic">2020-2022</p>
        </div>
      </div>
      <div class="componentOne">
        <img src={dot} alt="blue line" class="transform" />
        <div class="detail">
          <p class="highLight">
            Perpetual Pharmaceuticals<span class="brightColor">.</span>
          </p>

          <p class="highLightDim">
            Office Manager | Currently i am working here and i manage the whole
            office by myself. Creating and parceling the order while also
            managing the stock.
          </p>
          <p class="highLightDim italic">2022 - Currently Working</p>
        </div>
      </div>
    </div>
  </div>
</main>

<style>
  .linesBlue {
    width: 100%;
    display: flex;
    height: 200px;
    justify-content: space-between;
    align-items: center;
    margin: 40px 0 0 0;
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
</style>
