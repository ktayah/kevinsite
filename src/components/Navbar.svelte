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
    <div class="modal-background"></div>
    <div class="modal-content">
      <p class="white-text">about</p>
      <p class="white-text">resume</p>
      <p class="white-text">contact</p>
    </div>
    <button class="modal-close is-large" aria-label="close" on:click={switchActive}></button>
  </div>
</nav>


<style lang="scss">
  .navbar {
    width: 50%;
    padding: 0rem 1rem;
  }
  .white-text {
    color: white;
  }
</style>