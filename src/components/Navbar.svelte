<script>
  let active = false;

  function switchActive() {
    active = !active;
  }

  function openCV() {
    const keys = {
      localhost: "802af1cccde747acbd720bef2460d02d",
      "ktayah.com": "eeec26b559a3462ea4e19799913d22d4",
      "kevintayah.com": "1c2403d943354eb58cc423ddf4952376",
    };

    const adobeDCView = new AdobeDC.View({
      clientId: keys[window.location.hostname],
    });

    adobeDCView.previewFile(
      {
        content: { location: { url: "static/pdf/resume.pdf" } },
        metaData: {
          fileName: "Kevin's Resume.pdf",
        },
      },
      {
        embedMode: "LIGHT_BOX",
        defaultViewMode: "FIT_PAGE",
      }
    );
  }

  // Wait will adobe pdf viewer is ready to enable CV button
  document.addEventListener("adobe_dc_view_sdk.ready", function () {
    document.getElementById("view-pdf-btn").disabled = false;
  });
</script>

<nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" on:click={openCV} id="view-pdf-btn" disabled>CV</a>

    <span
      role="button"
      class="navbar-burger"
      aria-label="menu"
      aria-expanded="false"
      data-target="navbarBasicExample"
      on:click={switchActive}
    >
      <span aria-hidden="true" />
      <span aria-hidden="true" />
      <span aria-hidden="true" />
    </span>
  </div>

  <div class="navbar-menu">
    <div class="navbar-end">
      <a class="navbar-item" href="#info"> info </a>
      <a class="navbar-item" href="#about"> about </a>
      <a class="navbar-item" href="#experience"> experience </a>
      <a class="navbar-item" href="#projects"> projects </a>
    </div>
  </div>
  <div class="modal {active && 'is-active'}">
    <div class="modal-background" on:click={switchActive} />
    <div
      class="modal-content is-flex is-flex-direction-column is-justify-content-space-around"
    >
      <div>
        <a href="#info" on:click={switchActive}>
          <span class="menu-option">info</span>
        </a>
      </div>
      <div>
        <a href="#about" on:click={switchActive}>
          <span class="menu-option">about</span>
        </a>
      </div>
      <div>
        <a href="#experience" on:click={switchActive}>
          <span class="menu-option">resume</span>
        </a>
      </div>
      <div>
        <a href="#contact" on:click={switchActive}>
          <span class="menu-option">contact</span>
        </a>
      </div>
    </div>
    <button
      class="modal-close is-large"
      aria-label="close"
      on:click={switchActive}
    />
  </div>
</nav>

<style lang="scss">
  @import "../assets/styles/global.scss";

  .navbar {
    width: 50%;
    padding: 0rem 1rem;
  }

  @media only screen and (max-width: 1024px) {
    .navbar {
      width: 100%;
    }
  }

  .modal-content {
    height: 50vh;
  }

  .menu-option {
    color: white;
    margin: 2rem 0rem;
    text-align: center;
    padding-bottom: 0.5rem;
    border-bottom: 1px $accent solid;
  }
</style>
