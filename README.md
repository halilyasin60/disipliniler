<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<title>Ultra Pro Web Site</title>

<style>
body{
  margin:0;
  font-family:Arial;
  transition:0.3s;
}

.light{background:#f4f4f4;color:#000;}
.dark{background:#121212;color:#fff;}

header{
  background:linear-gradient(90deg,#3498db,#8e44ad);
  color:white;
  text-align:center;
  padding:30px;
}

/* NAV */
nav{
  position:sticky;
  top:0;
  background:#111;
  display:flex;
  justify-content:center;
}

nav a{
  color:white;
  padding:15px;
  text-decoration:none;
}

nav a:hover{background:#1abc9c;}

/* CARD */
.card{
  width:80%;
  margin:20px auto;
  padding:20px;
  border-radius:10px;
  background:white;
  box-shadow:0 3px 10px rgba(0,0,0,0.2);
  transition:0.3s;
}

.dark .card{background:#1e1e1e;}

.card:hover{
  transform:scale(1.02);
}

/* BUTTON */
button{
  padding:10px;
  border:none;
  border-radius:5px;
  background:#3498db;
  color:white;
  cursor:pointer;
}

button:hover{background:#1abc9c;}

/* FORM */
input,textarea{
  width:100%;
  padding:10px;
  margin:5px 0;
}

footer{
  text-align:center;
  padding:15px;
  background:#000;
  color:white;
}
</style>
</head>

<body class="light">

<header>
  <h1>🚀 Ultra Pro Site</h1>
  <p>HTML + CSS + JS Proje</p>
  <button onclick="mode()">🌙 Mod Değiştir</button>
</header>

<nav>
  <a href="#home">Ana</a>
  <a href="#about">Hakkımda</a>
  <a href="#projects">Projeler</a>
  <a href="#contact">İletişim</a>
</nav>

<div class="card" id="home">
  <h2>🏠 Ana Sayfa</h2>
  <p>Bu site ileri seviye web projesidir.</p>
  <p id="counter">Ziyaretçi: 0</p>
</div>

<div class="card" id="about">
  <h2>👤 Hakkımda</h2>
  <p>Adım: Halil</p>
  <p>Web geliştirme öğreniyorum.</p>
</div>

<div class="card" id="projects">
  <h2>💻 Projeler</h2>
  <ul>
    <li>Site tasarımı</li>
    <li>Mini oyun</li>
    <li>HTML projeleri</li>
  </ul>
</div>

<div class="card" id="contact">
  <h2>📧 İletişim</h2>

  <input placeholder="Adın">
  <input placeholder="E-posta">
  <textarea placeholder="Mesaj"></textarea>
  <button onclick="alert('Mesaj gönderildi!')">Gönder</button>
</div>

<footer>
  © 2026 Ultra Pro Site
</footer>

<script>
let count = 0;

function mode(){
  document.body.classList.toggle("dark");
  document.body.classList.toggle("light");
}

setInterval(()=>{
  count++;
  document.getElementById("counter").innerText = "Ziyaretçi: " + count;
},2000);
</script>

</body>
</html>
