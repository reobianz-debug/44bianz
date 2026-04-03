<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MBG - Martabak Bang Ganteng</title>

<style>
body {
  margin:0;
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(to bottom, #f6fbff, #ffffff);
}

header {
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:15px 30px;
  background:white;
  box-shadow:0 2px 10px rgba(0,0,0,0.05);
}

.logo {
  display:flex;
  align-items:center;
  gap:10px;
}

.logo img {
  width:40px;
}

nav a {
  margin:0 10px;
  text-decoration:none;
  color:#333;
  font-weight:500;
}

.btn-wa {
  background:#25D366;
  color:white;
  padding:10px 20px;
  border-radius:25px;
  text-decoration:none;
  font-weight:bold;
}

.hero {
  display:flex;
  flex-wrap:wrap;
  align-items:center;
  padding:50px 30px;
}

.hero-text {
  flex:1;
}

.hero-text h1 {
  font-size:40px;
  color:#219ebc;
}

.hero-text p {
  max-width:500px;
  margin:15px 0;
}

.hero-img {
  flex:1;
}

.hero-img img {
  width:100%;
  border-radius:20px;
}

.section {
  padding:40px;
  text-align:center;
}

.grid {
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
  gap:20px;
  margin-top:20px;
}

.card {
  background:white;
  border-radius:15px;
  padding:10px;
  box-shadow:0 5px 15px rgba(0,0,0,0.05);
  transition:0.3s;
}

.card:hover {
  transform:translateY(-5px);
}

.card img {
  width:100%;
  border-radius:10px;
}

footer {
  text-align:center;
  padding:20px;
  background:#8ecae6;
  color:white;
}
</style>
</head>

<body>

<header>
  <div class="logo">
    <!-- LOGO ANDA -->
    <img src="logo.png">
    <b>MBG</b>
  </div>

  <nav>
    <a href="#">Home</a>
    <a href="#">Menu</a>
    <a href="#">About</a>
  </nav>

  <!-- GANTI NOMOR -->
  <a href="https://wa.me/6281234567890" class="btn-wa">
    WhatsApp
  </a>
</header>

<section class="hero">

  <div class="hero-text">
    <h1>Martabak Premium Rasa Sultan 👑</h1>
    <p>
      Martabak Bang Ganteng hadir dengan topping melimpah,
      rasa mewah, dan kualitas terbaik.
    </p>

    <a href="https://wa.me/6281234567890" class="btn-wa">
      Pesan Sekarang
    </a>
  </div>

  <div class="hero-img">
    <img src="martabak-hero.jpg">
  </div>

</section>

<section class="section">
  <h2>🔥 Varian Favorit</h2>

  <div class="grid">

    <div class="card">
      <img src="1.jpg"><h4>Coklat Keju</h4>
    </div>

    <div class="card">
      <img src="2.jpg"><h4>Kacang Susu</h4>
    </div>

    <div class="card">
      <img src="3.jpg"><h4>Nutella Keju</h4>
    </div>

    <div class="card">
      <img src="4.jpg"><h4>Oreo Cream</h4>
    </div>

    <div class="card">
      <img src="5.jpg"><h4>Matcha Keju</h4>
    </div>

    <div class="card">
      <img src="6.jpg"><h4>Red Velvet</h4>
    </div>

    <div class="card">
      <img src="7.jpg"><h4>Tiramisu</h4>
    </div>

    <div class="card">
      <img src="8.jpg"><h4>Keju Premium</h4>
    </div>

    <div class="card">
      <img src="9.jpg"><h4>Coklat Kacang</h4>
    </div>

    <div class="card">
      <img src="10.jpg"><h4>Special MBG Mix</h4>
    </div>

  </div>
</section>

<footer>
  © MBG - Martabak Bang Ganteng
</footer>

</body>
</html>
