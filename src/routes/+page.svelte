<script>
  import Hero from "./hero.svelte";
  import Aboutshort from "./aboutshort.svelte";
  import Shortprojects from "./shortprojects.svelte";
  import { blur } from "svelte/transition";
  import { fly } from "svelte/transition";
  import { quintOut } from "svelte/easing";
</script>

<!-- transition:blur={{ amount: 100 }} transition:fly={{
    delay: 250,
    duration: 500,
    x: 0,
    y: 100,
    opacity: 0,
    easing: quintOut,
  }} -->
<main
  transition:blur={{
    duration: 600,
    amount: 50,
  }}
>
  <Hero />
  <Aboutshort />
  <Shortprojects />
</main>
