<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Alifaannoo</title>
    <style>
      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
          sans-serif;
      }
      body {
        background: #000;
        color: #fff;
        scroll-behavior: smooth;
      }
      a {
        text-decoration: none;
      }

      .navbar {
        display: flex;
        justify-content: space-between;
        padding: 20px 40px;
        background: #000;
      }
      .navbar .logo {
        font-size: 24px;
        font-weight: 600;
      }
      .navbar .btn {
        background: #fff;
        color: #000;
        padding: 8px 20px;
        border-radius: 30px;
      }

      .hero {
        text-align: center;
        padding: 120px 20px 80px;
      }
      .hero h1 {
        font-size: 60px;
        font-weight: 700;
        line-height: 1.1;
      }
      .hero p {
        font-size: 20px;
        color: #aaa;
        margin-top: 20px;
      }
      .hero-btn {
        display: inline-block;
        margin-top: 40px;
        padding: 14px 32px;
        background: #fff;
        color: #000;
        border-radius: 30px;
        font-size: 16px;
      }

      .products {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
        gap: 30px;
        padding: 60px 40px;
      }
      .product {
        background: #fff;
        color: #000;
        border-radius: 20px;
        padding: 30px;
        text-align: center;
        transition: transform 0.3s ease, box-shadow 0.3s ease;
      }
      .product:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 20px rgba(255, 255, 255, 0.1);
      }
      .product img {
        width: 120px;
        margin-bottom: 20px;
      }
      .product h2 {
        font-size: 24px;
        font-weight: 600;
      }
      .product p {
        color: #555;
        margin: 16px 0 24px;
      }
      .product-btn {
        display: inline-block;
        padding: 10px 24px;
        border-radius: 30px;
        background: #000;
        color: #fff;
        font-size: 14px;
      }

      .order-form {
        max-width: 500px;
        margin: 60px auto;
        padding: 0 20px;
      }
      .order-form h1 {
        text-align: center;
        font-size: 36px;
        margin-bottom: 30px;
      }
      .order-form form {
        display: flex;
        flex-direction: column;
        gap: 20px;
      }
      .order-form label {
        font-size: 16px;
        font-weight: 500;
      }
      .order-form input,
      .order-form select {
        padding: 14px 16px;
        border-radius: 12px;
        border: none;
        background: #222;
        color: #fff;
        font-size: 16px;
      }
      .order-form input::placeholder {
        color: #aaa;
      }
      .order-form button {
        margin-top: 10px;
        padding: 14px;
        background: #fff;
        color: #000;
        border-radius: 30px;
        font-size: 16px;
      }

      footer {
        text-align: center;
        padding: 40px 20px;
        color: #555;
        font-size: 14px;
        margin-top: 60px;
      }
    </style>
  </head>
  <body>
    <!-- Navbar -->
    <nav class="navbar">
      <div class="logo">Alifaannoo</div>
      <a href="#order" class="btn">Top Up</a>
    </nav>

    <!-- Hero -->
    <section class="hero">
      <h1>Top Up Diamonds Instan</h1>
      <p>Mobile Legends & Free Fire</p>
      <a href="#products" class="hero-btn">Mulai Sekarang</a>
    </section>

    <!-- Produk -->
    <section class="products" id="products">
      <div class="product">
        <img src="https://i.postimg.cc/YCV2QBJg/ml.png" alt="Mobile Legends" />
        <h2>Mobile Legends</h2>
        <p>Diamond ML harga terbaik & instan.</p>
        <a href="#order" class="product-btn">Top Up</a>
      </div>

      <div class="product">
        <img src="https://i.postimg.cc/V6q7qJK9/ff.png" alt="Free Fire" />
        <h2>Free Fire</h2>
        <p>Diamond FF aman & cepat tanpa ribet.</p>
        <a href="#order" class="product-btn">Top Up</a>
      </div>
    </section>

    <!-- Order Form -->
    <section class="order-form" id="order">
      <h1>Isi Diamond Sekarang</h1>
      <form action="#" method="POST">
        <label for="game">Pilih Game</label>
        <select id="game" name="game" required>
          <option value="">-- Pilih --</option>
          <option value="ML">Mobile Legends</option>
          <option value="FF">Free Fire</option>
        </select>

        <label for="userid">User ID</label>
        <input
          type="text"
          id="userid"
          name="userid"
          placeholder="Masukkan User ID"
          required
        />

        <label for="zone">Zone ID (Opsional)</label>
        <input
          type="text"
          id="zone"
          name="zone"
          placeholder="Masukkan Zone ID"
        />

        <label for="nominal">Nominal Diamond</label>
        <select id="nominal" name="nominal" required>
          <option value="">-- Pilih Nominal --</option>
          <option value="86">86 Diamond</option>
          <option value="172">172 Diamond</option>
          <option value="257">257 Diamond</option>
          <option value="514">514 Diamond</option>
        </select>

        <button type="submit">Bayar Sekarang</button>
      </form>
    </section>

    <footer>© 2025 Alifaannoo. All rights reserved.</footer>
  </body>
</html>
    
