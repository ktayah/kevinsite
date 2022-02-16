<script>
  import "bulma/css/bulma.scss";
  import Navbar from "./components/Navbar.svelte";
  import Info from "./components/Info.svelte";
  import About from "./components/About.svelte";
  import Skills from "./components/Skills.svelte";
  import Experience from "./components/Experience.svelte";
  import Education from "./components/Education.svelte";
  import Projects from "./components/Projects.svelte";

  let modalActive = true;

  function switchModalActive() {
    modalActive = !modalActive;
  }
</script>

<main class="has-navbar-fixed-top">
  <div class="columns is-desktop">
    <div class="column">
      <Navbar />
      <Info />
      <About />
      <Skills />
      <Experience />
      <Projects />
      <Education />
    </div>
    <div class="column is-hidden-touch">
      <div class="image" />
    </div>
  </div>
</main>

<style lang="scss">
  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }

  .image {
    position: fixed;
    bottom: 0;
    top: 0;
    right: 0;
    padding: 0;
    height: 100%;
    width: 50%;
    background-image: url("/static/images/me.png");
    background-size: cover;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
