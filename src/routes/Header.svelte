<script>
  import "./styles.css";
</script>

<header>
  <div class="positionAbsoluteHeader">
    <div class="myNameLogo">
      <h1>Bhavya<br />Panchal<span class="brightColor">.</span></h1>
    </div>

    <div class="navLinks">
      <a href="/"><button class="btn items">Home</button></a>
      <a href="/about"><button class="btn items">About Me</button></a>
      <a href="/myprojects"><button class="btn items">My Projects</button></a>
      <a href="/myprojects"><button class="btn items">Connect</button></a>
    </div>
  </div>
</header>

<style>
  header {
    color: #fff;
    font-family: Outfit;
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
</style>
