<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Snakista - Taste the Tradition!</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      background-color: #fff0f8;
      color: #333;
    }
    header, nav, footer {
      background-color: #800080;
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
      color: #800080;
    }
    .section {
      padding: 2em;
      text-align: center;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1em;
      margin-top: 1em;
    }
    .product {
      background: #fff;
      border-radius: 15px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      padding: 1em;
    }
    .product img {
      width: 100%;
      height: 150px;
      object-fit: cover;
      border-radius: 10px;
    }
    .btn {
      display: inline-block;
      margin-top: 1em;
      padding: 0.5em 1em;
      background-color: #800080;
      color: white;
      text-decoration: none;
      border-radius: 5px;
    }
    footer {
      margin-top: 2em;
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
    <a href="#about">About</a>
    <a href="#products">Products</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="home" class="section">
    <h2>Welcome to Snakista!</h2>
    <p>Delicious dry snacks, fresh mixes & desi flavours served with love.</p>
  </section>

  <section id="about" class="section">
    <h2>About Us</h2>
    <p>Snakista brings you the best of Indian traditional snacks with a modern twist. We focus on quality, taste and customer happiness.</p>
  </section>

  <section id="products" class="section">
    <h2>Our Menu</h2>

    <h3>Bhel & Mixes</h3>
    <div class="products">
      <div class="product">
        <img src="https://source.unsplash.com/200x150/?bhel" alt="Shuka Bhel">
        <h4>Shuka Bhel - ₹25</h4>
        <a class="btn" href="https://wa.me/917208731279?text=I want to order Shuka Bhel">Order Now</a>
      </div>
      <div class="product">
        <img src="https://source.unsplash.com/200x150/?bhel,puffedrice" alt="Spicy Bhel">
        <h4>Spicy Bhel - ₹30</h4>
        <a class="btn" href="https://wa.me/917208731279?text=I want to order Spicy Bhel">Order Now</a>
      </div>
      <div class="product">
        <img src="https://source.unsplash.com/200x150/?namkeen" alt="Mixed Chaat">
        <h4>Mixed Chaat - ₹35</h4>
        <a class="btn" href="https://wa.me/917208731279?text=I want to order Mixed Chaat">Order Now</a>
      </div>
    </div>

    <h3>Bhujia & Namkeen</h3>
    <div class="products">
      <div class="product">
        <img src="https://source.unsplash.com/200x150/?bhujia" alt="Aloo Bhujia">
        <h4>Aloo Bhujia - ₹30</h4>
        <a class="btn" href="https://wa.me/917208731279?text=I want to order Aloo Bhujia">Order Now</a>
      </div>
      <div class="product">
        <img src="https://source.unsplash.com/200x150/?moongdal" alt="Moong Dal">
        <h4>Moong Dal - ₹40</h4>
        <a class="btn" href="https://wa.me/917208731279?text=I want to order Moong Dal">Order Now</a>
      </div>
      <div class="product">
        <img src="https://source.unsplash.com/200x150/?namkeen" alt="Masala Peanuts">
        <h4>Masala Peanuts - ₹35</h4>
        <a class="btn" href="https://wa.me/917208731279?text=I want to order Masala Peanuts">Order Now</a>
      </div>
    </div>

    <h3>Beverages</h3>
    <div class="products">
      <div class="product">
        <img src="https://source.unsplash.com/200x150/?chai" alt="Masala Chai">
        <h4>Masala Chai - ₹15</h4>
        <a class="btn" href="https://wa.me/917208731279?text=I want to order Masala Chai">Order Now</a>
      </div>
      <div class="product">
        <img src="https://source.unsplash.com/200x150/?coffee" alt="Filter Coffee">
        <h4>Filter Coffee - ₹25</h4>
        <a class="btn" href="https://wa.me/917208731279?text=I want to order Filter Coffee">Order Now</a>
      </div>
    </div>

    <h3>Combos</h3>
    <div class="products">
      <div class="product">
        <img src="https://source.unsplash.com/200x150/?snacks,tea" alt="Combo Pack">
        <h4>Combo Pack (Chai + Nasta) - ₹89</h4>
        <a class="btn" href="https://wa.me/917208731279?text=I want to order Combo Pack">Order Now</a>
      </div>
    </div>
  </section>

  <section id="contact" class="section">
    <h2>Contact Us</h2>
    <p>Phone/WhatsApp: <a href="https://wa.me/917208731279">+91 72087 31279</a></p>
    <p>Email: snakista@gmail.com</p>
  </section>

  <footer>
    <p>&copy; 2025 Snakista. All rights reserved.</p>
  </footer>
</body>
</html>
