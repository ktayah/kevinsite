<script>
  import 'bulma/css/bulma.scss';
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
  <Navbar />
  <Info />
  <About />
  <Skills />
  <Experience />
  <Education />
  <Projects />
  <!-- Temporary code -->
  <div class="modal {modalActive && 'is-active'}">
    <div class="modal-background" on:click={switchModalActive} />
    <div class="modal-content">
      <div class="box mx-4">
        <p class="article my-3">
          Pardon my appearance, this website is still a work in-progress.
        </p>
        <button class="button is-light is-rounded " on:click={switchModalActive}
          >Okay</button
        >
      </div>
    </div>
    <button
      class="modal-close is-large"
      aria-label="close"
      on:click={switchModalActive}
    />
  </div>
</main>

<style lang="scss">
  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
