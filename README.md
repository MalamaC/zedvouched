<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ZedVouched – Trusted Local Service Providers</title>
  <link
    href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap"
    rel="stylesheet"
  />
  <style>
    /* Base & Typography */
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: 'Inter', sans-serif;
      color: #333;
      background: #f9f9f9;
      line-height: 1.6;
    }
    a { text-decoration: none; }
    img { display: block; max-width: 100%; }

    /* Header */
    header {
      background: #006600;
      padding: 1rem 2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    header img { height: 40px; }
    nav ul {
      list-style: none;
      display: flex;
      gap: 1.5rem;
    }
    nav a {
      color: #fff;
      font-weight: 600;
      transition: opacity 0.2s;
    }
    nav a:hover { opacity: 0.8; }

    /* Hero */
    .hero {
      background: #004d00 url('images/hero-bg.jpg') center/cover no-repeat;
      color: #fff;
      text-align: center;
      padding: 6rem 1rem;
    }
    .hero h1 { font-size: 3rem; margin-bottom: 1rem; }
    .hero p {
      font-size: 1.125rem;
      max-width: 600px;
      margin: 0 auto 2rem;
    }
    .hero .cta {
      background: #ff8c00;
      color: #fff;
      padding: 0.75rem 2rem;
      border-radius: 5px;
      font-size: 1rem;
      font-weight: 600;
      transition: background 0.2s;
    }
    .hero .cta:hover { background: #e67600; }

    /* Sections */
    section {
      padding: 4rem 1rem;
      max-width: 1200px;
      margin: 0 auto;
    }
    .section-title {
      text-align: center;
      font-size: 2rem;
      margin-bottom: 2rem;
      color: #006600;
    }

    /* Card Grid */
    .card-grid {
      display: grid;
      gap: 1.5rem;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    }
    .card {
      background: #fff;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s;
    }
    .card:hover { transform: translateY(-5px); }
    .card img { height: 180px; object-fit: cover; }
    .card-content {
      padding: 1rem;
    }
    .card-content h3 {
      margin-bottom: 0.5rem;
      color: #006600;
      font-size: 1.25rem;
    }
    .card-content p { color: #555; font-size: 0.95rem; }

    /* Map Embed */
    .map-container {
      position: relative;
      width: 100%;
      padding-top: 56.25%; /* 16:9 aspect ratio */
    }
    .map-container iframe {
      position: absolute;
      top: 0; left: 0;
      width: 100%; height: 100%;
      border: 0;
    }

    /* Footer */
    footer {
      background: #333;
      color: #fff;
      text-align: center;
      padding: 2rem 1rem;
      font-size: 0.9rem;
    }
    footer a { color: #ff8c00; }
  </style>
</head>
<body>
  <header>
    <img src="images/zedvouched_logo.png" alt="ZedVouched Logo" />
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#map">Find a Provider</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <h1>Trusted Local Service Providers</h1>
    <p>Connecting you with verified professionals across Zambia. Quality service you can rely on, right in your community.</p>
    <a href="#services" class="cta">Explore Services</a>
  </section>

  <section id="services">
    <h2 class="section-title">Our Services</h2>
    <div class="card-grid">
      <div class="card">
        <img src="images/plumber.jpg" alt="Plumbing Service" />
        <div class="card-content">
          <h3>Plumbing</h3>
          <p>Expert plumbers for repairs, installations, and maintenance.</p>
        </div>
      </div>
      <div class="card">
        <img src="images/electrician.jpg" alt="Electrical Service" />
        <div class="card-content">
          <h3>Electrical</h3>
          <p>Professional electricians ensuring safe and efficient solutions.</p>
        </div>
      </div>
      <div class="card">
        <img src="images/carpentry.jpg" alt="Carpentry Service" />
        <div class="card-content">
          <h3>Carpentry</h3>
          <p>Skilled carpenters for customized woodwork and repairs.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="map">
    <h2 class="section-title">Find a Provider Near You</h2>
    <div class="map-container">
      <iframe
        src="https://www.google.com/maps/d/embed?mid=1LQXoxhIWpbgSo7cwGqGIzcfA8jWEMM4&ehbc=2E312F"
        width="640"
        height="480"
      ></iframe>
    </div>
  </section>

  <footer id="contact">
    <p>&copy; 2025 ZedVouched. All rights reserved.</p>
    <p>
      <a href="mailto:info@zedvouched.com">info@zedvouched.com</a>
    </p>
  </footer>
</body>
</html>
