<script>
  import { page } from "$app/stores";
  import "./styles.css";

  /**
   * @type {boolean}
   */
  let toggleNav;

  function topScroll() {
    window.scrollTo({
      top: 0,
      behavior: "smooth",
    });
  }
</script>

<header>
  <div class="positionAbsoluteHeader">
    <div class="myNameLogo">
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div class="imgLogo" on:click={topScroll}>
        <svg
          width="356"
          height="356"
          viewBox="0 0 356 356"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect
            x="47.1852"
            y="214"
            width="185"
            height="185"
            transform="rotate(-45 47.1852 214)"
            fill="#00F4F4"
            stroke="#00F4F4"
            stroke-width="15"
          />
          <rect
            x="28.3959"
            y="195.21"
            width="211.572"
            height="211.572"
            transform="rotate(-45 28.3959 195.21)"
            stroke="#00F4F4"
            stroke-width="15"
          />
          <rect
            x="10.8961"
            y="177.71"
            width="236.321"
            height="236.321"
            transform="rotate(-45 10.8961 177.71)"
            stroke="#00F4F4"
            stroke-width="15"
          />
          <path
            d="M121.962 223C122.382 223 122.772 222.58 123.132 221.74C123.552 220.9 123.762 219.52 123.762 217.6V174.4C123.762 172.48 123.552 171.13 123.132 170.35C122.712 169.51 122.292 169.06 121.872 169H151.392C156.492 169 160.602 169.75 163.722 171.25C166.902 172.69 169.242 174.79 170.742 177.55C172.242 180.25 172.992 183.49 172.992 187.27C172.992 191.11 172.242 194.44 170.742 197.26C169.242 200.02 166.902 202.15 163.722 203.65C160.602 205.09 156.492 205.81 151.392 205.81H137.622V217.6C137.622 219.52 137.832 220.9 138.252 221.74C138.672 222.58 139.092 223 139.512 223H121.962ZM141.312 195.91H145.812C149.352 195.91 152.082 195.61 154.002 195.01C155.982 194.41 157.362 193.48 158.142 192.22C158.922 190.96 159.312 189.31 159.312 187.27C159.312 185.29 158.892 183.7 158.052 182.5C157.272 181.3 155.952 180.46 154.092 179.98C152.292 179.44 149.832 179.17 146.712 179.17H141.312C139.452 179.17 138.372 179.29 138.072 179.53C137.772 179.71 137.622 180.4 137.622 181.6V193.39C137.622 194.59 137.772 195.31 138.072 195.55C138.372 195.79 139.452 195.91 141.312 195.91ZM180.671 223C181.091 223 181.511 222.58 181.931 221.74C182.351 220.9 182.561 219.52 182.561 217.6V174.4C182.561 172.48 182.351 171.13 181.931 170.35C181.511 169.51 181.091 169.06 180.671 169H214.331C219.011 169 222.671 169.54 225.311 170.62C227.951 171.7 229.811 173.26 230.891 175.3C231.971 177.28 232.511 179.62 232.511 182.32C232.511 184.48 232.121 186.31 231.341 187.81C230.621 189.25 229.691 190.39 228.551 191.23C227.411 192.07 226.271 192.7 225.131 193.12V193.3C229.031 194.2 231.971 195.82 233.951 198.16C235.931 200.44 236.921 203.5 236.921 207.34C236.921 209.92 236.411 212.41 235.391 214.81C234.371 217.21 232.481 219.19 229.721 220.75C227.021 222.25 223.091 223 217.931 223H180.671ZM200.021 213.01H213.521C216.941 213.01 219.371 212.53 220.811 211.57C222.311 210.55 223.061 208.93 223.061 206.71C223.061 204.61 222.251 202.99 220.631 201.85C219.011 200.65 216.341 200.05 212.621 200.05H200.111C198.311 200.05 197.231 200.17 196.871 200.41C196.571 200.65 196.421 201.46 196.421 202.84V210.31C196.421 211.63 196.571 212.41 196.871 212.65C197.231 212.89 198.281 213.01 200.021 213.01ZM200.111 190.87H210.731C213.611 190.87 215.651 190.39 216.851 189.43C218.111 188.41 218.741 186.91 218.741 184.93C218.741 182.95 218.141 181.48 216.941 180.52C215.801 179.56 213.761 179.08 210.821 179.08H200.021C198.221 179.08 197.171 179.2 196.871 179.44C196.571 179.62 196.421 180.4 196.421 181.78V188.17C196.421 189.49 196.571 190.27 196.871 190.51C197.231 190.75 198.311 190.87 200.111 190.87Z"
            fill="black"
          />
        </svg>
      </div>
      <!-- <h1>Bhavya<br />Panchal<span class="brightColor">.</span></h1> -->
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

      <a href="/connect"
        ><button
          class="btn items aria"
          aria-current={$page.url.pathname === "/connect" ? "page" : undefined}
          on:click={() => (toggleNav = !toggleNav)}>Connect</button
        ></a
      >
    </div>
  </div>
</header>

<style>
  .imgLogo {
    width: 60px;
    height: 60px;
    transition: 0.5s;
  }
  .imgLogo svg {
    width: 60px;
    height: 60px;
    cursor: pointer;
  }
  .imgLogo:hover {
    transform: rotateY(60deg) rotate(12deg);
  }
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
