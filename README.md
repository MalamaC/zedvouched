<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>ZedVouched</title>

    <!-- Google Fonts -->
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap"
      rel="stylesheet"
    />

    <!-- Tailwind CDN -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- Custom Styles -->
    <style>
      body {
        font-family: 'Inter', sans-serif;
        background-color: #fef3e5;
      }

      .bg-semi-transparent-card {
        background-color: rgba(255, 255, 255, 0.7);
      }

      .bg-sec-bg {
        background-color: #fef3e5;
      }
    </style>
  </head>
  <body class="bg-sec-bg text-gray-800">
    <!-- Header -->
    <header class="flex items-center justify-between p-4 shadow bg-white">
      <img
        src="./images/logo_nobackground.png"
        alt="ZedVouched Logo"
        class="h-12"
      />
      <nav>
        <ul class="flex space-x-6 font-medium text-sm">
          <li><a href="#" class="hover:text-orange-600">Home</a></li>
          <li class="relative group">
            <button class="hover:text-orange-600">Technical Services</button>
            <ul class="absolute hidden mt-2 bg-white shadow-lg rounded group-hover:block text-sm z-10">
              <li><a href="#" class="block px-4 py-2 hover:bg-gray-100">Plumber</a></li>
              <li><a href="#" class="block px-4 py-2 hover:bg-gray-100">Mechanic</a></li>
              <li><a href="#" class="block px-4 py-2 hover:bg-gray-100">Welder</a></li>
              <li><a href="#" class="block px-4 py-2 hover:bg-gray-100">Carpenter</a></li>
              <li><a href="#" class="block px-4 py-2 hover:bg-gray-100">Electrician</a></li>
              <li><a href="#" class="block px-4 py-2 hover:bg-gray-100">Technician</a></li>
            </ul>
          </li>
          <li><a href="#" class="hover:text-orange-600">About</a></li>
        </ul>
      </nav>
    </header>

    <!-- Hero Section -->
    <section class="flex flex-col md:flex-row p-6 md:p-12 gap-6 items-center md:items-stretch">
      <!-- Text Block -->
      <div class="w-full md:w-1/3 flex flex-col justify-center">
        <h1 class="text-4xl md:text-5xl font-bold leading-tight mb-4">
          Let’s fill the <br />
          <span class="text-orange-600">Zambian</span> map, together
        </h1>
        <p class="text-lg mb-4">
          Search local workers and businesses trusted and vouched for by Zambians…
        </p>
        <input
          type="text"
          placeholder="Search"
          class="px-4 py-2 border border-gray-300 rounded w-full"
        />
      </div>

      <!-- Map Block -->
      <div class="w-full md:w-2/3">
        <div class="w-f
