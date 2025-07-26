<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>[ZedVouched Platform]</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #FF6600;
      color: white;
    }

    header {
      text-align: center;
      padding: 40px 20px;
    }

    header h1 {
      font-size: 3em;
      margin-bottom: 10px;
    }

    header p {
      font-size: 1.3em;
      opacity: 0.9;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: white;
      padding: 15px 30px;
    }

    .logo {
      font-size: 1.5em;
      font-weight: bold;
      color: #1a1a4b;
    }

    .nav-links {
      display: flex;
      gap: 20px;
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
      margin: 20px auto;
      max-width: 500px;
      display: flex;
      justify-content: center;
    }

    .search-bar input {
      padding: 10px;
      width: 80%;
      border-radius: 20px 0 0 20px;
      border: none;
      outline: none;
    }

    .search-bar button {
      padding: 10px 20px;
      background-color: #2e8b57;
      color: white;
      border-radius: 0 20px 20px 0;
      border: none;
      cursor: pointer;
    }

    .cta-button {
      background-color: #2e8b57;
      color: white;
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

    footer {
      text-align: center;
      padding: 20px;
      background-color: #111;
      color: white;
    }
  </style>
</head>
<body>

  <header>
    <h1>[ZedVouched]</h1>
    <p>[Empowering Trustworthy Connections]</p>
  </header>

  <nav>
    <div class="logo">ZedVouched</div>
    <div class="nav-links">
      <a href="#">Home</a>
      <div class="dropdown">
        Services
        <div class="dropdown-content">
          <a href="#">Domestic Help</a>
          <a href="#">Home Repairs</a>
          <a href="#">Tutoring</a>
        </div>
      </div>
      <a href="#">Blog</a>
      <a href="#">Careers</a>
      <a href="#">Contact</a>
      <a href="#">Login</a>
    </div>
    <a class="cta-button" href="#">Chat with us on Whatsapp</a>
  </nav>

  <div class="search-bar">
    <input type="text" placeholder="Search for builders, barbers, tailors, welders...."/>
    <button>Search</button>
  </div>

  <section class="form-section">
    <h2 style="text-align:center;">Help us map out verified providers by nominating your trusted workers</h2>
    <form>
      <input type="text" placeholder="Full Name" required/>
      <input type="email" placeholder="Email Address" required/>
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit" style="background-color:#2e8b57;color:white;border:none;padding:10px;border-radius:20px;">Submit</button>
    </form>
  </section>

  <iframe
    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d30689.456387045594!2d28.2873581!3d-15.3875257!2m3!1f0!2f0!3f0!3m2!
    1i1024!2i768!4f13.1!3m3!1m2!1s0x19409136f68e1e55%3A0xd3076fdb6a192709!2sLusaka!5e0!3m2!1sen!2szm!4v1681130269695!5m2!1sen!2szm"
    allowfullscreen="" loading="lazy">
  </iframe>

  <footer>
    &copy; [2025] ZedVouched | Built with ❤️ in Zambia
  </footer>

</body>
</html>
