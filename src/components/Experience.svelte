<section id="experience">
  <p class="header-text mb-5">work experience</p>

  <div class="block content has-text-left">
    <p class="is-size-5 has-text-weight-bold mb-0">
      Senior Software Engineer, Ethermed, Remote
    </p>
    <p class="is-size-6 orange">June 2024 - Present</p>
    <ul>
      <li><b><i>Skills and technologies:</i></b> Elixir, Phoenix, Python, RabbitMQ, Postgres, Docker, Kubernetes, Terraform, Terragrunt, HTML, CSS, Javascript, FHIR</li>
      <li><b>Led the development of a flagship AI-powered healthcare platform</b> to process medical prior authorizations, leveraging LLMs to provide approval probabilities and guideline matches&mdash;<b>delivering on critical deadlines that secured key client buy-in.</b></li>
      <li><b>Developed a scalable reprocessing system for AI validation</b> using RabbitMQ Streams, enabling prior authorizations to be rerun as AI models improved. This system established a foundation for continuous learning and refinement of AI decision-making models.<li>
      <li><b>Built a client-ready management and review portal</b> using Phoenix LiveView and JavaScript, providing medical professionals with real-time tracking of processed authorizations. This facilitated AI model feedback loops and improved system transparency.</li>
      <li><b>Enhanced security in the open-source Azurex library,</b> implementing managed identity authentication, a more secure alternative to the existing authentication method.</li>
    </ul>
  </div>

  <div class="block content has-text-left">
    <p class="is-size-5 has-text-weight-bold mb-0">
      Senior Software Engineer, WithBelay, Philadelphia, PA
    </p>
    <p class="is-size-6 orange">December 2021 - Mar 2024</p>
    <ul>
      <li><b><i>Skills and technologies:</i></b> Elixir, Phoenix, RabbitMQ, Postgres, Docker, Kubernetes, Terraform, HTML, CSS, JavaScript, Rust, Erlang</li>
      <li>Engineered <b>~41% of the frontend and backend codebase</b> due to management prioritizing my involvement in pair programming collaborative sessions that focused on critical code paths.</li>
      <li>Instrumental in <b>securing a seed round of over $5M in funding</b> through the development of robust backend systems, demonstrating the viability and potential of the product to investors.</li>
      <li><b>Independently spearheaded the implementation of critical features</b> including user authentication, automatic PDF and email generation, seamless user bank account access, secure ACH payment transfers, and cross-service observability, enhancing the user experience and operational efficiency.</li>
      <li><b>Led the development of a distributed micro-service</b> to stream data pertaining to <b>over 10K stocks and their option chains</b>, ensuring real-time data availability and accuracy for financial operations.</li>
      <li>Architected an abstraction layer to our market data within our system to facilitate backtesting our internal business logic and trading algorithms to ensure produce viability</li>
      <li>Solely designed and engineered an brokerage integration via API proxy to allow Alpaca-based brokerages to use Belay’s stock insurance services as a white-labelled product</li>
      <li>Expanded feature sets of <b>three critical Elixir open-source libraries</b> to align with company goals</li>
    </ul>
  </div>
</section>

<style lang="scss">
  @import "../assets/styles/global.scss";

  .header-text {
    font-size: 48px;
    width: 100%;
    border-bottom-width: 1px;
    border-bottom-color: black;
    border-bottom-style: solid;
    text-align: left;
  }

  .orange {
    color: $accent;
  }
</style>
