
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Snakista - Taste the Tradition!</title>

  <!-- Google Font Link -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet" />

  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background-color: #f4efff;
      color: #4b0082;
    }
    header, nav, footer {
      background-color: #4b0082;
      color: white;
      padding: 1em;
      text-align: center;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
    }
    h1, h2 {
      color: #4b0082;
    }
    .section {
      padding: 2em;
      text-align: center;
    }
    .products, .gallery {
      display: flex;
      justify-content: center;
      gap: 1em;
      flex-wrap: wrap;
    }
    .products img, .gallery img {
      width: 200px;
      height: 200px;
      border-radius: 15px;
      object-fit: cover;
    }
    .btn {
      display: inline-block;
      margin-top: 1em;
      padding: 0.75em 1.5em;
      background-color: #4b0082;
      color: white;
      text-decoration: none;
      border-radius: 8px;
    }
  </style>
</head>
<body>

  <header>
    <h1>Snakista</h1>
    <p>Taste the love, spice the life.</p>
  </header>

  <nav>
    <a href="#home">Home</a>
    <a href="#menu">Menu</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="home" class="section">
    <h2>Welcome to Snakista</h2>
    <p>Your destination for crunchy, spicy, and fresh snacks – with a desi twist!</p>
    <a href="#menu" class="btn">Explore Our Menu</a>
  </section>

  <section id="menu" class="section">
    <h2>Our Snacks</h2>
    <div class="products">
      <div>
        <img src="https://via.placeholder.com/200" alt="Tandoori Twists" />
        <p><strong>Tandoori Twists</strong> – ₹60</p>
      </div>
      <div>
        <img src="https://via.placeholder.com/200" alt="Masala Munch" />
        <p><strong>Masala Munch Mix</strong> – ₹80</p>
      </div>
      <div>
        <img src="https://via.placeholder.com/200" alt="Combo Box" />
        <p><strong>Chai + Snack Combo</strong> – ₹99</p>
      </div>
    </div>
  </section>

  <section id="about" class="section">
    <h2>About Us</h2>
    <p>Snakista is where street-style meets soul food. We serve handcrafted snacks with bold spices, authentic flavors, and the warmth of home.</p>
  </section>

  <section id="contact" class="section">
    <h2>Contact Us</h2>
    <p>📱 WhatsApp Order: 
      <a class="btn" href="https://wa.me/917208731279?text=Hi%20Snakista%2C%20I%20want%20to%20place%20an%20order!" target="_blank">
        Message Now
      </a>
    </p>
    <p>📸 Instagram: <a href="https://instagram.com/snakista.in" target="_blank">@snakista.in</a></p>
  </section>

  <footer>
    <p>© 2025 Snakista. All rights reserved.</p>
  </footer>

</body>
</html>
