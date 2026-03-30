<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Undangan Pernikahan Bimbi & Sasa</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Poppins:wght@300;400&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #f9f7f5;
      color: #333;
    }
    header {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://images.unsplash.com/photo-1520854221256-17451cc331bf');
      background-size: cover;
      color: white;
      flex-direction: column;
    }
    header h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3em;
      margin: 0;
    }
    header p {
      margin-top: 10px;
    }
    .btn {
      margin-top: 20px;
      padding: 10px 25px;
      border: none;
      background: #d4af37;
      color: white;
      cursor: pointer;
      border-radius: 30px;
    }
    section {
      padding: 60px 20px;
      text-align: center;
    }
    h2 {
      font-family: 'Playfair Display', serif;
      margin-bottom: 20px;
    }
    .couple {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 40px;
    }
    .card {
      background: white;
      padding: 20px;
      border-radius: 15px;
      width: 250px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px,1fr));
      gap: 10px;
    }
    .gallery img {
      width: 100%;
      border-radius: 10px;
    }
    iframe {
      width: 100%;
      height: 300px;
      border: none;
      border-radius: 10px;
    }
    footer {
      background: #222;
      color: white;
      padding: 20px;
      text-align: center;
    }
  </style>
</head>
<body>

<header>
  <h1>Bimbi & Sasa</h1>
  <p>Kepada Yth. <span id="guest">Tamu Undangan</span></p>
  <button class="btn" onclick="openInvite()">Buka Undangan</button>
</header>

<section id="opening" style="display:none;">
  <h2>Assalamu'alaikum Warahmatullahi Wabarakatuh</h2>
  <p>Dengan memohon rahmat dan ridho Allah SWT, kami bermaksud menyelenggarakan pernikahan putra-putri kami.</p>
</section>

<section>
  <h2>Pasangan Pengantin</h2>
  <div class="couple">
    <div class="card">
      <h3>Bimbi</h3>
      <p>Putra dari Bapak & Ibu</p>
    </div>
    <div class="card">
      <h3>Sasa</h3>
      <p>Putri dari Bapak & Ibu</p>
    </div>
  </div>
</section>

<section>
  <h2>Detail Acara</h2>
  <p><b>Akad Nikah:</b> Sabtu, 10 Oktober 2026</p>
  <p><b>Resepsi:</b> Sabtu, 10 Oktober 2026</p>
  <p><b>Lokasi:</b> Gedung Serbaguna</p>
</section>

<section>
  <h2>Galeri</h2>
  <div class="gallery">
    <img src="https://images.unsplash.com/photo-1519741497674-611481863552">
    <img src="https://images.unsplash.com/photo-1529634896116-cdb1f4c46a6d">
    <img src="https://images.unsplash.com/photo-1501908734255-16579c18c25f">
  </div>
</section>

<section>
  <h2>Lokasi</h2>
  <iframe src="https://www.google.com/maps?q=jakarta&output=embed"></iframe>
</section>

<section>
  <h2>Amplop Digital</h2>
  <p>Bank BCA - 1234567890 a.n Bimbi</p>
  <p>Bank Mandiri - 9876543210 a.n Sasa</p>
</section>

<footer>
  <p>Terima kasih atas doa dan restu Anda</p>
</footer>

<script>
  function openInvite() {
    document.getElementById('opening').style.display = 'block';
    window.scrollTo({ top: document.getElementById('opening').offsetTop, behavior: 'smooth' });
  }

  // Ambil nama tamu dari URL
  const params = new URLSearchParams(window.location.search);
  const name = params.get('to');
  if(name) {
    document.getElementById('guest').innerText = name;
  }
</script>

</body>
</html>
