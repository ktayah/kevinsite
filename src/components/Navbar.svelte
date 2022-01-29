<script>
  let active = false;

  function switchActive() {
    active = !active;
  }
</script>

<nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item">CV</a>

    <span
      role="button" 
      class="navbar-burger" 
      aria-label="menu" 
      aria-expanded="false" 
      data-target="navbarBasicExample" 
      on:click={switchActive}>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </span>
  </div>

  <div class="navbar-menu">
    <div class="navbar-end">
      <a class="navbar-item" href="#about">
        about
      </a>
      <a class="navbar-item" href="#experience">
        resume
      </a>
      <a class="navbar-item" href="#contact">
        contact
      </a>
    </div>
  </div>
  <div class="modal {active && 'is-active'}">
    <div class="modal-background" on:click={switchActive} />
    <div class="modal-content">
      <a href="#about" on:click={switchActive}>
        <p class="white-text">about</p>
      </a>
      <a href="#experience" on:click={switchActive}>
        <p class="white-text">resume</p>
      </a>
      <a href="#contact" on:click={switchActive}>
        <p class="white-text">contact</p>
      </a>
    </div>
    <button class="modal-close is-large" aria-label="close" on:click={switchActive}></button>
  </div>
</nav>


<style lang="scss">
  .navbar {
    width: 50%;
    padding: 0rem 1rem;
  }

  @media only screen and (max-width: 768px) {
    .navbar {
      width: 100%;
    }
  }
  .white-text {
    color: white;
  }
</style>