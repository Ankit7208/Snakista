<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Snakista - Taste the Love, Spice the Life</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Poppins', sans-serif;
      background-color: #fdf6f9;
      color: #333;
    }
    header {
      background-color: #6a1b9a;
      color: white;
      padding: 1.5em 1em;
      text-align: center;
    }
    nav {
      background-color: #4a148c;
      display: flex;
      justify-content: center;
      padding: 0.8em 0;
    }
    nav a {
      color: white;
      margin: 0 1.5em;
      text-decoration: none;
      font-weight: 600;
    }
    .hero {
      text-align: center;
      padding: 3em 1em;
      background: url('https://images.unsplash.com/photo-1606851092094-d68ef3e5d90d') no-repeat center center/cover;
      color: white;
    }
    .hero h1 {
      font-size: 3em;
      margin-bottom: 0.5em;
    }
    .section {
      padding: 3em 1em;
      text-align: center;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 2em;
      padding: 1em;
    }
    .card {
      background: white;
      padding: 1em;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }
    .card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 8px;
    }
    .card h3 {
      margin: 1em 0 0.5em;
    }
    .btn {
      display: inline-block;
      margin-top: 1em;
      padding: 0.75em 1.5em;
      background-color: #6a1b9a;
      color: white;
      border-radius: 5px;
      text-decoration: none;
      font-weight: 600;
    }
    footer {
      background-color: #4a148c;
      color: white;
      padding: 1.5em;
      text-align: center;
    }
  </style>
</head>
<body>
  <header>
    <h1>Snakista</h1>
    <p>Taste the Love, Spice the Life</p>
  </header>
  <nav>
    <a href="#home">Home</a>
    <a href="#products">Products</a>
    <a href="#order">Order</a>
    <a href="#contact">Contact</a>
  </nav>

  <div class="hero">
    <h1>Welcome to Snakista</h1>
    <p>Your destination for irresistible dry & fresh snacks!</p>
  </div>

  <div class="section" id="products">
    <h2>Our Popular Snacks</h2>
    <div class="products">
      <div class="card">
        <img src="https://images.unsplash.com/photo-1601050690590-be1bfa311a12" alt="Dry Bhel">
        <h3>Shuka Bhel</h3>
        <p>Only ₹25</p>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1627308595229-7830a5c91f9f" alt="Aloo Bhujia">
        <h3>Aloo Bhujia</h3>
        <p>Only ₹30</p>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1611042553365-490bf6f3228d" alt="Moong Dal">
        <h3>Moong Dal</h3>
        <p>Only ₹40</p>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1586190848861-99aa4a171e90" alt="Combo">
        <h3>Combo Pack (Chai + Nasta)</h3>
        <p>Only ₹89</p>
      </div>
    </div>
    <a class="btn" href="https://wa.me/917208731279" target="_blank">Order on WhatsApp</a>
  </div>

  <footer id="contact">
    <p>&copy; 2025 Snakista. All rights reserved.</p>
    <p>Contact: +91 72087 31279 | Instagram: @snakista</p>
  </footer>
</body>
</html>
