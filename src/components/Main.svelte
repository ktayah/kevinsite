<section>
  <h1 class="text big-font">I<span class="orange">’</span>m</h1>
  <h1 class="text big-font">Kevin Tayah<span class="orange">.</span></h1>
  <p class="text medium-font">Software Engineer</p>
  <p class="text"><span class="bold">Phone:</span> 267-546-7901</p>
  <p class="text"><span class="bold">Email:</span> kevintayah@gmail.com</p>
</section>

<style lang="scss">
  @import '../assets/styles/global.scss';
  
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
</style>