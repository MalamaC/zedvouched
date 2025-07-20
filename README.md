#<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ZedVouched | Trusted Service Providers</title>
  <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; }
    header { background-color: #1e6f5c; color: white; padding: 1rem; text-align: center; }
    #search-container { padding: 1rem; text-align: center; }
    #search-input { width: 60%; padding: 0.5rem; font-size: 1rem; }
    #map { height: 500px; width: 100%; }
    #footer-comment { text-align: center; padding: 1rem; font-style: italic; color: #444; }
    #nominate-container { padding: 2rem; text-align: center; background-color: #f9f9f9; }
    #nominate-container input, #nominate-container textarea { width: 80%; padding: 0.5rem; margin: 0.5rem 0; font-size: 1rem; }
    #nominate-container button { background-color: #1e6f5c; color: white; padding: 0.75rem 1.5rem; border: none; border-radius: 5px; cursor: pointer; font-size: 1rem; }
    .whatsapp-button { display: inline-block; margin-top: 1rem; background-color: #25d366; color: white; padding: 0.75rem 1.5rem; border-radius: 25px; text-decoration: none; font-weight: bold; font-size: 1rem; }
  </style>
</head>
<body>
  <header>
    <h1>ZedVouched</h1>
    <p>Verified Service Providers in Zambia</p>
  </header>

  <div id="search-container">
    <input type="text" id="search-input" placeholder="Search for barbers, tailors, welders, bakers..." />
  </div>

  <div id="map"></div>

  <div id="nominate-container">
    <h3>Nominate a Service Provider</h3>
    <input type="text" placeholder="Provider's Name" /><br />
    <input type="text" placeholder="Type of Service (e.g. Barber, Tailor)" /><br />
    <input type="text" placeholder="Location (e.g. Lusaka, Chilenje)" /><br />
    <textarea placeholder="Why are you nominating them? (Optional)"></textarea><br />
    <button>Submit Nomination</button>
    <p style="font-size: 0.9rem; color: gray;">By submitting, you confirm you have the provider's consent to share their contact details. ZedVouched respects privacy and only displays info with permission.</p>
  </div>

  <div id="footer-comment">
    📍 Help us fill this map with your verified service provider! <br />
    Visit our <a href="https://facebook.com/zedvouched" target="_blank">Facebook page</a> to nominate someone.<br /><br />
    <a class="whatsapp-button" href="https://wa.me/260978109185" target="_blank">💬 Chat with us on WhatsApp</a>
  </div>

  <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>
  <script>
    const map = L.map('map').setView([-15.3875, 28.3228], 13); // Lusaka coordinates

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      attribution: 'Map data © OpenStreetMap contributors',
    }).addTo(map);

    const providers = [
      {
        name: "John the Barber",
        type: "Barber",
        lat: -15.4075,
        lng: 28.3228,
      },
      {
        name: "Mary's Tailor Shop",
        type: "Tailor",
        lat: -15.3975,
        lng: 28.3175,
      },
    ];

    providers.forEach((provider) => {
      L.marker([provider.lat, provider.lng])
        .addTo(map)
        .bindPopup(`<b>${provider.name}</b><br>${provider.type}`);
    });

    document.getElementById("search-input").addEventListener("input", function (e) {
      const term = e.target.value.toLowerCase();
      map.eachLayer((layer) => {
        if (layer.getPopup && layer.getPopup()) {
          const content = layer.getPopup().getContent().toLowerCase();
          if (!content.includes(term)) {
            map.removeLayer(layer);
          } else {
            layer.addTo(map);
          }
        }
      });
    });
  </script>
</body>
</html>
