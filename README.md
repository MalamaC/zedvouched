<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>ZedVouched</title>

  <!-- Inter font (weights used on the mock) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

  <style>
    *,*::before,*::after{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0;font-family:"Inter",sans-serif;background:
      radial-gradient(1200px 800px at 15% 18%, #FFB36B 0%, #F47F2A 38%, rgba(244,127,42,0) 60%),
      radial-gradient(900px 700px at 85% 80%, #E45E00 0%, #CF5200 45%, rgba(207,82,0,0) 70%),
      linear-gradient(200deg, #F27024 0%, #EF6C00 100%);
    background-color:#F27024;
    background-attachment:fixed;color:#2C2C2C;}
    a{text-decoration:none;color:inherit}
    .container{max-width:1160px;margin:0 auto;padding:0 10px}
    .site-header{padding:18px 0;}
    .brand img{height:64px}
    .header-flex {display:flex;justify-content:space-between;align-items:center;}
    .nav{display:flex;justify-content:space-between;gap:28px;font-weight:600;font-size:16px;width:100%; padding:20px 0;}
    .nav a:hover{color:#ffdbbf}
    .cta{padding:10px 16px;background:#226E2F;color:#fff;border-radius:12px;margin-left:auto}
    .cta:hover{background:#1B5E20}
    .hero{padding:2% 0 8px}
    .hero-title{font-weight:900;line-height:0.95;font-size:clamp(44px, 7.5vw, 96px)}
    .hero-card{margin-top:28px;max-width:440px;background:rgba(255,255,255,0.30);padding:18px 20px;border-radius:14px;font-weight:500}
    .btn{display:inline-block;margin-top:18px;padding:14px 22px;background:#226E2F;color:#fff;border-radius:10px}
    .btn:hover{background:#1B5E20}
    .card{background:#FEF3E5;padding:22px;border-radius:16px;max-width:520px;margin-left:auto; margin-top:5%;}
    .card h2{font-size:22px;font-weight:700;margin-bottom:12px}
    label{font-size:14px;font-weight:600;margin-bottom:6px;display:block;font-family:"Inter",sans-serif}
    .input,.textarea{width:100%;border:1px solid #d7d7d7;background:#fff;border-radius:10px;padding:12px 14px;font-size:16px;margin-bottom:16px;font-family:"Inter",sans-serif}
    .textarea{min-height:112px}
    .submit{width:100%;padding:14px 22px;background:#226E2F;color:#fff;border-radius:10px;font-family:"Inter",sans-serif}
    .submit:hover{background:#1B5E20}
    .section{padding:32px 0}
    .map-title{font-weight:900;line-height:.98;font-size:clamp(38px, 6.5vw, 84px)}
    .map-frame{border:0;width:100%;height:480px;border-radius:16px}
    .footer{padding:14px 0;text-align:center;color:#222;font-size:14px;font-weight:600}

    /* Grid for map section */
    .map-grid {
      display: grid;
      grid-template-columns: 35% 65%;
      gap: 28px;
      align-items: center;
    }
    @media(max-width: 900px){
      .map-grid {grid-template-columns: 1fr;}
    }

    /* Grid for hero section */
    .hero-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
      align-items: start;
    }
    @media(max-width: 900px){
      .hero-grid {grid-template-columns: 1fr;}
    }
  </style>
</head>
<body>
  <!-- Header -->
  <header class="site-header">
    <div class="container header-flex">
      <div class="brand">
        <img src="zedvouched_logo.png" alt="ZedVouched Logo">
      </div>
      <a class="cta" href="https://wa.me/260978109185">WhatsApp</a>
    </div>
    <nav class="nav container">
      <a href="#">Technical Services</a>
      <a href="#">Design Services</a>
      <a href="#">Domestic &amp; Support</a>
      <a href="#">Administrative</a>
      <a href="#">Logistics</a>
    </nav>
  </header>

  <!-- Hero -->
  <section class="hero container hero-grid">
    <div>
      <h1 class="hero-title">Let’s fill the<br>Zambian map, together</h1>
      <div class="hero-card">Search local workers and businesses trusted and vouched for by Zambians…</div>
      <a class="btn" href="#map">Search</a>
    </div>
    <div>
      <div class="card">
        <h2>Nominate a Provider</h2>
        <form action="https://formsubmit.co/your@email.com" method="POST" enctype="multipart/form-data">
          <label>Full Name</label>
          <input class="input" type="text" name="name" placeholder="e.g. Jelita Mulenga" required>
          <label>Type of Service</label>
          <input class="input" type="text" name="service" placeholder="e.g. Tailor" required>
          <label>Phone Number</label>
          <input class="input" type="tel" name="phone" placeholder="e.g. +2609…" required>
          <label>Location (e.g. Lusaka, Kitwe)</label>
          <input class="input" type="text" name="location" placeholder="Where to find provider" required>
          <label>Attach photo of completed work (optional)</label>
          <input type="file" name="photo" accept="image/*" style="margin-bottom:16px">
          <label>Your Message</label>
          <textarea class="textarea" name="message" placeholder="Why do you vouch for them?"></textarea>
          <button type="submit" class="submit">Nominate</button>
        </form>
      </div>
    </div>
  </section>

  <!-- Map -->
  <section id="map" class="section container map-grid">
    <div>
      <h2 class="map-title">Your Map to<br>Zambia’s Trusted Service Providers</h2>
    </div>
    <div>
      <iframe class="map-frame" src="https://www.google.com/maps/d/embed?mid=1LQXoxhIWpbgSo7cwGqGIzcfA8jWEMM4&ehbc=2E312F" loading="lazy" allowfullscreen></iframe>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">&copy; 2025 ZedVouched | Built with ❤️ in Zambia</footer>

  <!-- Reminder: Place a blank .nojekyll file at the root of your repo to disable Jekyll on GitHub Pages -->
</body>
</html>
