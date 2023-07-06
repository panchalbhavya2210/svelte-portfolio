<script>
  import { page } from "$app/stores";
  import "./styles.css";

  /**
   * @type {boolean}
   */
  let toggleNav;
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
      <a href="/connect"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/connect" ? "page" : undefined}
          >Connect</button
        ></a
      >
    </div>

    <button class="hamBurger" on:click={() => (toggleNav = !toggleNav)}>
      <div class="hamburgerDesign">
        <div class="barOne one" />
        <div class="barOne two" />
        <div class="barOne thi" />
      </div>
    </button>
  </div>

  <div id="toShow" class="{toggleNav ? 'toggleNav' : ''} navBlock">
    <div class="navBlockMain">
      <a href="/"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/" ? "page" : undefined}
          on:click={() => (toggleNav = !toggleNav)}>Home</button
        ></a
      >
      <br />
      <a href="/about"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/about" ? "page" : undefined}
          on:click={() => (toggleNav = !toggleNav)}>About Me</button
        ></a
      >
      <br />

      <a href="/myprojects"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/myprojects"
            ? "page"
            : undefined}
          on:click={() => (toggleNav = !toggleNav)}>My Projects</button
        ></a
      >
      <br />

      <a href="/myprojects"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/contactme"
            ? "page"
            : undefined}
          on:click={() => (toggleNav = !toggleNav)}>Connect</button
        ></a
      >
    </div>
  </div>
</header>

<style>
  .navBlock {
    display: none;
  }
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
    background-color: #010203b4;
    backdrop-filter: blur(5px);
    z-index: 555;
  }
  .navLinks {
    margin: 0 40px 0 0;
  }
  .btn {
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
    box-shadow: 0 0 5px var(--bright-blue);
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
      font-size: 2vw;
      margin: 0 0 0 30px;
    }
    .hamBurger {
      display: block;
      width: 50px;
      height: 40px;
      margin: 0 20px 0 0;
      z-index: 5555;
      background-color: #00000000;
      border: none;
      outline: none;
      border-radius: 2px;
    }

    .barOne {
      width: 40px;
      height: 2px;
      background-color: var(--bright-blue);
      margin: 8px auto;
      border-radius: 10px;
    }
    .navBlock {
      opacity: 0;
      pointer-events: none;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      position: fixed;
      width: 100%;
      height: 100%;
      background-color: var(--body-color);
      transition: 0.5s;
    }
    .toggleNav {
      opacity: 1;
      pointer-events: all;
    }
    .btn {
      width: 200px;
      font-size: 2rem;
      margin: 30px 0;
      border-radius: 10px;
      border: none;
      outline: none;
      background-color: var(--body-color);
      color: #fff;
    }
    .aria[aria-current="page"] {
      color: #fff;
      background-color: none;
      border: none;
      border-top: 2px solid var(--bright-blue);
      border-bottom: 2px solid var(--bright-blue);
      box-shadow: 0 0 0px var(--bright-blue);
    }
  }
</style>
