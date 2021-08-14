<script>
  let active = false;

  function switchActive() {
    active = !active;
  }
</script>

<div>
<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item">CV</a>

    <a 
      role="button" 
      class="navbar-burger" 
      aria-label="menu" 
      aria-expanded="false" 
      data-target="navbarBasicExample" 
      on:click={switchActive}>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div class="navbar-menu">
    <div class="navbar-end">
      <a class="navbar-item">
        about
      </a>

      <a class="navbar-item">
        resume
      </a>

      <a class="navbar-item">
        contact
      </a>
    </div>
  </div>
  <div class="modal {active && 'is-active'}">
    <div class="modal-background"></div>
    <div class="modal-content">
      <p>Testing</p>
    </div>
    <button class="modal-close is-large" aria-label="close" on:click={switchActive}></button>
  </div>
</nav>
</div>


<!-- <style lang="scss">
  // @import "../assets/styles/global.scss";

}
</style> -->