<div class="page columns is-desktop is-multiline" id="info">
  <div class="page-info column">
    <h1 class="text big-font">I<span class="orange">&#8217;</span>m</h1>
    <h1 class="text big-font">Kevin Tayah<span class="orange">.</span></h1>
    <p class="text medium-font">Software Engineer</p>
    <p class="text"><span class="bold">Phone:</span> 267-546-7901</p>
    <p class="text"><span class="bold">Email:</span> kevintayah@gmail.com</p>

    <div class="my-5">
      <a
        class="link orange right-line pr-2"
        href="https://www.linkedin.com/in/ktayah/">LinkedIn</a>
      <a class="link orange pl-2" href="https://github.com/ktayah">GitHub</a>
    </div>
  </div>
  <div class="column is-hidden-touch">
    <div class="image"></div>
  </div>
</div>

<style lang="scss">
  @import "../assets/styles/global.scss";

  .text {
    text-align: left;
  }

  .big-font {
    font-size: 72px;
  }

  .medium-font {
    font-size: 30px;
  }

  @media only screen and (max-width: 768px) {
    .big-font {
      font-size: 48px;
    }

    .medium-font {
      font-size: 24px;
    }
  }

  .bold {
    font-weight: bold;
  }

  .orange {
    color: $accent;
  }

  .right-line {
    border-right: 1px black solid;
  }

  .image {
    padding: 0;
    margin: 0;
    height: 100vh;
    width: 100%;
    background-image: url("/static/images/me.png");
    background-size: cover;
  }
</style>
