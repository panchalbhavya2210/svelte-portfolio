<script>
  import { page } from "$app/stores";
  import "./styles.css";
</script>

<header>
  <div class="positionAbsoluteHeader">
    <div class="myNameLogo">
      <h1>Bhavya<br />Panchal<span class="brightColor">.</span></h1>
    </div>

    <div class="navLinks">
      <a href="/"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/" ? "page" : undefined}
          >Home</button
        ></a
      >
      <a href="/about"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/about" ? "page" : undefined}
          >About Me</button
        ></a
      >
      <a href="/myprojects"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/myprojects"
            ? "page"
            : undefined}>My Projects</button
        ></a
      >
      <a href="/myprojects"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/contactme"
            ? "page"
            : undefined}>Connect</button
        ></a
      >
    </div>

    <div class="hamBurger">
      <div class="hamburgerDesign">
        <div class="barOne one" />
        <div class="barOne two" />
        <div class="barOne thi" />
      </div>
    </div>
  </div>
</header>

<style>
  header {
    width: 100%;
    position: fixed;
    color: #fff;
    font-family: Outfit;
    z-index: 555;
  }
  .brightColor {
    color: var(--bright-blue);
  }
  .myNameLogo {
    font-size: 1vw;
    margin: 0 0 0 30px;
  }
  .positionAbsoluteHeader {
    position: absolute;
    width: 100%;
    height: 80px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: #fff;
    background-color: #050f1ea5;
    backdrop-filter: blur(5px);
  }
  .navLinks {
    margin: 0 40px 0 0;
  }
  button {
    position: relative;
    margin: 0 40px 0 40px;
    background-color: var(--bright-blue);
    padding: 1vw;
    border: none;
    outline: none;
    cursor: pointer;
    font-family: Outfit;
    font-size: 1.2vw;
    border-radius: 30px;
    transition: 0.5s;
    border: 1px solid var(--body-color);
  }
  button:hover {
    /* background-color: var(--dim-blue); */
    color: #fff;
    border: 1px solid var(--bright-blue);
    background-color: var(--body-color);
  }

  .aria[aria-current="page"] {
    color: #fff;
    border: 1px solid var(--bright-blue);
    background-color: var(--body-color);
  }
  .hamBurger {
    display: none;
  }
  @media only screen and (max-width: 675px) {
    .navLinks {
      display: none;
    }
    .myNameLogo {
      font-size: 3vw;
      margin: 0 0 0 30px;
    }
    .hamBurger {
      display: block;
      width: 50px;
      height: 30px;
      margin: 0 20px 0 0;
    }
    .barOne {
      width: 40px;
      height: 2px;
      background-color: var(--bright-blue);
      margin: 8px auto;
      border-radius: 10px;
    }
  }
</style>
