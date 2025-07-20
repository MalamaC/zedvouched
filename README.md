<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ZedVouched - Find Trusted Services</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  <script>
    function toggleDropdown(id) {
      const menu = document.getElementById(id);
      menu.classList.toggle("hidden");
    }
  </script>
</head>
<body class="bg-gray-100 font-sans">
  <!-- Navigation bar -->
  <nav class="bg-white shadow p-4 flex justify-between items-center">
    <h1 class="text-2xl font-bold text-green-600">ZedVouched</h1>
    <div class="relative">
      <button onclick="toggleDropdown('categoriesDropdown')" class="text-gray-600 hover:text-green-600">Categories ▾</button>
      <div id="categoriesDropdown" class="absolute mt-2 bg-white border rounded shadow-md hidden z-10 w-64">
        <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100"><span class="text-gray-700 font-semibold">🛠️ Trades & Technical Services</span></a>
        <a href="#" class="block px-4 py-2 text-sm text-indigo-700 hover:bg-gray-100">🎨 Creative & Design Services</a>
        <a href="#" class="block px-4 py-2 text-sm text-teal-700 hover:bg-gray-100">🧹 Domestic & Support Services</a>
        <a href="#" class="block px-4 py-2 text-sm text-blue-700 hover:bg-gray-100">💼 Administrative & Logistical Services</a>
        <a href="#" class="block px-4 py-2 text-sm text-yellow-700 hover:bg-gray-100">🧑🏽‍🏫 Instructional & Skilled Coaching</a>
      </div>
    </div>
    <div class="space-x-4">
      <a href="https://wa.me/260978109185" target="_blank" class="bg-green-500 text-white px-4 py-2 rounded hover:bg-green-600">WhatsApp Us</a>
      <a href="#nominate" class="text-green-700 underline hover:text-green-800">Nominate a Worker</a>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="bg-green-50 p-6 text-center">
    <h2 class="text-3xl font-bold text-gray-700">Your Map to Zambia's Trusted Service Providers</h2>
    <p class="mt-2 text-gray-600">Search, nominate, and share trusted local workers and businesses</p>
    <form class="mt-4 max-w-xl mx-auto flex">
      <input type="text" placeholder="Search for barbers, tailors, welders..." class="flex-grow px-4 py-2 border border-gray-300 rounded-l-md">
      <button class="bg-green-600 text-white px-6 py-2 rounded-r-md hover:bg-green-700">Search</button>
    </form>
    <p class="mt-3 text-sm text-gray-500">Help us fill this map with verified providers by nominating your trusted workers!</p>
  </section>

  <!-- Nomination Form -->
  <section id="nominate" class="p-6 bg-white max-w-2xl mx-auto mt-8 rounded shadow">
    <h3 class="text-xl font-semibold text-gray-800 mb-4">Nominate a Worker</h3>
    <form action="https://docs.google.com/forms/d/e/1FAIpQLSeLwYOURFORMID/formResponse" method="POST" target="_blank" class="space-y-4">
      <input name="entry.1234567890" type="text" placeholder="Worker's Full Name" class="w-full px-4 py-2 border border-gray-300 rounded">
      <input name="entry.0987654321" type="text" placeholder="Type of Service (e.g. Plumber, Tailor)" class="w-full px-4 py-2 border border-gray-300 rounded">
      <input name="entry.1122334455" type="text" placeholder="Phone Number" class="w-full px-4 py-2 border border-gray-300 rounded">
      <input name="entry.6677889900" type="text" placeholder="Location (e.g. Lusaka, Kitwe)" class="w-full px-4 py-2 border border-gray-300 rounded">
      <textarea name="entry.4455667788" placeholder="Why do you recommend them?" class="w-full px-4 py-2 border border-gray-300 rounded"></textarea>
      <input name="entry.9988776655" type="text" placeholder="Link to photo of completed work (optional)" class="w-full px-4 py-2 border border-gray-300 rounded">
      <button type="submit" class="bg-green-600 text-white px-6 py-2 rounded hover:bg-green-700">Submit Nomination</button>
    </form>
  </section>

  <!-- Ratings & Reviews Section -->
  <section class="p-6 mt-8 bg-gray-50 max-w-4xl mx-auto rounded shadow">
    <h3 class="text-xl font-semibold text-gray-800 mb-4">Ratings & Reviews</h3>
    <div class="space-y-6">
      <div class="bg-white p-4 rounded shadow">
        <div class="flex items-center justify-between mb-2">
          <span class="font-semibold text-gray-700">Chipo Banda - Tailor</span>
          <span class="text-yellow-500">★★★★☆</span>
        </div>
        <p class="text-gray-600 text-sm">Chipo delivers on time and her stitching is top-notch. Highly recommended in Chelstone!</p>
      </div>
      <div class="bg-white p-4 rounded shadow">
        <div class="flex items-center justify-between mb-2">
          <span class="font-semibold text-gray-700">James Mwila - Electrician</span>
          <span class="text-yellow-500">★★★★★</span>
        </div>
        <p class="text-gray-600 text-sm">Very reliable and always neat with his work. He fixed our power issue within the hour!</p>
      </div>
    </div>
  </section>

  <!-- Google Map Embed -->
  <section class="mt-8 max-w-5xl mx-auto px-4">
    <h3 class="text-xl font-semibold text-gray-800 mb-4">Pinned Service Providers Map</h3>
    <div class="aspect-w-16 aspect-h-9">
      <iframe src="https://www.google.com/maps/d/u/0/embed?mid=1LQXoxhIWpbgSo7cwGqGIzcfA8jWEMM4" width="100%" height="480" class="rounded shadow"></iframe>
    </div>
  </section>

  <!-- Footer -->
  <footer class="text-center text-sm text-gray-500 p-4 mt-6">
    © 2025 ZedVouched. All rights reserved. | <a href="#" class="text-blue-500 underline">Privacy Disclaimer</a>
  </footer>
</body>
</html>
