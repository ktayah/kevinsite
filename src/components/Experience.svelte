<section id="experience">
  <p class="header-text mb-5">work experience</p>

  <div class="block content has-text-left">
    <p class="is-size-5 has-text-weight-bold mb-0">
      Lead Software Engineer, Ethermed, Remote
    </p>
    <p class="is-size-6 orange">June 2024 - Present</p>
    <ul>
      <li><b><i>Skills and technologies:</i></b> Elixir, Phoenix LiveView, Python, Postgres, RabbitMQ, Docker, Kubernetes, Terraform, Terragrunt, HTML, CSS, Javascript, Azure, OpenAI, Anthropic, FHIR</li>
      <li><b>Led development and technical direction of an AI-powered medical prior authorization platform used by 10+ clients,</b> automating medical policy search and approval probability across a pool of <b>270k medical policies.</b></li>
      <li><b>Architected and built AI-powered medical policy scraping, extraction, and normalization systems,</b> and established reusable engineering patterns that enabled parallel development across the team allowing the platform to scale up to ~270k policies and meet multiple client integration deadlines.</li>
      <li><b>Owned the medical policy matching and retrieval systems, improving matching accuracy by ~75%</b> through iterative improvements to retrieval, ranking, and evaluation pipelines using production data and benchmarking.</li>
      <li><b>Reduced LLM usage costs by 50%</b> by designing reusable processing workflows and batch processing patterns using Anthropic batch APIs for large-scale document extraction.</li>
      <li><b>Designed and delivered internal self-service tooling</b> that allowed client integration specialists to manage policy matching logic, onboarded new clients, and adapt to diverse client data formats that ensured integration delivery.</li>
      <li><b>Developed a scalable reprocessing system for AI validation</b> using RabbitMQ Streams, enabling prior authorizations to be rerun as AI models improved. This system established a foundation for continuous learning and refinement of AI decision-making models.</li>
      <li><b>Built a client-ready management and review portal</b> using Phoenix LiveView and JavaScript, providing medical professionals with real-time tracking of processed authorizations. This facilitated AI model feedback loops and improved system transparency.</li>
      <li><b>Mentored engineers</b> through design reviews, pair programming, and code reviews, and <b>helped grow the engineering team from 2 to 10 engineers</b> through interviewing and onboarding.</li>
      <li>Collaborated with product managers, client integration teams, and external clients to define requirements, resolve integration challenges, and guide technical implementation decisions.</li>
      <li>Worked with DevOps to design and manage infrastructure and deployments using Terraform and Azure infrastructure, and <b>owned the deployment process through staging and production</b> until stabilization.</li>
      <li><b>Contributed security improvements to the open-source Azurex library</b> by implementing managed identity authentication.</li>
    </ul>
  </div>

  <div class="block content has-text-left">
    <p class="is-size-5 has-text-weight-bold mb-0">
      Senior Software Engineer, WithBelay, Philadelphia, PA
    </p>
    <p class="is-size-6 orange">December 2021 - May 2024</p>
    <ul>
      <li><b><i>Skills and technologies:</i></b> Elixir, Phoenix, RabbitMQ, Postgres, Docker, Kubernetes, Terraform, HTML, CSS, JavaScript, Rust, Erlang</li>
      <li>Engineered <b>~41% of the frontend and backend codebase</b> due to management prioritizing my involvement in pair programming collaborative sessions that focused on critical code paths.</li>
      <li>Instrumental in <b>securing a seed round of ~$5M in funding</b> through the development of robust backend systems, demonstrating the viability and potential of the product to investors.</li>
      <li><b>Independently spearheaded the implementation and owned critical features</b> including user authentication, automatic PDF and email generation, seamless user bank account access, secure ACH payment transfers, and cross-service observability, enhancing the user experience and operational efficiency.</li>
      <li><b>Led the development of a high-performance distributed micro-service</b> which leveraged Elixir to track and stream data pertaining to <b>over 10K stocks and their option chains</b>, ensuring real-time data availability and accuracy for financial operations.</li>
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
