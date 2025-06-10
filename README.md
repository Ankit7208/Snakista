<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Snakista Cafe</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }
    body {
      background-color: #f9f5fc;
      color: #333;
    }
    header {
      background-color: #6a0dad;
      padding: 1.5rem;
      text-align: center;
      color: white;
    }
    nav {
      display: flex;
      justify-content: center;
      background-color: #55007a;
      padding: 0.8rem;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin: 0 1rem;
      font-weight: 600;
    }
    .hero {
      background: url('https://images.unsplash.com/photo-1498654200943-1088dd4438ae?auto=format&fit=crop&w=1200&q=80') no-repeat center center/cover;
      height: 60vh;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      text-shadow: 2px 2px 5px rgba(0,0,0,0.7);
    }
    .hero h1 {
      font-size: 3rem;
    }
    .section {
      padding: 3rem 2rem;
      text-align: center;
    }
    .products {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 2rem;
      margin-top: 2rem;
    }
    .card {
      background-color: white;
      width: 250px;
      border-radius: 15px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      overflow: hidden;
    }
    .card img {
      width: 100%;
      height: 170px;
      object-fit: cover;
    }
    .card h3 {
      margin: 1rem 0 0.5rem;
    }
    .card p {
      color: #666;
      margin-bottom: 1rem;
    }
    .order-btn {
      display: inline-block;
      margin-bottom: 1rem;
      padding: 0.6rem 1.2rem;
      background-color: #6a0dad;
      color: white;
      text-decoration: none;
      border-radius: 8px;
    }
    footer {
      background-color: #2f003f;
      color: white;
      padding: 2rem;
      text-align: center;
    }
  </style>
</head>
<body>

  <header>
    <h1>Snakista Cafe</h1>
    <p>Taste the Love, Spice the Life</p>
  </header>

  <nav>
    <a href="#home">Home</a>
    <a href="#menu">Menu</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>

  <section class="hero" id="home">
    <h1>Welcome to Snakista</h1>
  </section>

  <section class="section" id="menu">
    <h2>Our Specialties</h2>
    <div class="products">
      <div class="card">
        <img src="https://source.unsplash.com/250x170/?bhel,snacks" alt="Shuka Bhel">
        <h3>Shuka Bhel</h3>
        <p>Only ₹25</p>
        <a href="https://wa.me/917208731279?text=I%20want%20to%20order%20Shuka%20Bhel" class="order-btn">Order</a>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/250x170/?spicy-food" alt="Spicy Bhel">
        <h3>Spicy Bhel</h3>
        <p>Only ₹30</p>
        <a href="https://wa.me/917208731279?text=I%20want%20to%20order%20Spicy%20Bhel" class="order-btn">Order</a>
      </div>
      <!-- Add more cards below similarly -->
    </div>
  </section>

  <section class="section" id="about">
    <h2>About Us</h2>
    <p>We are a modern snack café that brings you the best of traditional flavors with a twist of style. Experience love in every bite!</p>
  </section>

  <section class="section" id="contact">
    <h2>Contact Us</h2>
    <p>Order via WhatsApp: <a href="https://wa.me/917208731279">+91 72087 31279</a></p>
  </section>

  <footer>
    <p>&copy; 2025 Snakista. All rights reserved.</p>
  </footer>

</body>
</html>
