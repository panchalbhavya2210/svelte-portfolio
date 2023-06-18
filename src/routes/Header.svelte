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
      <div
        class="aria"
        aria-current={$page.url.pathname === "/" ? "page" : undefined}
      >
        <a href="/"><button class="btn items">Home</button></a>
      </div>
      <a href="/about"><button class="btn items">About Me</button></a>
      <a href="/myprojects"><button class="btn items">My Projects</button></a>
      <a href="/myprojects"><button class="btn items">Connect</button></a>
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
  .aria {
    position: relative;
  }
  .aria[aria-current="page"]::before {
    --size: 6px;
    content: "";
    width: 0;
    height: 0;
    position: absolute;
    top: 0;
    left: calc(50% - 10px);
    border: 10px solid transparent;
    border-top: 10px solid #f00;
  }
</style>
