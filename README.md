# Merhaba, Ben Kürşad! 👋

<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>SmartWatch X200</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f4f4f4;
      scroll-behavior: smooth;
    }

    header {
      background: linear-gradient(135deg, #0d47a1, #1976d2);
      color: white;
      text-align: center;
      padding: 30px 20px;
    }
    header img {
      width: 150px;
      height: auto;
      margin: 20px 0;
      transition: transform 0.3s;
    }
    header img:hover {
      transform: scale(1.05);
    }

    .buy-btn {
      background: #ff9800;
      color: white;
      padding: 12px 25px;
      border: none;
      font-size: 16px;
      cursor: pointer;
      border-radius: 5px;
      transition: background 0.3s, transform 0.2s;
    }
    .buy-btn:hover {
      background: #e68900;
      transform: scale(1.05);
    }

    .features {
      display: flex;
      justify-content: space-around;
      flex-wrap: wrap;
      background: white;
      padding: 40px 20px;
    }
    .feature-card {
      width: 200px;
      text-align: center;
      margin: 15px;
      transition: transform 0.3s;
      position: relative;
      cursor: pointer;
    }
    .feature-card:hover {
      transform: scale(1.05);
    }
    .feature-card i {
      font-size: 40px;
      color: #0d47a1;
      margin-bottom: 10px;
    }
    .tooltip {
      visibility: hidden;
      width: 180px;
      background-color: #0d47a1;
      color: #fff;
      text-align: center;
      border-radius: 6px;
      padding: 8px;
      position: absolute;
      bottom: 110%;
      left: 50%;
      transform: translateX(-50%);
      opacity: 0;
      transition: opacity 0.3s ease, transform 0.3s ease;
      z-index: 1;
      font-size: 13px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.2);
    }
    .feature-card:hover .tooltip {
      visibility: visible;
      opacity: 1;
      transform: translateX(-50%) translateY(-5px);
    }

    .reviews {
      background: #e3f2fd;
      padding: 40px 20px;
      text-align: center;
      position: relative;
    }
    .review-slider {
      display: flex;
      overflow: hidden;
      max-width: 600px;
      margin: auto;
      justify-content: center;
    }
    .review {
      background: white;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      margin: 0 10px;
      padding: 20px;
      width: 100%;
      max-width: 400px;
      flex-shrink: 0;
      transition: transform 0.3s;
      display: none;
    }
    .review img {
      border-radius: 50%;
      width: 60px;
      height: 60px;
    }
    .review h4 {
      margin: 10px 0 5px;
    }
    .slider-buttons {
      margin-top: 20px;
    }
    .slider-buttons button {
      background: #0d47a1;
      color: white;
      border: none;
      padding: 10px;
      border-radius: 50%;
      margin: 0 5px;
      cursor: pointer;
      transition: background 0.3s;
    }
    .slider-buttons button:hover {
      background: #1565c0;
    }

    .price-section {
      background: #fff;
      padding: 30px 20px;
      text-align: center;
    }
    .price {
      font-size: 28px;
      color: #0d47a1;
      margin: 10px 0;
    }
    .shipping {
      color: green;
      font-weight: bold;
    }
    .contact {
      background: #f1f1f1;
      padding: 30px 20px;
    }
    .contact form {
      max-width: 400px;
      margin: auto;
      display: flex;
      flex-direction: column;
    }
    .contact input, .contact textarea {
      margin: 10px 0;
      padding: 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    .contact button {
      background: #0d47a1;
      color: white;
      padding: 10px;
      border: none;
      border-radius: 5px;
      transition: background 0.3s;
    }
    .contact button:hover {
      background: #1565c0;
    }
    footer {
      background: #0d47a1;
      color: white;
      text-align: center;
      padding: 20px;
    }
    footer a {
      color: white;
      margin: 0 10px;
      text-decoration: none;
    }
  </style>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" rel="stylesheet">
</head>
<body>

<header>
  <h1>SmartWatch X200</h1>
  <p>Hayatınızı Kolaylaştıran Akıllı Saat</p>
  <img src="https://i0.wp.com/cyberdeals.lk/wp-content/uploads/2024/09/X200-Pro-Series-9-Smart-Watch.jpg?fit=600%2C600&ssl=1" alt="SmartWatch X200 Pro">
  <br>
  <button class="buy-btn">Şimdi Satın Al</button>
</header>

<section class="features">
  <div class="feature-card">
    <i class="fas fa-heartbeat"></i>
    <p>Kalp Atış Takibi</p>
    <span class="tooltip">Günlük kalp ritminizi ölçerek sağlık takibi sağlar.</span>
  </div>
  <div class="feature-card">
    <i class="fas fa-wifi"></i>
    <p>Wi-Fi & Bluetooth</p>
    <span class="tooltip">Kablosuz bağlantı ile bildirimleri ve çağrıları gösterir.</span>
  </div>
  <div class="feature-card">
    <i class="fas fa-battery-full"></i>
    <p>7 Gün Pil</p>
    <span class="tooltip">Tam şarjla 7 gün boyunca kullanım sağlar.</span>
  </div>
  <div class="feature-card">
    <i class="fas fa-cloud-sun"></i>
    <p>Hava Durumu</p>
    <span class="tooltip">Anlık hava durumu bilgilerini gösterir.</span>
  </div>
</section>

<!-- Kullanıcı Yorumları - SLIDER -->
<section class="reviews">
  <h2>Kullanıcı Yorumları</h2>
  <div class="review-slider" id="review-slider">
    <div class="review">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTL5tuMLT69cmAIfPBf9N9h3UAOg5BVcXly-w&s" alt="Ayşe">
      <h4>Ayşe Yılmaz</h4>
      <p>Harika bir ürün! Spor yaparken çok yardımcı oluyor.</p>
    </div>
    <div class="review">
      <img src="https://images.pexels.com/photos/2379004/pexels-photo-2379004.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" alt="Mehmet">
      <h4>Mehmet Demir</h4>
      <p>Şık ve kullanışlı. Bildirimleri takip etmek çok kolay.</p>
    </div>
    <div class="review">
      <img src="https://img3.stockfresh.com/files/l/lithian/m/81/6255119_stock-photo-young-woman-taking-photos.jpg" alt="Selin">
      <h4>Selin Koç</h4>
      <p>Pil ömrü uzun, tasarımı çok zarif. Tavsiye ederim.</p>
    </div>
  </div>
  <div class="slider-buttons">
    <button onclick="slide(-1)">‹</button>
    <button onclick="slide(1)">›</button>
  </div>
</section>

<section class="price-section">
  <p class="price">₺1.499</p>
  <p class="shipping">Ücretsiz Kargo</p>
  <button class="buy-btn">Satın Al</button>
</section>

<section class="contact">
  <h2>İletişim</h2>
  <form id="contactForm">
    <input type="text" placeholder="Ad Soyad" required>
    <input type="email" placeholder="E-posta" required>
    <textarea rows="4" placeholder="Mesajınız..." required></textarea>
    <button type="submit">Gönder</button>
  </form>
</section>

<footer>
  <p>&copy; 2025 SmartWatch X200</p>
  <a href="#">Instagram</a> |
  <a href="#">Twitter</a> |
  <a href="#">Facebook</a>
</footer>

<script>
  let currentIndex = 0;
  const reviews = document.querySelectorAll('.review');

  function showReview(index) {
    reviews.forEach((review, i) => {
      review.style.display = (i === index) ? 'block' : 'none';
    });
  }

  function slide(direction) {
    currentIndex += direction;
    if (currentIndex < 0) currentIndex = reviews.length - 1;
    if (currentIndex >= reviews.length) currentIndex = 0;
    showReview(currentIndex);
  }

  showReview(currentIndex);
</script>

</body>
</html>

