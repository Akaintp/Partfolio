<script lang="ts">
  import About from "./pages/about.svelte";
  import Contact from "./pages/contact.svelte";
  import Portfolio from "./pages/portfolio.svelte";
  import Resume from "./pages/resume.svelte";
  import Services from "./pages/services.svelte";
</script>


<Router>
  <main>
    <header id="header">
      <div class="container">
        <h1><a href="index.html">Emily Jones</a></h1>
        <!-- Uncomment below if you prefer to use an image logo -->
        <!-- <a href="index.html" class="mr-auto"><img src="assets/img/logo.png" alt="" class="img-fluid"></a> -->
        <h2>I'm a passionate <span>graphic designer</span> from New York</h2>

        <!-- ======= Hero Section ======= -->
        <section id="hero" class="d-flex flex-column justify-content-center align-items-center">
          <div class="hero-container" data-aos="fade-in">
            <h1>Pulatov Temur</h1>
            <p>I'm <span class="typed" data-typed-items="Designer, Developer, Freelancer, Photographer"></span></p>
          </div>
        </section><!-- End Hero -->

        <nav id="navbar" class="navbar">
          <ul>
            <li><Link to="/" class="nav-link active">Home</Link></li>
            <li><Link to="/about" class="nav-link">About</Link></li>
            <li><Link to="/resume" class="nav-link">Resume</Link></li>
            <li><Link to="/services" class="nav-link">Services</Link></li>
            <li><Link to="/portfolio" class="nav-link">Portfolio</Link></li>
            <li><Link to="/contact" class="nav-link">Contact</Link></li>
          </ul>
          <i class="bi bi-list mobile-nav-toggle" />
        </nav>
        <!-- .navbar -->

        <div class="social-links">
          <!-- svelte-ignore a11y-invalid-attribute -->
          <a href="#" class="twitter"><i class="bi bi-twitter" /></a>
          <!-- svelte-ignore a11y-invalid-attribute -->
          <a href="#" class="facebook"><i class="bi bi-facebook" /></a>
          <!-- svelte-ignore a11y-invalid-attribute -->
          <a href="#" class="instagram"><i class="bi bi-instagram" /></a>
          <!-- svelte-ignore a11y-invalid-attribute -->
          <a href="#" class="linkedin"><i class="bi bi-linkedin" /></a>
        </div>
      </div>
      <Route path="/about" component={About} />
      <Route path="/resume" component={Resume} />
      <Route path="/services" component={Services} />
      <Route path="/portfolio" component={Portfolio} />
      <Route path="/contact" component={Contact} />
    </header>
  </main>
</Router>

