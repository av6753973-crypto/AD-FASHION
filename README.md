
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AD FASHION DESIGNER</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f8f8f8;
      color: #333;
    }
    header {
      background-color: #000;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    nav {
      background-color: #444;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }
    nav a {
      color: white;
      padding: 1rem;
      text-decoration: none;
    }
    nav a:hover {
      background-color: #222;
    }
    section {
      padding: 2rem;
      text-align: center;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1rem;
    }
    .product {
      background: white;
      padding: 1rem;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .product img {
      width: 100%;
      height: 150px;
      object-fit: cover;
    }
    form {
      display: flex;
      flex-direction: column;
      max-width: 400px;
      margin: auto;
    }
    input, textarea {
      margin-bottom: 1rem;
      padding: 0.5rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    footer {
      background: #000;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    .language-toggle {
      position: fixed;
      top: 10px;
      right: 10px;
    }
  </style>
</head>
<body>
  <div class="language-toggle">
    <button onclick="setLanguage('en')">English</button>
    <button onclick="setLanguage('hi')">हिन्दी</button>
  </div>
  <header>
    <h1>AD FASHION DESIGNER</h1>
    <p id="tagline">Trendy Fashion for Everyone | हर किसी के लिए फैशनेबल कपड़े</p>
  </header>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#products">Products</a>
    <a href="#contact">Contact</a>
  </nav>
  <section id="home">
    <h2 data-en="Welcome to AD FASHION DESIGNER!" data-hi="AD FASHION DESIGNER में आपका स्वागत है!">Welcome to AD FASHION DESIGNER!</h2>
    <p data-en="Explore the latest trends in fashion." data-hi="फैशन की नई रुझानों को खोजें।">Explore the latest trends in fashion.</p>
  </section>
  <section id="about">
    <h2 data-en="About Us" data-hi="हमारे बारे में">About Us</h2>
    <p data-en="We bring stylish and affordable fashion to your doorstep." data-hi="हम आपके दरवाज़े तक स्टाइलिश और किफायती फैशन लाते हैं।">We bring stylish and affordable fashion to your doorstep.</p>
  </section>
  <section id="products">
    <h2 data-en="Our Products" data-hi="हमारे उत्पाद">Our Products</h2>
    <div class="products">
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Product 1">
        <h3 data-en="Stylish Shirt" data-hi="स्टाइलिश शर्ट">Stylish Shirt</h3>
        <p>₹499</p>
        <button>Buy Now</button>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Product 2">
        <h3 data-en="Trendy Kurti" data-hi="ट्रेंडी कुर्ती">Trendy Kurti</h3>
        <p>₹699</p>
        <button>Buy Now</button>
      </div>
    </div>
  </section>
  <section id="contact">
    <h2 data-en="Contact Us" data-hi="संपर्क करें">Contact Us</h2>
    <form>
      <input type="text" placeholder="Name / नाम" required>
      <input type="email" placeholder="Email / ईमेल" required>
      <textarea rows="4" placeholder="Your Message / आपका संदेश" required></textarea>
      <button type="submit">Send / भेजें</button>
    </form>
  </section>
  <footer>
    <p>&copy; 2025 AD FASHION DESIGNER</p>
    <p>
      <a href="#" style="color:white;">Facebook</a> |
      <a href="#" style="color:white;">Instagram</a> |
      <a href="https://wa.me/91XXXXXXXXXX" style="color:white;">WhatsApp</a>
    </p>
  </footer>  <script>
    function setLanguage(lang) {
      document.querySelectorAll('[data-en]').forEach(el => {
        el.textContent = el.getAttribute(`data-${lang}`);
      });
    }
  </script></body>
</html>
