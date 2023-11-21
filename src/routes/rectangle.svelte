<script defer>
  // @ts-nocheck
  export let src;
  export let languageName;
  export let alt;
  import { onMount } from "svelte";

  import "./styles.css";

  onMount(() => {
    let grabElement = document.querySelectorAll(".rect");

    const mouseMove = (e) => {
      const { currentTarget: target } = e;
      const rect = target.getBoundingClientRect(),
        x = e.clientX - rect.left,
        y = e.clientY - rect.top;

      target.style.setProperty("--mouse-x", `${x}px`);
      target.style.setProperty("--mouse-y", `${y}px`);
    };

    for (const rectGrad of grabElement) {
      rectGrad.onmousemove = (e) => mouseMove(e);
    }
  });
</script>

<main>
  <div class="rect">
    <div class="flexMain">
      <img {src} {alt} srcset="" class="img" />
      <p class="bottomTxt">{languageName}</p>
    </div>
  </div>
</main>

<style>
  .rect {
    position: relative;
    width: 80%;
    height: 130%;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: rgba(0, 26, 81, 0.215);
    border: 0.5px solid rgba(0, 12, 48, 1);
    border-radius: 5px;
    cursor: default;
  }

  .rect:hover::before {
    opacity: 1;
  }
  .rect::before {
    position: absolute;
    content: "";
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: inherit;
    z-index: -2;
    opacity: 0;
    transition: opacity 500ms;
    background: radial-gradient(
      400px circle at var(--mouse-x) var(--mouse-y),
      rgba(145, 222, 255, 0.54),
      transparent 40%
    );
  }

  .flexMain {
    width: 100%;
    text-align: center;
  }
  .img {
    width: 20%;
    height: 20%;
    margin: 0 0 20px 0;
    pointer-events: none;
  }
  @media only screen and (max-width: 675px) {
    .rect {
      width: 150px;
      height: 120px;
    }
  }
</style>
