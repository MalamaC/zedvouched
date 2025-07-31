<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ZedVouched</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    :root {
      --orange-bg: #F27024;
      --orange-grad1: #FF8A00;
      --orange-grad2: #FF5E00;
      --btn-green: #226E2F;
      --btn-green-h: #1B5E20;
      --text-black: #2C2C2C;
      --text-gray: #555555;
      --form-bg: #FEF3E5;
      --card-bg: #FFFFFF;
      --reviews-bg: #F2F2F2;
    }
    body {
      font-family: 'Inter', sans-serif;
      /* Gradient background matching mock: angle 135deg from #FF8A00 to #FF5E00 */
      background: linear-gradient(135deg, var(--orange-grad1) 0%, var(--orange-grad2) 100%);
      color: var(--text-black);
      margin: 0;
    }
    .input, .textarea {
      border: 1px solid #ccc;
      border-radius: 8px;
      font-size: 16px;
      line-height: 24px;
    }
    h1 {
      font-size: 56px;
      line-height: 64px;
    }
    h2 {
      font-size: 56px;
      line-height: 64px;
    }
    .btn-green {
      background-color: var(--btn-green);
      transition: background-color 0.3s;
      border-radius: 8px;
    }
    .btn-green:hover {
      background-color: var(--btn-green-h);
    }
    .animate-fade {
      animation: fadeIn 0.8s ease-in-out;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
</head>
<body>
  <!-- Header -->
  <header class="flex items-center justify-between py-4 px-6 bg-transparent">
    <div class="flex items-center space-x-3">
      <img src="images/logo_nobackground.png" alt="ZedVouched" class="h-20 w-50">
    </div>
    <nav class="hidden lg:flex items-center space-x-6 text-base font-medium">
      <div class="relative group">
        <button class="flex items-center space-x-1">Technical Services <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path d="M19 9l-7 7-7-7"></path></svg></button>
      </div>
      <div class="relative group">
        <button class="flex items-center space-x-1">Design Services <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path d="M19 9l-7 7-7-7"></path></svg></button>
      </div>
      <div class="relative group">
        <button class="flex items-center space-x-1">Domestic & Support <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path d="M19 9l-7 7-7-7"></path></svg></button>
      </div>
      <div class="relative group">
        <button class="flex items-center space-x-1">Administrative <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path d="M19 9l-7 7-7-7"></path></svg></button>
      </div>
      <div class="relative group">
        <button class="flex items-center space-x-1">Logistics <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path d="M19 9l-7 7-7-7"></path></svg></button>
      </div>
      <a href="https://wa.me/260978109185" class="ml-6 px-4 py-2 bg-green-700 text-white rounded shadow hover:bg-green-800">WhatsApp</a>
    </nav>
    <button class="lg:hidden px-2 py-1 bg-white rounded"><svg class="w-6 h-6 text-gray-800" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path d="M4 6h16M4 12h16M4 18h16"></path></svg></button>
  </header>

  <!-- Main Hero + Form -->
  <section class="flex flex-col lg:flex-row items-center px-6 lg:px-24 pt-12 animate-fade">
    <!-- Hero Text -->
    <div class="lg:w-1/2 mb-12 lg:mb-0">
      <h1 class="text-black text-6xl font-bold leading-tight mb-6">
        Let’s fill the<br />Zambian map, together
      </h1>
      <blockquote class="bg-semi-transparent-card p-4 rounded mb-6 max-w-md text-gray-800">Search local workers and businesses trusted and vouched for by Zambians…</blockquote>
      <button class="btn-green text-white px-6 py-3 rounded shadow">Search</button>
    </div>
    <!-- Nomination Form -->
    <div class="lg:w-1/2 px-4">
      <div class="bg-sec-bg p-6 rounded-lg shadow-lg animate-fade max-w-md">
        <h2 class="text-xl font-semibold text-black mb-4">Nominate a Provider</h2>
        <form action="https://formsubmit.co/your@email.com" method="POST" enctype="multipart/form-data">
          <label class="block text-sm font-medium text-black mb-1">Provider Full Name</label>
          <input type="text" name="name" class="input w-full p-2 mb-4" placeholder="e.g. Jelita Mulenga" required>
          <label class="block text-sm font-medium text-black mb-1">Type of Service</label>
          <input type="text" name="service" class="input w-full p-2 mb-4" placeholder="e.g. Tailor" required>
          <label class="block text-sm font-medium text-black mb-1">Provider Phone Number</label>
          <input type="tel" name="phone" class="input w-full p-2 mb-4" placeholder="e.g. +2609…" required>
          <label class="block text-sm font-medium text-black mb-1">Location (e.g. Lusaka, Kitwe)</label>
          <input type="text" name="location" class="input w-full p-2 mb-4" placeholder="Where to find provider" required>
          <label class="block text-sm font-medium text-black mb-1">Attach Photo (optional)</label>
          <input type="file" name="photo" class="w-full mb-4" accept="image/*">
          <label class="block text-sm font-medium text-black mb-1">Your Message</label>
          <textarea name="message" rows="4" class="textarea w-full p-2 mb-4" placeholder="Why do you vouch for them?">
          <button type="submit" class="btn-green w-full text-white py-3 rounded">Nominate</button>
        </form>
      </div>
    </div>
  </section>

  <!-- Map Section Title -->
  <section class="px-6 lg:px-24 pt-16 animate-fade">
    <div class="flex flex-col lg:flex-row items-center gap-8">
      <!-- Left Text Block (30%) -->
      <div style="flex: 0 0 30%;">
        <h2 class="text-black text-6xl font-bold leading-tight">Your Map to<br />Zambia’s Trusted Service Providers</h2>
      </div>
      <!-- Right Map Block (70%) -->
      <div class="rounded-lg overflow-hidden shadow-lg" style="flex: 0 0 70%;">
        <iframe src="https://www.google.com/maps/d/embed?mid=1LQXoxhIWpbgSo7cwGqGIzcfA8jWEMM4&ehbc=2E312F" width="100%" height="480" class="block"></iframe>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="mt-16 px-6 lg:px-24 py-6 text-center text-gray-800 text-sm animate-fade">&copy; 2025 ZedVouched | Built with ❤️ in Zambia</footer>
</body>
</html>
