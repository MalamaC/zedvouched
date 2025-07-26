<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ZedVouched</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --clr-primary: #FF6600;
      --clr-primary-dark: #e65500;
      --clr-secondary: #25D366;
      --clr-secondary-dark: #21b95c;
      --clr-bg: #f5f5f5;
      --clr-card: #ffffff;
      --clr-text: #222222;
      --clr-nav-bg: #ffffff;
      --shadow: 0 4px 16px rgba(0, 0, 0, 0.1);
      --radius: 12px;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: var(--clr-bg);
      color: var(--clr-text);
      line-height: 1.6;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 1rem;
    }

    header.site-header {
      background: var(--clr-nav-bg);
      box-shadow: var(--shadow);
    }

    header.site-header .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 0;
    }

    .logo {
      height: 60px;
    }

    nav {
      display: flex;
      align-items: center;
      gap: 1.5rem;
      position: relative;
    }

    nav a {
      text-decoration: none;
      color: var(--clr-text);
      font-weight: 500;
      padding: 0.5rem 0;
      transition: color 0.3s;
    }

    nav a:hover {
      color: var(--clr-primary);
    }

    .dropdown {
      position: relative;
    }

    .dropdown-menu {
      position: absolute;
      top: 100%;
      left: 0;
      background: var(--clr-card);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      opacity: 0;
      visibility: hidden;
      transform: translateY(10px);
      transition: all 0.3s;
      min-width: 180px;
      z-index: 10;
    }

    .dropdown:hover .dropdown-menu {
      opacity: 1;
      visibility: visible;
      transform: translateY(0);
    }

    .dropdown-menu a {
      display: block;
      padding: 0.75rem 1rem;
      color: var(--clr-text);
    }

    .dropdown-menu a:hover {
      background: var(--clr-bg);
    }

    .cta-button {
      background: var(--clr-secondary);
      color: #fff;
      padding: 0.5rem 1.25rem;
      border: none;
      border-radius: var(--radius);
      text-decoration: none;
      font-weight: 600;
      box-shadow: var(--shadow);
      transition: background 0.3s;
    }

    .cta-button:hover {
      background: var(--clr-secondary-dark);
    }

    .search-section {
      padding: 2rem 0;
    }

    .search-bar {
      display: flex;
      max-width: 600px;
      margin: 0 auto;
      box-shadow: var(--shadow);
      border-radius: var(--radius);
      overflow: hidden;
    }

    .search-bar input {
      flex: 1;
      padding: 1rem;
      border: none;
      outline: none;
    }

    .search-bar button {
      background: var(--clr-primary);
      border: none;
      padding: 1rem 1.5rem;
      color: #fff;
      cursor: pointer;
      transition: background 0.3s;
    }

    .search-bar button:hover {
      background: var(--clr-primary-dark);
    }

    .card {
      background: var(--clr-card);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 2rem;
      margin-bottom: 2rem;
    }

    .form-section .card {
      display: grid;
      grid-template-columns: 1fr 2fr;
      gap: 2rem;
      align-items: start;
    }

    .form-section h2 {
      font-size: 1.75rem;
      margin: 0;
      color: var(--clr-text);
    }

    .form-section form {
      display: grid;
      gap: 1rem;
    }

    .form-section input,
    .form-section textarea {
      width: 100%;
      padding: 0.75rem;
      border: 1px solid #ddd;
      border-radius: var(--radius);
      font-family: inherit;
    }

    .form-section button {
      background: var(--clr-primary);
      color: #fff;
      padding: 0.75rem;
      border: none;
      border-radius: var(--radius);
      cursor: pointer;
      font-size: 1rem;
      transition: background 0.3s;
    }

    .form-section button:hover {
      background: var(--clr-primary-dark);
    }

    .map-section .card {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    .map-section h2 {
      margin: 0;
      font-size: 1.75rem;
      color: var(--clr-text);
    }

    .map-section iframe {
      width: 100%;
      height: 350px;
      border: none;
      border-radius: var(--radius);
    }

    footer {
      text-align: center;
      padding: 1.5rem 0;
      background: #222;
      color: #fff;
    }
  </style>
</head>
<body>

  <header class="site-header">
    <div class="container">
      <img src="images/zedvouched_logo.png" alt="ZedVouched Logo" class="logo">
      <nav>
        <div class="dropdown">
          <a href="#">Technical Services</a>
          <div class="dropdown-menu">
            <a href="#">Electrician</a>
            <a href="#">Plumber</a>
            <a href="#">Mechanic</a>
            <a href="#">Carpenter</a>
            <a href="#">Borehole Siting</a>
          </div>
        </div>
        <div class="dropdown">
          <a href="#">Design Services</a>
          <div class="dropdown-menu">
            <a href="#">Tailor</a>
            <a href="#">Graphic Designer</a>
            <a href="#">Architect</a>
            <a href="#">Hairdresser</a>
            <a href="#">Videographer</a>
          </div>
        </div>
        <div class="dropdown">
          <a href="#">Domestic &amp; Support</a>
          <div class="dropdown-menu">
            <a href="#">Gardener</a>
            <a href="#">Maid</a>
            <a href="#">Chef</a>
            <a href="#">Nanny</a>
            <a href="#">Tutor</a>
          </div>
        </div>
        <div class="dropdown">
          <a href="#">Administrative</a>
          <div class="dropdown-menu">
            <a href="#">Legal Services</a>
            <a href="#">Taxation Agent</a>
            <a href="#">Web Designer</a>
            <a href="#">Resume Compiler</a>
          </div>
        </div>
        <div class="dropdown">
          <a href="#">Logistics</a>
          <div class="dropdown-menu">
            <a href="#">Driver</a>
            <a href="#">Courier Service</a>
          </div>
        </div>
        <a class="cta-button" href="https://wa.me/260977000000" target="_blank">WhatsApp Us</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="search-section">
      <div class="container">
        <div class="search-bar">
          <input type="text" placeholder="Search trusted local experts…" />
          <button>Search</button>
        </div>
      </div>
    </section>

    <section class="form-section">
      <div class="container card">
        <h2>Let's fill the Zambian map, together</h2>
        <form>
          <input type="text" placeholder="Full Name" required />
          <input type="text" placeholder="Type of Service" required />
          <input type="tel" placeholder="Phone Number" required />
          <input type="text" placeholder="Location (e.g. Lusaka, Kitwe)" required />
          <input type="file" placeholder="Attach photo of completed work" />
          <textarea rows="5" placeholder="Your Message" required></textarea>
          <button type="submit">Nominate</button>
        </form>
      </div>
    </section>

    <section class="map-section">
      <div class="container card">
        <h2>Your Map to Zambia's Trusted Service Providers</h2>
        <iframe
          src="https://www.google.com/maps/d/embed?mid=1LQXoxhIWpbgSo7cwGqGIzcfA8jWEMM4&ehbc=2E312F"
          allowfullscreen=""
          loading="lazy">
        </iframe>
      </div>
    </section>
  </main>

  <footer>
    &copy; 2025 ZedVouched | Built with ❤️ in Zambia
  </footer>

</body>
</html>
