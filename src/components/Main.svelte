<div class="main">
  <h1 class="t">I<span class="orange">'</span>m</h1>
  <h1 class="t">Kevin Tayah<span class="orange">.</span></h1>
  <h2 class="st">Senior Full Stack Developer</h2>
  <p><span class="bold">Phone:</span> 267-546-7901</p>
  <p><span class="bold">Email:</span> kevintayah@gmail.com</p>
  <p><span class="bold">Address:</span> 2428 Poplar St, Philadelphia PA</p>
</div>

<style lang="scss">
  @import '../assets/styles/global.scss';

  .main {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    height: 100%;
  }

  .t {
    font-size: 72px;
  }

  .st {
    font-size: 30px;
  }

  .bold {
    font-weight: bold;
  }

  .orange {
    color: $accent;
  }
</style>