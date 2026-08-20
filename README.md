# stylemart
one in two<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>StyleMart - Fashion Store</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f5f5f5;
      color: #222;
    }

    /* NAVBAR */
    .navbar {
      background: #111;
      color: white;
      padding: 18px 5%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
      flex-wrap: wrap;
    }

    .logo {
      font-size: 28px;
      font-weight: bold;
      color: #ffcc00;
    }

    .nav-links {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }

    .nav-links a {
      color: white;
      text-decoration: none;
      cursor: pointer;
    }

    .nav-links a:hover {
      color: #ffcc00;
    }

    .cart {
      font-size: 18px;
    }

    /* HERO */
    .hero {
      min-height: 450px;
      background: linear-gradient(135deg, #111, #444);
      color: white;

      display: flex;
      align-items: center;
      justify-content: center;

      text-align: center;
      padding: 30px;
    }

    .hero h1 {
      font-size: 55px;
      margin-bottom: 15px;
    }

    .hero p {
      font-size: 22px;
      margin-bottom: 25px;
    }

    .hero button {
      background: #ffcc00;
      border: none;
      padding: 14px 30px;
      font-size: 17px;
      font-weight: bold;
      border-radius: 5px;
      cursor: pointer;
    }

    .hero button:hover {
      background: white;
    }

    /* SEARCH */
    .search {
      text-align: center;
      padding: 30px 20px;
    }

    .search input {
      width: 600px;
      max-width: 100%;
      padding: 15px 20px;
      border: 1px solid #ccc;
      border-radius: 30px;
      font-size: 16px;
      outline: none;
    }

    /* CATEGORY */
    .category-buttons {
      display: flex;
      justify-content: center;
      gap: 10px;
      flex-wrap: wrap;
      padding: 10px 20px 30px;
    }

    .category-buttons button {
      border: none;
      padding: 12px 20px;
      border-radius: 25px;
      background: white;
      cursor: pointer;
      box-shadow: 0 2px 8px #ddd;
    }

    .category-buttons button:hover {
      background: #111;
      color: white;
    }

    /* PRODUCTS */
    .title {
      text-align: center;
      font-size: 32px;
      margin: 20px 0 30px;
    }

    .products {
      width: 90%;
      max-width: 1200px;
      margin: auto;

      display: grid;
      grid-template-columns: repeat(
        auto-fit,
        minmax(220px, 1fr)
      );

      gap: 25px;
    }

    .product {
      background: white;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 4px 15px #ddd;
      transition: 0.3s;
    }

    .product:hover {
      transform: translateY(-7px);
    }

    .product-image {
      height: 220px;
      background: #eee;

      display: flex;
      align-items: center;
      justify-content: center;

      font-size: 90px;
    }

    .product-info {
      padding: 18px;
    }

    .product-info small {
      color: #777;
    }

    .product-info h3 {
      margin: 10px 0;
    }

    .price {
      font-size: 22px;
      font-weight: bold;
      margin-bottom: 15px;
    }

    .add-cart {
      width: 100%;
      border: none;
      padding: 12px;
      background: #111;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }

    .add-cart:hover {
      background: #ffcc00;
      color: #111;
    }

    /* CART */
    .cart-section {
      width: 90%;
      max-width: 900px;
      margin: 60px auto;
      background: white;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 3px 15px #ddd;
    }

    .cart-section h2 {
      margin-bottom: 20px;
    }

    .cart-item {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 15px;
      padding: 15px 0;
      border-bottom: 1px solid #ddd;
    }

    .remove {
      background: red;
      color: white;
      border: none;
      padding: 7px 12px;
      border-radius: 4px;
      cursor: pointer;
    }

    .total {
      text-align: right;
      margin-top: 20px;
      font-size: 22px;
    }

    /* FOOTER */
    footer {
      background: #111;
      color: white;
      text-align: center;
      padding: 40px 20px;
      margin-top: 60px;
    }

    footer h2 {
      color: #ffcc00;
      margin-bottom: 10px;
    }

    footer p {
      color: #ccc;
      margin: 7px;
    }

    /* MOBILE */
    @media (max-width: 768px) {

      .navbar {
        flex-direction: column;
      }

      .nav-links {
        justify-content: center;
      }

      .hero {
        min-height: 350px;
      }

      .hero h1 {
        font-size: 38px;
      }

      .hero p {
        font-size: 18px;
      }

      .cart-item {
        flex-direction: column;
        align-items: flex-start;
      }

      .total {
        text-align: left;
      }
    }

    @media (max-width: 480px) {

      .hero h1 {
        font-size: 30px;
      }

      .products {
        width: 94%;
        grid-template-columns: 1fr;
      }

      .product-image {
        height: 200px;
      }
    }
  </style>
</head>

<body>

  <!-- NAVBAR -->

  <nav class="navbar">

    <div class="logo">
      StyleMart
    </div>

    <div class="nav-links">

      <a href="#">Home</a>

      <a href="#products">
        Men
      </a>

      <a href="#products">
        Women
      </a>

      <a href="#products">
        Shoes
      </a>

      <a href="#products">
        Watches
      </a>

    </div>

    <div class="cart">
      🛒 Cart:
      <span id="cartCount">0</span>
    </div>

  </nav>


  <!-- HERO -->

  <section class="hero">

    <div>

      <h1>
        Style For Everyone
      </h1>

      <p>
        Men & Women Clothes, Shoes and Watches
      </p>

      <button onclick="showAll()">
        Shop Now
      </button>

    </div>

  </section>


  <!-- SEARCH -->

  <div class="search">

    <input
      type="text"
      id="searchInput"
      placeholder="Search clothes, shoes, watches..."
      onkeyup="searchProducts()"
    >

  </div>


  <!-- CATEGORY BUTTONS -->

  <div class="category-buttons">

    <button onclick="filterProducts('all')">
      All
    </button>

    <button onclick="filterProducts('men-clothes')">
      👕 Men Clothes
    </button>

    <button onclick="filterProducts('men-shoes')">
      👟 Men Shoes
    </button>

    <button onclick="filterProducts('watches')">
      ⌚ Watches
    </button>

    <button onclick="filterProducts('women-clothes')">
      👗 Women Clothes
    </button>

    <button onclick="filterProducts('women-shoes')">
      👠 Women Shoes
    </button>

  </div>


  <!-- PRODUCTS -->

  <h2 class="title" id="products">
    Our Products
  </h2>

  <div class="products">


    <!-- PRODUCT 1 -->

    <div class="product men-clothes">

      <div class="product-image">
        👕
      </div>

      <div class="product-info">

        <small>
          Men Clothes
        </small>

        <h3>
          Men's T-Shirt
        </h3>

        <div class="price">
          ₹599
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Men T-Shirt', 599)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 2 -->

    <div class="product men-clothes">

      <div class="product-image">
        👔
      </div>

      <div class="product-info">

        <small>
          Men Clothes
        </small>

        <h3>
          Men's Shirt
        </h3>

        <div class="price">
          ₹999
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Men Shirt', 999)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 3 -->

    <div class="product men-clothes">

      <div class="product-image">
        👖
      </div>

      <div class="product-info">

        <small>
          Men Clothes
        </small>

        <h3>
          Men's Jeans
        </h3>

        <div class="price">
          ₹1299
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Men Jeans', 1299)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 4 -->

    <div class="product men-shoes">

      <div class="product-image">
        👟
      </div>

      <div class="product-info">

        <small>
          Men Shoes
        </small>

        <h3>
          Sports Shoes
        </h3>

        <div class="price">
          ₹1799
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Sports Shoes', 1799)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 5 -->

    <div class="product men-shoes">

      <div class="product-image">
        🥾
      </div>

      <div class="product-info">

        <small>
          Men Shoes
        </small>

        <h3>
          Casual Shoes
        </h3>

        <div class="price">
          ₹1499
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Casual Shoes', 1499)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 6 -->

    <div class="product watches">

      <div class="product-image">
        ⌚
      </div>

      <div class="product-info">

        <small>
          Watches
        </small>

        <h3>
          Smart Watch
        </h3>

        <div class="price">
          ₹2499
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Smart Watch', 2499)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 7 -->

    <div class="product watches">

      <div class="product-image">
        ⌚
      </div>

      <div class="product-info">

        <small>
          Watches
        </small>

        <h3>
          Classic Watch
        </h3>

        <div class="price">
          ₹1999
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Classic Watch', 1999)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 8 -->

    <div class="product women-clothes">

      <div class="product-image">
        👗
      </div>

      <div class="product-info">

        <small>
          Women Clothes
        </small>

        <h3>
          Women's Dress
        </h3>

        <div class="price">
          ₹1299
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Women Dress', 1299)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 9 -->

    <div class="product women-clothes">

      <div class="product-image">
        👚
      </div>

      <div class="product-info">

        <small>
          Women Clothes
        </small>

        <h3>
          Women's Top
        </h3>

        <div class="price">
          ₹699
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Women Top', 699)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 10 -->

    <div class="product women-clothes">

      <div class="product-image">
        👗
      </div>

      <div class="product-info">

        <small>
          Women Clothes
        </small>

        <h3>
          Women's Kurti
        </h3>

        <div class="price">
          ₹899
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Women Kurti', 899)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 11 -->

    <div class="product women-shoes">

      <div class="product-image">
        👠
      </div>

      <div class="product-info">

        <small>
          Women Shoes
        </small>

        <h3>
          Women's Heels
        </h3>

        <div class="price">
          ₹1599
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Women Heels', 1599)"
        >
          Add To Cart
        </button>

      </div>

    </div>


    <!-- PRODUCT 12 -->

    <div class="product women-shoes">

      <div class="product-image">
        👟
      </div>

      <div class="product-info">

        <small>
          Women Shoes
        </small>

        <h3>
          Women's Sneakers
        </h3>

        <div class="price">
          ₹1399
        </div>

        <button
          class="add-cart"
          onclick="addToCart('Women Sneakers', 1399)"
        >
          Add To Cart
        </button>

      </div>

    </div>

  </div>


  <!-- CART -->

  <section class="cart-section">

    <h2>
      Your Cart 🛒
    </h2>

    <div id="cartItems">
      <p>
        Your cart is empty.
      </p>
    </div>

    <h3 class="total">
      Total: ₹<span id="total">0</span>
    </h3>

  </section>


  <!-- FOOTER -->

  <footer>

    <h2>
      StyleMart
    </h2>

    <p>
      Fashion For Men & Women
    </p>

    <p>
      Clothes • Shoes • Watches
    </p>

    <p>
      © 2026 StyleMart
    </p>

  </footer>


  <!-- JAVASCRIPT -->

  <script>

    let cart = [];

    function addToCart(name, price) {

      cart.push({
        name: name,
        price: price
      });

      updateCart();

    }


    function updateCart() {

      const cartItems =
        document.getElementById("cartItems");

      const cartCount =
        document.getElementById("cartCount");

      const total =
        document.getElementById("total");

      cartCount.innerText = cart.length;

      if (cart.length === 0) {

        cartItems.innerHTML =
          "<p>Your cart is empty.</p>";

        total.innerText = "0";

        return;

      }

      let html = "";
      let totalPrice = 0;

      cart.forEach(function(item, index) {

        totalPrice += item.price;

        html += `
          <div class="cart-item">

            <span>
              ${item.name}
            </span>

            <strong>
              ₹${item.price}
            </strong>

            <button
              class="remove"
              onclick="removeItem(${index})"
            >
              Remove
            </button>

          </div>
        `;

      });

      cartItems.innerHTML = html;

      total.innerText = totalPrice;

    }


    function removeItem(index) {

      cart.splice(index, 1);

      updateCart();

    }


    function filterProducts(category) {

      const products =
        document.querySelectorAll(".product");

      products.forEach(function(product) {

        if (category === "all") {

          product.style.display = "block";

        } else {

          if (
            product.classList.contains(category)
          ) {

            product.style.display = "block";

          } else {

            product.style.display = "none";

          }

        }

      });

    }


    function searchProducts() {

      const search =
        document
          .getElementById("searchInput")
          .value
          .toLowerCase();

      const products =
        document.querySelectorAll(".product");

      products.forEach(function(product) {

        const name =
          product
            .querySelector("h3")
            .innerText
            .toLowerCase();

        if (name.includes(search)) {

          product.style.display = "block";

        } else {

          product.style.display = "none";

        }

      });

    }


    function showAll() {

      document
        .getElementById("products")
        .scrollIntoView({
          behavior: "smooth"
        });

      filterProducts("all");

    }

  </script>

</body>
</html>
