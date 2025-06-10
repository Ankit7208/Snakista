<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Snakista Café</title>
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
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
      padding: 1rem;
      max-width: 1000px;
      margin: auto;
    }

    .item {
      background-color: #f9e6ff;
      border-radius: 12px;
      padding: 1rem;
      text-align: center;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
      transition: transform 0.2s ease;
    }

    .item:hover {
      transform: translateY(-4px);
    }

    .item img {
      width: 100%;
      aspect-ratio: 4/3;
      object-fit: cover;
      border-radius: 12px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }

    .item img:hover {
      transform: scale(1.03);
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
      margin-top: 0.5rem;
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
      <button onclick="filterItems('coffee')">Coffee</button>
      <button onclick="filterItems('tea')">Tea</button>
      <button onclick="filterItems('dessert')">Desserts</button>
      <button onclick="filterItems('snack')">Snacks</button>
    </div>
    <div class="menu-section" id="menu-items">
      <!-- Items will be rendered here -->
    </div>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p style="max-width: 600px; margin: auto; text-align: center">
