

<head>
  <title>Mateus Gomes's Website</title>

  <!-- Bootstrap CSS -->
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css">

  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:ital,wght@0,400;0,700;1,400;1,700&display=swap" rel="stylesheet">

  <style>
    body {
      font-family: 'Roboto Mono', monospace;
      margin: 0;
    }

    .container {
      max-width: 800px;
      margin: 0 auto;
    }

    .bg-primary {
      background-color: ##004201;
      color: #fff;
    }

    .nav-link {
      color: #fff;
      text-decoration: none;
    }
  </style>

</head>

<body data-spy="scroll" data-target=".navbar" data-offset="50">

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-primary fixed-top">
    <div class="container">
      <a class="navbar-brand" href="#">Mateus Gomes</a>

      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a class="nav-link" href="#home">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#about">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#timeline">Timeline</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contact">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Home -->
  <section id="home" class="bg-primary py-5">
    <div class="container">
      <h1>Mateus Gomes</h1>
      <p class="lead">Software Engineer</p>
    </div>
  </section>

  <!-- About -->
  <section id="about" class="py-5">
    <div class="container">
      <h2>About Me</h2>
      <p>Experienced software engineer with over 7 years of experience developing customized solutions and MVPs for startups and enterprise clients. I specialize in front-end development using Angular, Typescript, and micro front-end architectures. On the back-end I focus on API first microservice architectures leveraging Java, Spring Boot, and AWS serverless.</p>
      <p>I believe expanding my knowledge is key for professional growth. I make time to regularly read technical books and test out the concepts I learn. For example, I'm a big fan of Robert C. Martin's ("Uncle Bob") teachings on clean code and solid design principles. I find his advice invaluable for writing maintainable, testable code.</p>
      <p>Career Highlights:</p>
      <ul>
        <li>Founded my own startup building MVPs for emerging companies across Brazil and the Dominican Republic. Gained hands-on experience bringing products to market.</li>
        <li>Worked on development of white label platform for major financial institution using Angular, Typescript, micro front-end principles. Implemented core back-end services with Java, Spring Boot.</li>
        <li>Built lambda microservices on AWS using Typescript, Postgres, and a test-driven approach. Integrated AWS infrastructure including SQS, CodePipeline.</li>
        <li>Implemented observability, testing, and deployment strategies for cloud-based applications. Experience with Terraform, Jitsi, and Grafana.</li>
        <li>Contributed across full stack improving stability and feature development. Leveraged Go, Node.js, Angular, and Reactive frameworks. Migrated codebases, optimized build processes.</li>
        <li>Passionate about continuously improving development practices through testing, monitoring, and modular architecture. Strong communication and collaboration skills.</li>
      </ul>
    </div>
  </section>
  <!-- Timeline -->
 <section id="timeline" class="py-5 bg-light"> <div class="container"> <h2>Timeline</h2> <div class="row"> <div class="col-md-6"> <div class="timeline-item">
        <span class="timeline-icon"><img src="https://clikbrasil.com.br/wp-content/uploads/2019/08/clik-1.png" width="80"></span>
        <h3 class="h5 mb-0">Clik Brasil</h3>

        <span class="small text-gray">2015 - 2020</span>
        <p>Founded my own web and mobile development company serving startups in Brazil and the Dominican Republic. Built interactive prototypes and MVPs using Java, JavaScript, React Native. Gained hands-on entrepreneurial experience taking products from idea to launch.</p>
      </div>
    </div>
    <div class="col-md-6">
      <div class="timeline-item">

        <span class="timeline-icon"><img src="https://is1-ssl.mzstatic.com/image/thumb/Purple114/v4/56/77/4d/56774df4-7e8a-cad4-b32a-642d570919e6/source/512x512bb.jpg" width="50"></span>
        <h3 class="h5 mb-0">sdbusiness</h3>

        <span class="small text-gray">2020 - 2021</span>
        <p>Developed and enhanced various components of a large enterprise web application using Angular, RxJs, and Bootstrap. Implemented a diagramming tool leveraging SVG and JavaScript for flexible representations.</p>
      </div>
    </div>
  </div>
  <hr>
  <div class="row">
    <div class="col-md-6">
      <div class="timeline-item">

        <span class="timeline-icon"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRb1Q2XKwsJRVwcalobLHJRkl4luClxjRLws8aUt1gqAnIbBrJrl9J0dDRwsQhOYzbDI6o&usqp=CAU" width="90"></span>
        <h3 class="h5 mb-0">konkerlabs</h3>

        <span class="small text-gray">2021 - 2021</span>
        <p>Architected and maintained an IoT platform using microservices written in Golang and Node.js. Deployed containerized services to AWS EKS. Built custom Grafana dashboards.</p>
      </div>
    </div>
    <div class="col-md-6">
      <div class="timeline-item">

        <span class="timeline-icon"><img src="data:image/png;base64,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" width="70"></span>
        <h3 class="h5 mb-0">Accenture</h3>

        <span class="small text-gray">2021 - 2023</span>
        <p>Worked on an Agile team responsible for ServiceNow implementations at large financial services clients. Developed workflows, custom services, and integrations.</p>
      </div>
    </div> 
  </div>
  <hr>
   <div class="row">
    <div class="col-md-6">
      <div class="timeline-item">

        <span class="timeline-icon"><img src="https://media.licdn.com/dms/image/C4D0BAQF1cWM6GMZ2sw/company-logo_200_200/0/1623068987405?e=1704931200&v=beta&t=615Z1jVju6uGmPA6hdkMObNUOnHqTK5hdx6P-5ibmhk" width="50"></span>
        <h3 class="h5 mb-0">Kintsu (Current)</h3>

        <span class="small text-gray">2023 - Present</span>
        <p>Develop and maintain a suite of TypeScript microservices and frontend applications using Angular, NestJS, and MongoDB. Implement CI/CD workflows, infrastructure as code with Terraform, and observability tooling.</p>
      </div>
    </div>
  </div>
  
</div>

</section>

  <!-- Contact -->
  <section id="contact" class="py-5">
    <div class="container">
      <h2>Contact</h2>
      <p>
        <a href="https://www.linkedin.com/in/mateusgms/" target="_blank">LinkedIn</a> |
        <a href="https://github.com/mateusgms" target="_blank">GitHub</a> |
        <a href="https://twitter.com/mateusgomes_dev" target="_blank">Twitter</a>
      </p>
    </div>
  </section>


  <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"></script>


  <script>
    $(document).ready(function() {
      $('body').scrollspy({
        target: ".navbar",
        offset: 50
      });
    });
  </script>
