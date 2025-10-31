<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ShopEasy</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f8f9fa;
    }

    /* Navbar */
    header {
      background-color: #222;
      color: white;
      padding: 15px 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    header h1 {
      font-size: 24px;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
    }

    nav a:hover {
      color: #ff9800;
    }

    /* Products grid */
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
      padding: 30px;
    }

    .product {
      background: white;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      padding: 15px;
      text-align: center;
      transition: transform 0.2s;
    }

    .product:hover {
      transform: scale(1.03);
    }

    .product img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
    }

    .product h3 {
      margin: 10px 0 5px;
    }

    .product p {
      color: #666;
    }

    .product button {
      background-color: #ff9800;
      border: none;
      color: white;
      padding: 10px 20px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 14px;
    }

    .product button:hover {
      background-color: #e68900;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 15px;
      background-color: #222;
      color: white;
      margin-top: 20px;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <header>
    <h1>🛒 ShopEasy</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#">Shop</a>
      <a href="#">Cart</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <!-- Product Section -->
  <section class="products">
    <div class="product">
      <img src="https://via.placeholder.com/200x200" alt="Product 1">
      <h3>Wireless Headphones</h3>
      <p>₹1,499</p>
      <button onclick="addToCart('Wireless Headphones')">Add to Cart</button>
    </div>

    <div class="product">
      <img src="https://via.placeholder.com/200x200" alt="Product 2">
      <h3>Smart Watch</h3>
      <p>₹2,999</p>
      <button onclick="addToCart('Smart Watch')">Add to Cart</button>
    </div>

    <div class="product">
      <img src="https://via.placeholder.com/200x200" alt="Product 3">
      <h3>Sneakers</h3>
      <p>₹1,999</p>
      <button onclick="addToCart('Sneakers')">Add to Cart</button>
    </div>

    <div class="product">
      <img src="https://via.placeholder.com/200x200" alt="Product 4">
      <h3>Bluetooth Speaker</h3>
      <p>₹899</p>
      <button onclick="addToCart('Bluetooth Speaker')">Add to Cart</button>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 ShopEasy. All rights reserved.</p>
  </footer>

  <script>
    function addToCart(product) {
      alert(product + " added to cart!");
    }
  </script>

</body>
</html>
