<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Snakista Cafe</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom right, #f5e6ff, #e0b3ff);
      color: #3c096c;
    }
    header {
      background-color: #da70ff;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 {
      color: white;
      font-size: 1.8rem;
    }
    nav {
      display: flex;
      gap: 1rem;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    .filters {
      text-align: center;
      margin: 1rem;
    }
    .filters button {
      background-color: #da70ff;
      color: white;
      border: none;
      margin: 0.2rem;
      padding: 0.5rem 1rem;
      cursor: pointer;
      border-radius: 5px;
    }
    .filters button:hover {
      background-color: #e0aaff;
    }
    .menu-section {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1rem;
      padding: 1rem;
    }
    .item {
      background-color: #f9e6ff;
      border-radius: 10px;
      padding: 1rem;
      text-align: center;
      box-shadow: 0 0 5px #ccc;
    }
    .item img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 8px;
    }
    .item h4 {
      margin: 0.5rem 0 0.2rem;
    }
    .item p {
      margin: 0.2rem 0;
      font-weight: bold;
    }
    .order-button {
      display: inline-block;
      background-color: #c77dff;
      color: white;
      text-align: center;
      padding: 0.5rem;
      border-radius: 5px;
      text-decoration: none;
      font-weight: bold;
      margin-top: 0.5rem;
    }
    .order-button:hover {
      background-color: #a64dff;
    }
    section {
      padding: 2rem 1rem;
    }
    footer {
      background-color: #b565e0;
      color: white;
      text-align: center;
      padding: 1rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Snakista Café</h1>
    <nav>
      <a href="#menu">Menu</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="menu">
    <h2 style="text-align:center">Our Menu</h2>
    <div class="filters">
      <button onclick="filterItems('all')">All</button>
      <button onclick="filterItems('Bhel & mixes')">Bhel & mixes</button>
      <button onclick="filterItems('specialplates')">special plates</button>
      <button onclick="filterItems('Sweet munchies')">Sweet munchies</button>
      <button onclick="filterItems('snack')">Snacks</button>
    </div>
    <div class="menu-section" id="menu-items"></div>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p style="max-width: 600px; margin: auto; text-align: center">
      Snakista Café is a cozy corner for coffee lovers and foodies. We specialize in brewing happiness in every cup and baking joy into every bite. Come visit us and taste the snakista's magic!
    </p>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <p style="text-align: center">📞 +91 72087 31279 | 📍 Mumbai, India</p>
  </section>

  <footer>
    &copy; 2025 Snakista Café | Designed with 💜
  </footer>

  <script>
    const products = [
      { name: 'Dry spicy bhel', price: 150, category: 'Bhel & mixes', img: 'cappuccino' },
      { name: 'khata meetha', price: 160, category: 'Bhel & mixes', img: 'latte' },
      { name: 'Frali mix', price: 140, category: 'Bhel & mixes', img: 'espresso' },
      { name: 'Mocha', price: 170, category: 'Bhel & mixes', img: 'mocha' },
      { name: 'Navratan mix', price: 130, category: 'Bhel & mixes', img: 'americano' },
      { name: 'Poha', price: 180, category: 'Bhel & mixes', img: 'coldbrew' },

      { name: 'Masala Chai', price: 120, category: 'special plates ', img: 'chai' },
      { name: 'Green Tea', price: 110, category: 'special plates', img: 'green-tea' },
      { name: 'Lemon Tea', price: 115, category: 'special plates', img: 'lemon-tea' },
      { name: 'Herbal Tea', price: 130, category: 'specialplates', img: 'herbal-tea' },
      { name: 'Milk Tea', price: 125, category: 'special plates', img: 'milk-tea' },
      { name: 'Iced Tea', price: 140, category: 'special plates', img: 'iced-tea' },

      { name: 'sev', price: 140, category: 'snack', img: 'sandwich' },
      { name: 'ghatiya', price: 130, category: 'snack', img: 'fries' },
      { name: 'Samosa', price: 50, category: 'snack', img: 'samosa' },
      { name: 'papdi', price: 150, category: 'snack', img: 'burger' },
      { name: 'chakli', price: 120, category: 'snack', img: 'roll' },
      { name: 'chivda', price: 140, category: 'snack', img: 'nachos' },
      { name: 'sakrpara', price: 170, category: 'snack', img: 'hot-chocolate' },
      { name: 'garlic chivada', price: 200, category: 'snack', img: 'affogato' },
      { name: 'Garlic Bread', price: 90, category: 'snack', img: 'ice-cream' },
      { name: 'Pudding', price: 120, category: 'snack', img: 'pudding' },

      { name: 'Tiramisu', price: 220, category: 'Sweet munchies', img: 'tiramisu' },
      { name: 'Garlic Bread', price: 110, category: 'Sweet munchies', img: 'garlic-bread' },
      { name: 'Paneer Tikka', price: 180, category: 'Sweet munchies', img: 'paneer-tikka' },
      { name: 'Fruit Salad', price: 100, category: 'Sweet munchies', img: 'fruit-salad' },
      { name: 'Chocolate Cake', price: 200, category: 'Sweet munchies', img: 'cake' },
      { name: 'Donut', price: 100, category: 'Sweet munchies', img: 'donut' },
      { name: 'Brownie', price: 130, category: 'Sweet munchies', img: 'brownie' },
      { name: 'Cupcake', price: 110, category: 'Sweet munchies', img: 'cupcake' },
      
    ];

    document.addEventListener("DOMContentLoaded", () => {
      const container = document.getElementById("menu-items");
      container.innerHTML = products.map(p => `
        <div class="item ${p.category}">
          <img src="https://source.unsplash.com/600x400/?${p.img}" alt="${p.name}">
          <h4>${p.name}</h4>
          <p>₹${p.price}</p>
          <a class="order-button" target="_blank" href="https://wa.me/917208731279?text=I%20want%20to%20order%20${encodeURIComponent(p.name)}">Order</a>
        </div>
      `).join('');
    });

    function filterItems(category) {
      const items = document.querySelectorAll('.item');
      items.forEach(item => {
        item.style.display = (category === 'all' || item.classList.contains(category)) ? 'block' : 'none';
      });
    }
  </script>
</body>
</html>
