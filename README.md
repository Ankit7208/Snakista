<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Purple Cafe</title>
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
      grid-template-columns: repeat(4, 1fr);
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
      height: 150px;
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
    .item a button {
      background-color: #c77dff;
      color: white;
      border: none;
      padding: 0.5rem;
      width: 100%;
      border-radius: 5px;
      cursor: pointer;
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
    <h1>Purple Café</h1>
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
      <button onclick="filterItems('coffee')">Coffee</button>
      <button onclick="filterItems('tea')">Tea</button>
      <button onclick="filterItems('dessert')">Desserts</button>
      <button onclick="filterItems('snack')">Snacks</button>
    </div>
    <div class="menu-section" id="menu-items">
      <!-- 30 products -->
      <script>
        const products = [
          { name: 'Cappuccino', price: 150, category: 'coffee', img: 'cappuccino' },
          { name: 'Latte', price: 160, category: 'coffee', img: 'latte' },
          { name: 'Espresso', price: 140, category: 'coffee', img: 'espresso' },
          { name: 'Mocha', price: 170, category: 'coffee', img: 'mocha' },
          { name: 'Americano', price: 130, category: 'coffee', img: 'americano' },
          { name: 'Cold Brew', price: 180, category: 'coffee', img: 'coldbrew' },

          { name: 'Masala Chai', price: 120, category: 'tea', img: 'chai' },
          { name: 'Green Tea', price: 110, category: 'tea', img: 'green-tea' },
          { name: 'Lemon Tea', price: 115, category: 'tea', img: 'lemon-tea' },
          { name: 'Herbal Tea', price: 130, category: 'tea', img: 'herbal-tea' },
