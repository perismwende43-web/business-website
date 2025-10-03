<!Atatech office solutions>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>atatech office Solutions</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    body { font-family: 'Poppins', sans-serif; margin: 0; padding: 0; background: #f4f6f9; color: #333; }
    header { background: #004080; color: #fff; padding: 15px 40px; display: flex; justify-content: space-between; align-items: center; box-shadow: 0 3px 8px rgba(0,0,0,0.2); }
    header h1 { margin: 0; font-size: 22px; font-weight: 700; }
    nav a { color: #fff; margin: 0 12px; text-decoration: none; font-weight: 500; transition: color 0.3s; }
    nav a:hover { color: #f0c040; }
    .hero { background: linear-gradient(rgba(0,64,128,0.7), rgba(0,64,128,0.7)), url('https://via.placeholder.com/1500x500') no-repeat center/cover; color: #fff; padding: 120px 20px; text-align: center; }
    .hero h2 { font-size: 42px; margin-bottom: 15px; font-weight: 700; animation: fadeInDown 1s ease-in-out; }
    .hero p { font-size: 18px; margin-bottom: 25px; animation: fadeInUp 1.2s ease-in-out; }
    .hero a.button { display: inline-block; padding: 14px 28px; margin: 8px; border-radius: 30px; background: #f0c040; color: #004080; font-size: 16px; font-weight: 600; text-decoration: none; transition: 0.3s; }
    .hero a.button:hover { background: #ffdb70; }
    .section { padding: 70px 20px; text-align: center; }
    .section h2 { font-size: 32px; margin-bottom: 20px; font-weight: 700; color: #004080; }
    .filters { margin: 20px auto; text-align: center; }
    .filters input, .filters select { padding: 10px; margin: 5px; border-radius: 8px; border: 1px solid #ccc; font-size: 14px; }
    .products { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 25px; margin-top: 20px; }
    .product { border: none; padding: 20px; border-radius: 15px; background: #fff; box-shadow: 0 4px 12px rgba(0,0,0,0.1); transition: transform 0.3s; }
    .product:hover { transform: translateY(-8px); }
    .product img { max-width: 100%; height: 140px; object-fit: contain; margin-bottom: 15px; }
    .product h3 { font-size: 18px; font-weight: 600; color: #333; margin: 5px 0; }
    .product p { margin: 5px 0; font-size: 15px; color: #004080; font-weight: 600; }
    .order-btn { display: inline-block; margin-top: 8px; padding: 8px 16px; border-radius: 20px; background: #25D366; color: #fff; font-size: 14px; text-decoration: none; font-weight: 600; transition: 0.3s; }
    .order-btn:hover { background: #1da851; }
    .cta { background: #004080; color: #fff; padding: 60px 20px; text-align: center; }
    .cta h2 { font-size: 30px; margin-bottom: 15px; font-weight: 700; }
    .cta p { margin-bottom: 20px; font-size: 18px; }
    .cta a { display: inline-block; padding: 14px 28px; margin: 8px; border-radius: 30px; background: #f0c040; color: #004080; font-size: 16px; font-weight: 600; text-decoration: none; transition: 0.3s; }
    .cta a:hover { background: #ffdb70; }
    footer { background: #222; color: #bbb; padding: 30px; text-align: center; font-size: 14px; }
    footer a { color: #f0c040; text-decoration: none; }
    .whatsapp-float { position: fixed; width: 55px; height: 55px; bottom: 20px; right: 20px; background: #25D366; color: #fff; border-radius: 50px; text-align: center; font-size: 28px; box-shadow: 2px 2px 8px rgba(0,0,0,0.3); z-index: 100; }
    .whatsapp-float i { margin-top: 13px; }
  </style>
  <script src="https://kit.fontawesome.com/yourcode.js" crossorigin="anonymous"></script>
</head>
<body>

<header>
  <h1>Printing & IT Solutions</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#about">About Us</a>
    <a href="#products">Products</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero">
  <h2>Reliable Printers, Toners & IT Solutions You Can Trust</h2>
  <p>Supplying original HP toners, printers, copiers, spare parts, refurbished machines, and computers.</p>
  <a href="tel:+254707045282" class="button">📞 Call Now</a>
  <a href="https://wa.me/254707045282" target="_blank" class="button">💬 WhatsApp Us</a>
</section>

<section class="section" id="products">
  <h2>Our Products</h2>
  <div class="filters">
    <input type="text" id="search" placeholder="Search products...">
    <select id="categoryFilter">
      <option value="all">All Categories</option>
      <option value="printers">Printers & Copiers</option>
      <option value="toners">HP Toners</option>
      <option value="parts">Spare Parts</option>
      <option value="refurbished">Refurbished</option>
      <option value="computers">Computers</option>
    </select>
  </div>
  <div class="products" id="productList"></div>
</section>

<section class="cta">
  <h2>Need Genuine HP Toner Today?</h2>
  <p>Call us now or chat with us on WhatsApp!</p>
  <a href="tel:+254707045282">📞 Call Now</a>
  <a href="https://wa.me/254707045282" target="_blank">💬 WhatsApp Us</a>
</section>

<footer>
  <p>&copy; 2025 atatech office Solutions| All Rights Reserved</p>
  <p>Made  in Kenya | <a href="#">Privacy Policy</a></p>
</footer>

<!-- Floating WhatsApp Button -->
<a href="https://wa.me/254707045282" class="whatsapp-float" target="_blank">
  <i class="fab fa-whatsapp"></i>
</a>

<script>
  // Load products from external JSON file
  async function loadProducts() {
    const response = await fetch('products.json');
    const products = await response.json();

    const productList = document.getElementById('productList');
    const searchInput = document.getElementById('search');
    const categoryFilter = document.getElementById('categoryFilter');

    function renderProducts() {
      const searchValue = searchInput.value.toLowerCase();
      const selectedCategory = categoryFilter.value;
      productList.innerHTML = '';

      products.filter(p => {
        const matchesSearch = p.name.toLowerCase().includes(searchValue);
        const matchesCategory = selectedCategory === 'all' || p.category === selectedCategory;
        return matchesSearch && matchesCategory;
      }).forEach(p => {
        const productDiv = document.createElement('div');
        productDiv.className = 'product';
        productDiv.innerHTML = `
          <img src="${p.image}" alt="${Kyocera TASKalfa 2553ci}">
          <h3>${}Kyocera TASKalfa 2553ci </h3>
          <p>KES $KSh 120,000 Original price was: KSh 120,000.KSh 85,000{}</p>
          <a class="order-btn" target="_blank" href="https://wa.me/254707045282?text=Hello, I want to order: ${Kyocera TASKalfa 2553ci} - KES $KSh 120,000 Original price was: KSh 120,000.KSh 85,000{}">Order on WhatsApp</a>
        `;
        productList.appendChild(productDiv);
      });
    }

    searchInput.addEventListener('input', renderProducts);
    categoryFilter.addEventListener('change', renderProducts);

    renderProducts();
  }

  loadProducts()


</body>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Atatech Office Solutions</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; }
    header { background: #1e3a8a; color: #fff; padding: 20px; text-align: center; }
    nav { background: #2563eb; padding: 10px; text-align: center; }
    nav a { color: white; margin: 0 10px; text-decoration: none; font-weight: bold; }
    nav a:hover { text-decoration: underline; }
    section { padding: 40px; }
    h2 { color: #1e3a8a; }
    .product-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; }
    .product-card { border: 1px solid #ddd; padding: 15px; text-align: center; border-radius: 8px; }
    .product-card img { max-width: 100%; height: auto; border-radius: 5px; }
    footer { background: #1e3a8a; color: white; text-align: center; padding: 20px; margin-top: 40px; }
  </style>
</head>
<body>
  <header>
    <h1>Atatech Office Solutions</h1>
    <p>Printers | Toners | Copiers | Spare Parts | Refurbished | Computers</p>
  </header>

  <nav>
    <a href="#printers">Printers</a>
    <a href="#toners">Toners</a>
    <a href="#copiers">Copiers</a>
    <a href="#spareparts">Spare Parts</a>
    <a href="#refurbished">Refurbished</a>
    <a href="#computers">Computers</a>
    <a href="#others">Others</a>
  </nav>

  <section id="printers">
    <h2>Printers</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="images/printer1.jpg" alt="Printer">
        <h3>HP LaserJet Pro</h3>
        <p>Reliable and fast printer for office use.</p>
      </div>
    </div>
  </section>

  <section id="toners">
    <h2>HP Original Toners & Cartridges</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="images/toner1.jpg" alt="Toner">
        <h3>HP 83A Black</h3>
        <p>Genuine HP toner for LaserJet printers.</p>
      </div>
    </div>
  </section>

  <section id="copiers">
    <h2>Copiers</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="images/copier1.jpg" alt="Copier">
        <h3>Canon ImageRunner</h3>
        <p>High-speed copier with duplex printing.</p>
      </div>
    </div>
  </section>

  <section id="spareparts">
    <h2>Spare Parts</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="images/sparepart1.jpg" alt="Spare Part">
        <h3>Printer Drum</h3>
        <p>Compatible replacement drum for HP printers.</p>
      </div>
    </div>
  </section>

  <section id="refurbished">
    <h2>Refurbished Products</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="images/refurb1.jpg" alt="Refurbished">
        <h3>Refurbished Laptop</h3>
        <p>Affordable and reliable refurbished laptops.</p>
      </div>
    </div>
  </section>

  <section id="computers">
    <h2>Computers</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="images/computer1.jpg" alt="Computer">
        <h3>HP ProBook</h3>
        <p>Business laptop with powerful performance.</p>
      </div>
    </div>
  </section>

  <section id="others">
    <h2>Other Products</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="images/other1.jpg" alt="Other Product">
        <h3>Networking Cables</h3>
        <p>High-quality LAN cables and accessories.</p>
      </div>
    </div>
  </section>

  <footer>
    <p>📍 Nairobi CBD, Tom Mboya Street, Oshwal House</p>
    <p>📞 0707045282 | ✉️ atatech@gmail.com</p>
  </footer>
</body>
</html>

