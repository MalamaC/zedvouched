<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ZedVouched</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet" />
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background-color: #fff9f3;
      color: #333;
    }

    header {
      background-color: #f27024;
      padding: 1rem 2rem;
      color: white;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    header h1 {
      margin: 0;
      font-size: 1.8rem;
    }

    nav {
      display: flex;
      gap: 1rem;
    }

    nav a {
      color: white;
      text-decoration: none;
      font-weight: 600;
      display: flex;
      align-items: center;
      gap: 0.4rem;
    }

    main {
      padding: 2rem;
    }

    .cta {
      background-color: #f9e6d5;
      padding: 1.5rem;
      border-radius: 10px;
      text-align: center;
      margin-bottom: 2rem;
    }

    .cta h2 {
      color: #f27024;
    }

    .cta a {
      display: inline-block;
      margin-top: 1rem;
      background-color: #f27024;
      color: white;
      padding: 0.75rem 1.5rem;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
    }

    .iframe-container {
      position: relative;
      overflow: hidden;
      padding-top: 56.25%;
    }

    iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: none;
    }

    .search-hero {
      background-color: #fff3e5;
      padding: 2rem 1rem;
      text-align: center;
      border-radius: 8px;
      margin-bottom: 2rem;
    }

    .search-hero h2 {
      font-size: 2rem;
      font-weight: bold;
      color: #4a4a4a;
    }

    .search-hero p {
      color: #666;
      margin-top: 0.5rem;
    }

    .search-hero form {
      margin-top: 1.5rem;
      max-width: 600px;
      margin-left: auto;
      margin-right: auto;
      display: flex;
    }

    .search-hero input[type="text"] {
      flex-grow: 1;
      padding: 0.75rem 1rem;
      border: 1px solid #ccc;
      border-radius: 0.375rem 0 0 0.375rem;
    }

    .search-hero button {
      background-color: #f27024;
      color: white;
      padding: 0.75rem 1.5rem;
      border: none;
      border-radius: 0 0.375rem 0.375rem 0;
      cursor: pointer;
    }

    .search-hero button:hover {
      background-color: #d65f1c;
    }

    .reviews-section {
      padding: 2rem 1rem;
      margin-top: 2rem;
      background-color: #f2f2f2;
      border-radius: 8px;
      max-width: 800px;
      margin-left: auto;
      margin-right: auto;
    }

    .reviews-section h3 {
      font-size: 1.5rem;
      font-weight: 600;
      color: #333;
      margin-bottom: 1rem;
    }

    .review {
      background-color: white;
      padding: 1rem;
      border-radius: 5px;
      margin-bottom: 1rem;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
    }

    .review-header {
      display: flex;
      justify-content: space-between;
      margin-bottom: 0.5rem;
      font-weight: 600;
    }

    .review-stars {
      color: #fbbf24;
    }

    footer {
      background-color: #f27024;
      color: white;
      padding: 1rem;
      text-align: center;
    }
  </style>
</head>
<body>
  <header>
    <h1>ZedVouched</h1>
    <nav>
      <a href="#map">Service Map</a>
      <a href="#form">Nominate</a>
      <a href="https://wa.me/260978109185" target="_blank"><i class="fab fa-whatsapp" style="color:#25D366;"></i> WhatsApp</a>
    </nav>
  </header>

  <main>
    <div class="search-hero">
      <h2>Your Map to Zambia's Trusted Service Providers</h2>
      <p>Search, nominate, and share trusted local workers and businesses</p>
      <form>
        <input type="text" placeholder="Search for barbers, tailors, welders...">
        <button type="submit">Search</button>
      </form>
      <p class="mt-3 text-sm text-gray-500">Help us fill this map with verified providers by nominating your trusted workers!</p>
    </div>

    <div class="cta">
      <h2>Help us fill this map with your trusted service providers</h2>
      <p>Nominate people you've worked with and vouch for!</p>
      <a href="#form">Nominate Now</a>
    </div>

    <section id="map">
      <h2>Service Provider Map</h2>
      <div class="iframe-container">
        <iframe src="https://www.google.com/maps/d/embed?mid=1LQXoxhIWpbgSo7cwGqGIzcfA8jWEMM4" allowfullscreen></iframe>
      </div>
    </section>

      <form class="custom-form" name="submit-to-google-sheet">
        <label for="name">Full Name</label>
        <input type="text" id="name" name="name" required />

        <label for="phone">Phone Number</label>
        <input type="tel" id="phone" name="phone" required />

        <label for="service">Type of Service</label>
        <input type="text" id="service" name="service" required />

        <label for="location">Location</label>
        <input type="text" id="location" name="location" required />

        <label for="comments">Why do you recommend them?</label>
        <textarea id="comments" name="comments" rows="4" required></textarea>

        <button type="submit">Submit Nomination</button>
      </form>
    </section>

    <section class="reviews-section">
      <h3>Ratings & Reviews</h3>
      <div class="review">
        <div class="review-header">
          <span>Chipo Banda - Tailor</span>
          <span class="review-stars">★★★★☆</span>
        </div>
        <p>Chipo delivers on time and her stitching is top-notch. Highly recommended in Chelstone!</p>
      </div>
      <div class="review">
        <div class="review-header">
          <span>James Mwila - Electrician</span>
          <span class="review-stars">★★★★★</span>
        </div>
        <p>Very reliable and always neat with his work. He fixed our power issue within the hour!</p>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 ZedVouched | Built with ❤️ in Zambia</p>
  </footer>
</body>
</html>
