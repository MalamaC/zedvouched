<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #FF6600;
      color: white;
    }

    .header {
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 40px 20px;
      background-color: #FF6600;
    }

    .header img {
      height: 300px;
      width: auto;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: #f9a769;
      padding: 15px 30px;
      border-radius: 45px;
    }

    .logo {
      height: 100px;
    }

    .nav-links {
      display: flex;
      gap: 15px;
    }

    .nav-links a, .dropdown {
      text-decoration: none;
      color: #1a1a4b;
      font-weight: 500;
      position: relative;
      cursor: pointer;
    }

    .dropdown-content {
      display: none;
      position: absolute;
      background-color: #f0f0f0;
      min-width: 160px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.2);
      z-index: 1;
    }

    .dropdown:hover .dropdown-content {
      display: block;
    }

    .dropdown-content a {
      color: #1a1a4b;
      padding: 12px 16px;
      text-decoration: none;
      display: block;
    }

    .search-bar {
      display: flex;
      justify-content: center;
      padding: 0 30px;
      margin: 20px 0;
    }

    .search-bar input {
      padding: 10px;
      flex: 1;
      border-radius: 20px 0 0 20px;
      border: none;
      outline: none;
    }

    .search-bar button {
      padding: 10px 20px;
      background-color: #edbb8a;
      color: black;
      border-radius: 0 20px 20px 0;
      border: none;
      cursor: pointer;
    }

    .cta-button {
      background-color: #25D366;
      color: black;
      padding: 8px 18px;
      border-radius: 20px;
      text-decoration: none;
      font-weight: 600;
    }

    .form-section {
      background-color: #ffffff10;
      padding: 40px 20px;
      margin: 20px;
      border-radius: 10px;
    }

    .form-section form {
      display: grid;
      gap: 20px;
      max-width: 500px;
      margin: auto;
    }

    .form-section input, .form-section textarea {
      padding: 12px;
      border-radius: 6px;
      border: none;
      font-size: 1em;
    }

    iframe {
      width: 100%;
      height: 300px;
      border: 0;
      margin-top: 30px;
    }

    .map-section {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 20px 30px;
    }

    .map-section h2 {
      font-size: 1.8em;
      font-weight: 600;
      color: white;
      margin: 0;
      width: 30%;
      padding-right: 20px;
    }

    .map-section iframe {
      width: 70%;
      height: 300px;
      border-radius: 10px;
      border: none;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #111;
      color: white;
    }
  </style>
</head>
<body>

  <div class="header">
    <img src="images/zedvouched_logo.png" alt="ZedVouched Logo">
  </div>

  <nav>
    <img class="logo" src="images/logo_only.png" alt="ZedVouched">
    <div class="nav-links">
      <div class="dropdown">Technical Services
        <div class="dropdown-content">
          <a href="#">Electrician</a>
          <a href="#">Plumber</a>
          <a href="#">Mechanic</a>
          <a href="#">Carpenter</a>
          <a href="#">Borehole Siting</a>
        </div>
      </div>
      <div class="dropdown">Design Services
        <div class="dropdown-content">
          <a href="#">Tailor</a>
          <a href="#">Graphic Designer</a>
          <a href="#">Architect</a>
          <a href="#">Hairdresser</a>
          <a href="#">Videographer</a>
        </div>
      </div>
      <div class="dropdown">Domestic & Support
        <div class="dropdown-content">
          <a href="#">Gardener</a>
          <a href="#">Maid</a>
          <a href="#">Chef</a>
          <a href="#">Nanny</a>
          <a href="#">Tutor</a>
        </div>
      </div>
      <div class="dropdown">Administrative
        <div class="dropdown-content">
          <a href="#">Legal Services</a>
          <a href="#">Taxation Agent</a>
          <a href="#">Web Designer</a>
          <a href="#">Resume Compiler</a>
        </div>
      </div>
      <div class="dropdown">Logistics
        <div class="dropdown-content">
          <a href="#">Driver</a>
          <a href="#">Courier Service</a>
        </div>
      </div>
    </div>
    <a class="cta-button" href="https://wa.me/260977000000" target="_blank">WhatsApp</a>
  </nav>

  <div class="search-bar">
    <input type="text" placeholder="Search local workers and businesses trusted and vouched for by Zambians..." />
    <button>Search</button>
  </div>

  <section class="form-section">
    <h2 style="text-align:center;">Help us map out verified providers by nominating your trusted workers</h2>
    <form>
      <input type="text" placeholder="Full Name" required/>
      <input type="servicetype" placeholder="Type of Service" required/>
      <input type="number" placeholder="Phone Number" required/>
      <input type="location" placeholder="Location (e.g. Lusaka, Kitwe)" required/>
      <input type="photo" placeholder="Attach photo of completed work if applicable" required/>
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit" style="background-color:#2e8b57;color:white;border:none;padding:10px;border-radius:20px;">Nominate</button>
    </form>
  </section>

  <div class="map-section">
    <h2>Your Map to Zambia's Trusted Service Providers</h2>
    <iframe 
      src="https://www.google.com/maps/d/embed?mid=1LQXoxhIWpbgSo7cwGqGIzcfA8jWEMM4&ehbc=2E312F" 
      allowfullscreen="" loading="lazy">
    </iframe>
  </div>

  <footer>
    &copy; 2025 ZedVouched | Built with ❤️ in Zambia
  </footer>

</body>
</html>
