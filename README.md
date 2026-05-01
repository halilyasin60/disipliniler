#disiplinler
<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<title>Benim Kişisel Web Sitem</title>

<style>
body {margin:0;font-family:Arial;background:#f4f4f4;}

/* ÜST BANNER */
header{
  background:linear-gradient(90deg,#2c3e50,#3498db);
  color:white;
  text-align:center;
  padding:30px;
}

/* MENÜ */
nav{
  display:flex;
  justify-content:center;
  background:#1f2d3a;
}
nav a{
  color:white;
  padding:15px 20px;
  text-decoration:none;
}
nav a:hover{
  background:#1abc9c;
}

/* KUTULAR */
.container{
  width:90%;
  margin:auto;
}

.card{
  background:white;
  padding:20px;
  margin:20px 0;
  border-radius:10px;
  box-shadow:0 2px 8px rgba(0,0,0,0.1);
}

/* BUTON */
button{
  padding:10px 15px;
  border:none;
  background:#3498db;
  color:white;
  border-radius:5px;
  cursor:pointer;
}
button:hover{
  background:#1abc9c;
}

/* FOOTER */
footer{
  text-align:center;
  background:#2c3e50;
  color:white;
  padding:15px;
  margin-top:20px;
}
</style>

</head>

<body>

<header>
  <h1>Benim Web Sitem</h1>
  <p>HTML ile yapılmış kişisel proje</p>
</header>

<nav>
  <a href="#home">Ana Sayfa</a>
  <a href="#about">Hakkımda</a>
  <a href="#projects">Projeler</a>
  <a href="#contact">İletişim</a>
</nav>

<div class="container">

<!-- ANA SAYFA -->
<div class="card" id="home">
  <h2>🏠 Ana Sayfa</h2>
  <p>Bu site benim okul ödevim için hazırlanmıştır. GitHub Pages ile yayınlanacaktır.</p>
  <button onclick="alert('Hoş geldin 😎')">Tıkla</button>
</div>

<!-- HAKKIMDA -->
<div class="card" id="about">
  <h2>👤 Hakkımda</h2>
  <p>Adım: Halil</p>
  <p>Web sitesi yapmayı öğreniyorum.</p>
  <p>HTML, CSS kullanarak bu projeyi oluşturdum.</p>
</div>

<!-- PROJELER -->
<div class="card" id="projects">
  <h2>💻 Projeler</h2>
  <ul>
    <li>Basit web sitesi</li>
    <li>Oyun projesi (köstebek oyunu)</li>
    <li>HTML öğrenme sayfası</li>
  </ul>
</div>

<!-- İLETİŞİM -->
<div class="card" id="contact">
  <h2>📧 İletişim</h2>
  <p>E-posta: example@gmail.com</p>
  <p>Telefon: 05xx xxx xx xx</p>
</div>

</div>

<footer>
  © 2026 Benim Web Sitem | Tüm hakları saklıdır
</footer>

</body>
</html>
