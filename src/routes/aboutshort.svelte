<script>
  import aboutMe from "../lib/images/aboutme.svg";

  import "./styles.css";
</script>

<main>
  <div class="displayFlex">
    <div class="imgAbt">
      <img src={aboutMe} alt="about me logo" class="imgAbt" />
    </div>
    <div class="myDetailsInShort">
      <p>
        My name is Bhavya Panchal and I am a web developer with experience in
        frontend development, HTML, CSS, JavaScript, Firebase, React, Svelte and
        Git.
        <br /><br /> I have been working in the web development field for the
        past few years and have gained extensive knowledge and experience in
        various technologies.
        <br /><br /> I am passionate about creating user-friendly websites that are
        visually appealing and technically sound. With my expertise in modern web
        technologies such as React and Svelte, I am confident that I can provide
        the best solutions to any of your web development needs.
      </p>
    </div>
  </div>
</main>

<style>
  main {
    height: 100vh;
    font-family: Outfit;
  }
  .displayFlex {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 100vh;
  }
  .imgAbt {
    width: 40%;
    margin: 0 -180px 0 20px;
  }
  .myDetailsInShort {
    width: 70%;
    color: #fff;
    font-size: 2.1vw;
    margin: 0 50px 0 0;
    line-height: 40px;
  }
</style>
