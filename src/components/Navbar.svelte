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
      <a class="navbar-item" href="#info">
        info
      </a>
      <a class="navbar-item" href="#about">
        about
      </a>
      <a class="navbar-item" href="#experience">
        experience
      </a>
      <a class="navbar-item" href="#projects">
        projects
      </a>
    </div>
  </div>
  <div class="modal {active && 'is-active'}">
    <div class="modal-background" on:click={switchActive} />
    <div class="modal-content">
      <a href="#info" on:click={switchActive}>
        <p class="menu-option">info</p>
      </a>
      <a href="#about" on:click={switchActive}>
        <p class="menu-option">about</p>
      </a>
      <a href="#experience" on:click={switchActive}>
        <p class="menu-option">resume</p>
      </a>
      <a href="#contact" on:click={switchActive}>
        <p class="menu-option">contact</p>
      </a>
    </div>
    <button class="modal-close is-large" aria-label="close" on:click={switchActive}></button>
  </div>
</nav>


<style lang="scss">
  @import '../assets/styles/global.scss';

  .navbar {
    width: 50%;
    padding: 0rem 1rem;
  }

  @media only screen and (max-width: 1024px) {
    .navbar {
      width: 100%;
    }
  }

  .menu-option {
    color: white;
    width: 30%;
    margin: 2rem 0rem;
    text-align: center;
    padding-bottom: 0.5rem;
    border-bottom: 1px $accent solid;
    margin-left: auto;
    margin-right: auto;
  }
</style>