<script>
  import "./styles.css";
</script>

<main>
  <div class="projectHead">
    <div class="projectTitleSecond">
      <p class="bolderTitle">
        Pr<span class="brightColor">o</span>jects<br />I Have Done<span
          class="brightColor">.</span
        >
      </p>
      <p class="inDetails">
        This is some side projects i have created as practical practice. This
        projects helped me understand the fundamental of frontend and backend
        side of web.
      </p>
    </div>
    <div class="projectFirst">
      <div class="parent">
        <div class="div1">Hi</div>
        <div class="div2">Bhavya</div>
        <div class="div3">PAnchal</div>
        <div class="div4">PAnchal</div>
        <div class="div5">PAnchal</div>
      </div>
    </div>
  </div>
</main>

<style>
  .projectHead {
    width: 95%;
    margin: 60px 30px 30px 20px;
    color: #fff;
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-between;
    font-family: Outfit;
  }
  .projectFirst {
    width: 80%;
  }
  .parent {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 1fr);
    grid-column-gap: 10px;
    grid-row-gap: 10px;
  }

  .parent div {
    width: 100%;
    height: 230px;
    background: linear-gradient(45deg, #f00, #f98);
    border-radius: 10px;
  }

  .div1 {
    grid-area: 1 / 1 / 2 / 2;
  }
  .div2 {
    grid-area: 1 / 2 / 2 / 3;
  }
  .div3 {
    grid-area: 1 / 3 / 2 / 4;
  }
  .div4 {
    grid-area: 2 / 1 / 3 / 2;
  }
  .div5 {
    grid-area: 2 / 2 / 3 / 3;
  }
  .projectTitleSecond {
    width: 25%;
    padding: 0 20px 20px 20px;
  }
  .bolderTitle {
    font-weight: 500;
    font-size: 2vw;
    margin: 0 0 20px 0;
  }
  .inDetails {
    line-height: 25px;
    font-weight: 300;
    font-size: 1.4vw;
  }
  @media only screen and (max-width: 675px) {
    .projectHead {
      width: 100%;
      display: block;
      margin: 400px 0 0 0;
    }
    .projectTitleSecond {
      width: 100%;
      font-size: 1rem;
    }
    .bolderTitle {
      font-weight: 500;
      font-size: 1.8rem;
      margin: 0 0 20px 10px;
    }
    .inDetails {
      line-height: 25px;
      font-weight: 300;
      font-size: 1.3rem;
      margin: 0 0 0 10px;
    }
    .projectFirst {
      width: 100%;
    }
    .parent {
      width: 100%;
      display: grid;
      grid-template-columns: 1fr;
      grid-template-rows: repeat(4, 1fr);
      grid-column-gap: 0px;
      grid-row-gap: 20px;
      margin: 0 0 0 20px;
    }
    .div1,
    .div2,
    .div3,
    .div4,
    .div5 {
      width: 100%;
      grid-area: auto;
    }
  }
</style>
