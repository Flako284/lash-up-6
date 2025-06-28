<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Crown Essence</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
  <script src="https://unpkg.com/feather-icons"></script>
  <script src="https://js.stripe.com/v3/"></script>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="icon" type="image/png" href="logo.png" />
  <style>
    body {
      font-family: 'Poppins', sans-serif;
    }
  </style>
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet" />
</head>
<body class="bg-gradient-to-r from-black to-gray-900 text-white">
  <button class="fixed top-4 right-4 bg-purple-700 hover:bg-purple-800 text-white p-2 rounded-full shadow-lg transition" onclick="toggleTheme()" title="Switch Theme"><i data-feather="sun"></i></button>

  <!-- Header -->
  <header class="bg-gradient-to-r from-purple-800 to-blue-600 text-white text-center py-16 clip-path-ellipse shadow-xl">
    <img src="logo.png" alt="Crown Essence Logo" class="w-36 h-36 mx-auto rounded-full border-4 border-white shadow-lg" />
    <h1 class="text-5xl font-bold mt-4 tracking-wide">Crown Essence</h1>
    <p class="text-lg mt-2">Royal Styles for Kings & Queens – Book Your Crown Today!</p>
  </header>

  <!-- Main Content -->
  <main class="max-w-6xl mx-auto px-4 py-10">
    <section class="grid md:grid-cols-2 gap-10 mb-16">
      <div>
        <h2 class="text-2xl font-bold text-purple-300 mb-2">📍 Location</h2>
        <p class="text-lg">East End, Tortola, British Virgin Islands 🇻🇬</p>
      </div>
      <div>
        <h2 class="text-2xl font-bold text-purple-300 mb-2">💇🏽‍♀️ Services</h2>
        <p class="text-lg">Talented Braiding • Protective Styles • Natural Haircare</p>
      </div>
    </section>

    <!-- User Images Section -->
    <section class="mb-16">
      <h2 class="text-2xl font-bold text-purple-300 mb-6 text-center">✨ Client Looks</h2>
      <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
        <div class="relative overflow-hidden rounded-xl shadow-xl group">
          <img src="/mnt/data/WhatsApp Image 2025-06-27 at 7.33.10 PM.jpeg" alt="Elegant Fulani Braids" class="w-full h-full object-cover transform group-hover:scale-105 transition duration-300">
          <div class="absolute bottom-0 bg-gradient-to-t from-black/80 to-transparent w-full text-white text-sm p-3">
            <p class="font-semibold">Elegant Fulani Braids</p>
          </div>
        </div>

        <div class="relative overflow-hidden rounded-xl shadow-xl group">
          <img src="/mnt/data/WhatsApp Image 2025-06-27 at 7.49.20 PM.jpeg" alt="Stylish Protective Cornrows" class="w-full h-full object-cover transform group-hover:scale-105 transition duration-300">
          <div class="absolute bottom-0 bg-gradient-to-t from-black/80 to-transparent w-full text-white text-sm p-3">
            <p class="font-semibold">Stylish Protective Cornrows</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Styles Gallery -->
    <section class="mb-16">
      <h2 class="text-2xl font-bold text-purple-300 mb-6 text-center">🎨 Style Inspiration</h2>
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6"></div>
    </section>

    <!-- Additional Braided Styles -->
    <hr class="my-12 border-purple-800 opacity-40">
    <section class="bg-gray-800 rounded-xl py-10 px-6 my-16 shadow-2xl" data-aos="fade-up">
      <h2 class="text-2xl font-semibold text-purple-200 mb-4 text-center">🌟 More Braided Inspiration</h2>
      <p class="text-purple-200 mb-8 text-center max-w-xl mx-auto">Here’s more braid artistry to inspire your next appointment. These trending styles combine elegance with edge.</p>
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
        <div class="relative overflow-hidden rounded-lg shadow-lg group">
          <img src="https://images.unsplash.com/photo-1592878904946-2691f000a9f5" alt="Tribal Braids" class="w-full h-56 object-cover transform group-hover:scale-105 transition duration-300">
          <div class="absolute bottom-0 bg-gradient-to-t from-black/80 to-transparent w-full text-white text-sm p-3">
            <p class="font-semibold">Tribal Braids</p>
          </div>
        </div>
        <div class="relative overflow-hidden rounded-lg shadow-lg group">
          <img src="https://images.unsplash.com/photo-1618354691213-3ba0bcb1e916" alt="Box Braids with Color" class="w-full h-56 object-cover transform group-hover:scale-105 transition duration-300">
          <div class="absolute bottom-0 bg-gradient-to-t from-black/80 to-transparent w-full text-white text-sm p-3">
            <p class="font-semibold">Box Braids with Color</p>
          </div>
        </div>
        <div class="relative overflow-hidden rounded-lg shadow-lg group">
          <img src="https://images.unsplash.com/photo-1611341511080-df8e4c1d4e3a" alt="Twists with Beads" class="w-full h-56 object-cover transform group-hover:scale-105 transition duration-300">
          <div class="absolute bottom-0 bg-gradient-to-t from-black/80 to-transparent w-full text-white text-sm p-3">
            <p class="font-semibold">Twists with Beads</p>
          </div>
        </div>
      </div>
      <div class="text-center mt-10">
        <a href="#bookingForm" class="inline-block bg-purple-700 hover:bg-purple-800 text-white px-6 py-3 rounded-full font-medium transition">View Full Style Guide</a>
      </div>
    </section>

    <!-- Booking Form -->
    <section class="bg-purple-900 p-8 rounded-2xl shadow-2xl mb-16">
      <h2 class="text-2xl font-bold text-white mb-6 text-center">Book Your Appointment</h2>
      <form id="bookingForm" class="space-y-4">
        <input type="text" id="name" name="name" placeholder="Full Name" required class="w-full p-3 rounded-lg bg-gray-800 text-white">
        <select id="gender" name="gender" required class="w-full p-3 rounded-lg bg-gray-800 text-white">
          <option value="">Select Gender</option>
          <option value="Female">Female</option>
          <option value="Male">Male</option>
          <option value="Other">Other</option>
        </select>
        <select id="style" name="style" required class="w-full p-3 rounded-lg bg-gray-800 text-white"></select>
        <select id="duration" name="duration" required class="w-full p-3 rounded-lg bg-gray-800 text-white">
          <option value="">Select Duration</option>
          <option value="1 hour">1 Hour</option>
          <option value="2 hours">2 Hours</option>
          <option value="3+ hours">3+ Hours</option>
        </select>
        <input type="date" id="date" name="date" required class="w-full p-3 rounded-lg bg-gray-800 text-white">
        <input type="time" id="time" name="time" required class="w-full p-3 rounded-lg bg-gray-800 text-white">
        <input type="number" id="deposit" name="deposit" min="10" step="0.01" placeholder="Deposit ($10 min)" required class="w-full p-3 rounded-lg bg-gray-800 text-white">
        <textarea id="notes" name="notes" rows="3" placeholder="Additional Notes" class="w-full p-3 rounded-lg bg-gray-800 text-white"></textarea>
        <button type="submit" class="w-full bg-purple-700 hover:bg-purple-800 transition p-3 rounded-lg font-bold">Confirm Booking</button>
      </form>
    </section>

    <!-- Instagram Section -->
    <section class="text-center mb-12">
      <h2 class="text-2xl text-purple-300 font-semibold">📸 Follow Us on Instagram</h2>
      <p class="mt-2">
        <a href="https://www.instagram.com/crownessence.vi/" target="_blank" class="text-purple-400 hover:underline">@crownessence.vi</a>
      </p>
      <img src="https://i.imgur.com/4M34hi2.png" alt="Instagram Preview" class="mx-auto mt-4 w-full max-w-sm rounded-xl shadow-xl">
    </section>

    <!-- Direct Booking CTA -->
    <div class="text-center mb-10">
      <a href="https://www.instagram.com/direct/t/crownessence.vi" target="_blank" class="text-white bg-purple-700 px-8 py-3 rounded-full shadow-lg hover:bg-purple-800 transition text-lg font-semibold">📩 Book Now via DM</a>
    </div>
  </main>

  <!-- Footer -->
  <footer class="text-center text-sm text-purple-300 py-8 border-t border-purple-800">
    <p class="mb-1"><i data-feather="phone"></i> (123) 456-7890 | <i data-feather="mail"></i> info@crownessence.com</p>
    <p class="mb-1"><i data-feather="map-pin"></i> 123 Queen's Way, Royal City</p>
    <p>© 2025 Crown Essence | Designed by Nai</p>
  </footer>

  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script>
    feather.replace();
    AOS.init();
    function toggleTheme() {
      document.body.classList.toggle('bg-white');
      document.body.classList.toggle('text-black');
    }

    const hairstyles = [
      { name: 'Box Braids', img: 'https://images.unsplash.com/photo-1590080876216-2f950c417cb9' },
      { name: 'Cornrows', img: 'https://images.unsplash.com/photo-1620819638426-8d129d3a63ee' },
      { name: 'Twist Out', img: 'https://images.unsplash.com/photo-1610805228010-c3ee6bc33db4' },
      { name: 'High Bun', img: 'https://images.unsplash.com/photo-1525072124605-497df6a9623f' },
      { name: 'Fulani Braids', img: 'https://images.unsplash.com/photo-1627497304541-0cb37b87806e' },
      { name: 'Passion Twists', img: 'https://images.unsplash.com/photo-1600185368184-bc10ef8a23b2' },
      { name: 'Braided Bun', img: 'https://images.unsplash.com/photo-1591183799321-5e1376716d1b' },
      { name: "Fade with Braids (Men)", img: "https://images.unsplash.com/photo-1531259683007-016a7b628fc6" }
    ];

    const gallery = document.querySelector('main > section:nth-of-type(3) > div');
    const styleDropdown = document.getElementById('style');

    hairstyles.forEach(style => {
      const card = document.createElement('div');
      card.className = 'bg-gray-800 p-4 rounded-xl shadow-xl text-center hover:scale-105 transition-transform';
      card.innerHTML = `<img src="${style.img}" alt="${style.name}" class="w-full h-40 object-cover rounded-lg mb-3" /><p class="font-semibold text-white">${style.name}</p>`;
      gallery.appendChild(card);

      const option = document.createElement('option');
      option.value = style.name;
      option.textContent = style.name;
      styleDropdown.appendChild(option);
    });

    document.getElementById('bookingForm').addEventListener('submit', function(event) {
      event.preventDefault();
      const deposit = parseFloat(document.getElementById('deposit').value);
      if (isNaN(deposit) || deposit < 10) {
        alert('A minimum deposit of $10 is required to book.');
        return;
      }
      alert('Thank you! Your appointment and deposit are confirmed.');
      this.reset();
    });
  </script>
</body>
</html>
<!-- Styles Gallery 2: More Braided Styles -->
<section class="max-w-4xl mx-auto px-4 py-8">
  <h2 class="text-2xl font-semibold text-purple-300 mb-6">🌟 More Braided Styles</h2>
  <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
    <div class="relative overflow-hidden rounded-lg shadow-lg group">
      <img src="https://images.unsplash.com/photo-1592878904946-2691f000a9f5" alt="Tribal Braids" class="w-full h-56 object-cover transform group-hover:scale-105 transition duration-300">
      <div class="absolute bottom-0 bg-gradient-to-t from-black/80 to-transparent w-full text-white text-sm p-3">
        <p class="font-semibold">Tribal Braids • 3 hrs</p>
      </div>
    </div>
    <div class="relative overflow-hidden rounded-lg shadow-lg group">
      <img src="https://images.unsplash.com/photo-1618354691213-3ba0bcb1e916" alt="Box Braids with Color" class="w-full h-56 object-cover transform group-hover:scale-105 transition duration-300">
      <div class="absolute bottom-0 bg-gradient-to-t from-black/80 to-transparent w-full text-white text-sm p-3">
        <p class="font-semibold">Box Braids with Color • 4 hrs</p>
      </div>
    </div>
    <div class="relative overflow-hidden rounded-lg shadow-lg group">
      <img src="https://images.unsplash.com/photo-1611341511080-df8e4c1d4e3a" alt="Twists with Beads" class="w-full h-56 object-cover transform group-hover:scale-105 transition duration-300">
      <div class="absolute bottom-0 bg-gradient-to-t from-black/80 to-transparent w-full text-white text-sm p-3">
        <p class="font-semibold">Twists with Beads • 2.5 hrs</p>
      </div>
    </div>
  </div>
</section>
