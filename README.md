<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Wally TV | Inspire, Create, Educate</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- HEADER -->
  <header>
    <div class="logo">🎥 WALLY Graphic TV</div>

    <!-- Search Bar -->
    <div class="search-container">
      <input type="text" id="search-input" placeholder="Search Wally Graphic TV...">
      <button id="search-btn">🔍</button>
    </div>

    <!-- Dark/Light Mode Toggle -->
    <button id="theme-toggle" class="theme-btn">🌞</button>

    <!-- Navigation -->
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#graphic">Wally Graphic Design</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- BACKGROUND MUSIC -->
  <audio id="bg-music" loop autoplay>
    <source src="music.mp3" type="audio/mpeg">
  </audio>

  <!-- HERO SECTION -->
  <section id="home" class="hero">
    <div class="overlay">
      <h1>Welcome to Wally Graphic TV</h1>
      <p>Communicating inspiration through beautiful designs, music, and education.</p>
      <a href="#gallery" class="btn">Watch Now</a>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about" class="section">
    <h2>About Us</h2>
    <p>Wally Graphic TV started in April 2024 in Bafoussam, Cameroon. We use creative designs, music, and videos to share meaningful information that inspires change and education. Our viral contents continue to touch lives across Cameroon and beyond.</p>
  </section>

  <!-- SERVICES -->
  <section id="services" class="section">
    <h2>Our Services</h2>
    <div class="cards">
      <div class="card">
        <h3>🎬 Video Production</h3>
        <p>We create educational, inspirational, and musical videos that move hearts and minds.</p>
      </div>
      <div class="card">
        <h3>🎨 Graphic Design</h3>
        <p>Professional digital art and designs for events, brands, and social media campaigns.</p>
      </div>
      <div class="card">
        <h3>🧑‍💻 Training Programs</h3>
        <p>Learn design skills through our online and onsite graphic design training courses.</p>
      </div>
      <div class="card">
        <h3>📢 Advertising</h3>
        <p>We help you promote your business and creative works across multiple platforms.</p>
      </div>
    </div>
  </section>

  <!-- WALLY GRAPHIC DESIGN -->
  <section id="graphic" class="section">
    <h2>Wally Graphic Design</h2>
    <p>We organize online and onsite training programs for beginners and professionals. Join us to learn practical skills in creative design and digital marketing.</p>
    <a href="#contact" class="btn">Join Our Training</a>
  </section>

  <!-- GALLERY / VIDEO PLAYER -->
  <section id="gallery" class="section">
    <h2>Our Media</h2>
    <div class="video-container">
      <iframe width="560" height="315"
        src="https://www.youtube.com/embed/YOUR_VIDEO_ID"
        title="Wally TV Video"
        frameborder="0"
        allowfullscreen></iframe>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="section contact">
    <h2>Contact Us</h2>
    <p>Email: info@wallytv.cm</p>
    <p>Location: Bafoussam, Cameroon</p>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit" class="btn">Send Message</button>
    </form>
  </section>

  <footer>
    <p>© 2025 Wally Graphic TV. All Rights Reserved.</p>
  </footer>

  <!-- JAVASCRIPT -->
  <script>
    // Search Function
    const searchBtn = document.getElementById("search-btn");
    const searchInput = document.getElementById("search-input");
    searchBtn.addEventListener("click", function() {
      const query = searchInput.value.trim();
      if (query) {
        window.open(`https://www.google.com/search?q=site:wallytv.cm+${query}`, "_blank");
      }
    });

    // Light/Dark Theme Toggle
    const themeToggle = document.getElementById("theme-toggle");
    themeToggle.addEventListener("click", () => {
      document.body.classList.toggle("dark-mode");
      themeToggle.textContent = document.body.classList.contains("dark-mode") ? "🌙" : "🌞";
    });

    // Background Music (auto starts low volume)
    const music = document.getElementById("bg-music");
    music.volume = 0.1; // soft background sound
  </script>
</body>
</html>
