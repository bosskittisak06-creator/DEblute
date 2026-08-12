# DEblute
<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>DEBLUTE - Flower Design</title>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;600&family=Prompt:wght@300;400;500;600&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Prompt', sans-serif;
    }

    body {
      background-color: #fdfbf7; /* สีครีมอ่อน นุ่มนวล */
      color: #4a4238;
      line-height: 1.6;
    }

    /* Top Announcement Bar */
    .top-bar {
      background-color: #e6dac8;
      text-align: center;
      padding: 0.4rem;
      font-size: 0.85rem;
      color: #5c4e3e;
      letter-spacing: 0.5px;
    }

    /* Header & Brand Logo */
    header {
      background-color: #f7f1e5;
      text-align: center;
      padding: 2.5rem 1rem;
      border-bottom: 1px solid #ebd3;
    }

    .brand-logo {
      font-family: 'Cinzel', serif;
      font-size: 2.8rem;
      font-weight: 600;
      letter-spacing: 6px;
      color: #3b3123;
      margin-bottom: 0.2rem;
    }

    .brand-sub {
      font-size: 0.85rem;
      letter-spacing: 3px;
      color: #8c765c;
      text-transform: uppercase;
    }

    /* Navigation Bar */
    nav {
      background-color: #ffffff;
      border-bottom: 1px solid #ece4d8;
      position: sticky;
      top: 0;
      z-index: 100;
      box-shadow: 0 2px 5px rgba(0,0,0,0.02);
    }

    nav ul {
      display: flex;
      justify-content: center;
      list-style: none;
      flex-wrap: wrap;
    }

    nav a {
      display: block;
      padding: 0.9rem 1.4rem;
      text-decoration: none;
      color: #52473b;
      font-size: 0.9rem;
      font-weight: 400;
      transition: all 0.3s ease;
    }

    nav a:hover, nav a.active {
      color: #a37d55;
      background-color: #fdfbf7;
    }

    /* Main Container */
    .container {
      max-width: 1200px;
      margin: 2.5rem auto;
      padding: 0 1.5rem;
    }

    .category-title {
      font-size: 1.6rem;
      font-weight: 500;
      text-align: center;
      color: #3b3123;
      margin-bottom: 0.3rem;
    }

    .category-subtitle {
      text-align: center;
      color: #8c765c;
      font-size: 0.9rem;
      margin-bottom: 2rem;
    }

    /* Product Grid Structure */
    .product-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
      gap: 2rem;
    }

    /* Product Card */
    .product-card {
      background: #ffffff;
      border: 1px solid #f0e6d8;
      border-radius: 6px;
      overflow: hidden;
      text-align: center;
      padding-bottom: 1.5rem;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .product-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 20px rgba(0,0,0,0.05);
    }

    .product-image-wrap {
      width: 100%;
      height: 280px;
      background-color: #f5efe6;
      overflow: hidden;
    }

    .product-image-wrap img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.5s ease;
    }

    .product-card:hover .product-image-wrap img {
      transform: scale(1.05);
    }

    .product-card h3 {
      font-size: 1.1rem;
      font-weight: 500;
      color: #3b3123;
      margin: 1.2rem 0 0.4rem;
    }

    .price-container {
      margin-bottom: 1rem;
    }

    .original-price {
      text-decoration: line-through;
      color: #a89a8b;
      font-size: 0.88rem;
      margin-right: 0.4rem;
    }

    .sale-price {
      color: #b05843;
      font-weight: 600;
      font-size: 1.15rem;
    }

    .btn-cart {
      background-color: #8c7355;
      color: #ffffff;
      border: none;
      padding: 0.65rem 1.4rem;
      border-radius: 4px;
      cursor: pointer;
      font-size: 0.88rem;
      letter-spacing: 0.5px;
      transition: background-color 0.3s ease;
    }

    .btn-cart:hover {
      background-color: #6b563d;
    }

    /* Footer Section */
    footer {
      background-color: #f2e9dc;
      color: #5c4e3e;
      padding: 3rem 1.5rem 1.5rem;
      margin-top: 4rem;
      border-top: 1px solid #e0d4c3;
    }

    .footer-content {
      max-width: 1200px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 2rem;
      margin-bottom: 2rem;
      text-align: left;
    }

    .footer-col h4 {
      font-family: 'Cinzel', serif;
      font-size: 1.1rem;
      margin-bottom: 0.8rem;
      color: #3b3123;
    }

    .footer-col p, .footer-col a {
      font-size: 0.88rem;
      color: #6e5e4d;
      text-decoration: none;
      margin-bottom: 0.4rem;
      display: block;
    }

    .footer-bottom {
      text-align: center;
      border-top: 1px solid #e0d4c3;
      padding-top: 1.5rem;
      font-size: 0.8rem;
      color: #8c7b69;
    }
  </style>
</head>
<body>

  <div class="top-bar">
    บริการจัดส่งช่อดอกไม้และกระเช้าดอกไม้ด่วน ในเขตกรุงเทพฯ และปริมณฑล
  </div>

  <header>
    <div class="brand-logo">DEBLUTE</div>
    <div class="brand-sub">FLOWER DESIGN & HOUSE</div>
  </header>

  <nav>
    <ul>
      <li><a href="#">หน้าหลัก</a></li>
      <li><a href="#">ช่อดอกไม้</a></li>
      <li><a href="#" class="active">กระเช้าดอกไม้</a></li>
      <li><a href="#">แจกันดอกไม้</a></li>
      <li><a href="#">กล่องดอกไม้</a></li>
      <li><a href="#">เกี่ยวกับเรา</a></li>
      <li><a href="#">ติดต่อเรา</a></li>
    </ul>
  </nav>

  <div class="container">
    <h2 class="category-title">กระเช้าดอกไม้</h2>
    <p class="category-subtitle">เลือกสรรกระเช้าดอกไม้สดพรีเมียม จัดแต่งอย่างประณีตเพื่อโอกาสพิเศษของคุณ</p>

    <div class="product-grid">

      <!-- สินค้า 1 -->
      <div class="product-card">
        <div class="product-image-wrap">
          <img src="https://via.placeholder.com/400x400/f2e9dc/8c7355?text=DEBLUTE+Basket+01" alt="กระเช้าดอกไม้ DEBLUTE Basket 001">
        </div>
        <h3>Basket 001</h3>
        <div class="price-container">
          <span class="original-price">4,500 ฿</span>
          <span class="sale-price">3,000 ฿</span>
        </div>
        <button class="btn-cart">หยิบใส่ตะกร้า</button>
      </div>

      <!-- สินค้า 2 -->
      <div class="product-card">
        <div class="product-image-wrap">
          <img src="https://via.placeholder.com/400x400/f2e9dc/8c7355?text=DEBLUTE+Basket+02" alt="กระเช้าดอกไม้ DEBLUTE Basket 002">
        </div>
        <h3>Basket 002</h3>
        <div class="price-container">
          <span class="original-price">4,500 ฿</span>
          <span class="sale-price">2,890 ฿</span>
        </div>
        <button class="btn-cart">หยิบใส่ตะกร้า</button>
      </div>

      <!-- สินค้า 3 -->
      <div class="product-card">
        <div class="product-image-wrap">
          <img src="https://via.placeholder.com/400x400/f2e9dc/8c7355?text=DEBLUTE+Basket+03" alt="กระเช้าดอกไม้ DEBLUTE Basket 003">
        </div>
        <h3>Basket 003</h3>
        <div class="price-container">
          <span class="original-price">3,500 ฿</span>
          <span class="sale-price">1,890 ฿</span>
        </div>
        <button class="btn-cart">หยิบใส่ตะกร้า</button>
      </div>

      <!-- สินค้า 4 -->
      <div class="product-card">
        <div class="product-image-wrap">
          <img src="https://via.placeholder.com/400x400/f2e9dc/8c7355?text=DEBLUTE+Basket+04" alt="กระเช้าดอกไม้ DEBLUTE Basket 004">
        </div>
        <h3>Basket 004</h3>
        <div class="price-container">
          <span class="original-price">3,500 ฿</span>
          <span class="sale-price">2,500 ฿</span>
        </div>
        <button class="btn-cart">หยิบใส่ตะกร้า</button>
      </div>

    </div>
  </div>

  <footer>
    <div class="footer-content">
      <div class="footer-col">
        <h4>DEBLUTE</h4>
        <p>ร้านจัดดอกไม้สไตล์มินิมอล หรูหรา ใส่ใจทุกรายละเอียดของดอกไม้ทุกช่อ</p>
      </div>
      <div class="footer-col">
        <h4>เวลาทำการ</h4>
        <p>เปิดบริการทุกวัน: 10:00 - 19:00 น.</p>
      </div>
      <div class="footer-col">
        <h4>ติดต่อเรา</h4>
        <p>Line ID: @deblute</p>
        <p>Facebook: DEBLUTE Flower</p>
        <p>Tel: 092-XXX-XXXX</p>
      </div>
    </div>
    <div class="footer-bottom">
      &copy; 2026 DEBLUTE. All rights reserved.
    </div>
  </footer>

</body>
</html>
