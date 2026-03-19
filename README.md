# Nitaaku-sayang
Happy bday
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Untuk Nitaa ❤️</title>

  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Arial', sans-serif;
      text-align: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      color: #fff;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }

    .card {
      background: rgba(0,0,0,0.35);
      padding: 30px;
      border-radius: 20px;
      max-width: 350px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.4);
      animation: fadeIn 2s ease;
    }

    h1 {
      margin-bottom: 20px;
    }

    #text {
      font-size: 18px;
      min-height: 80px;
      margin-bottom: 20px;
      transition: 0.5s;
    }

    button {
      padding: 10px 20px;
      border: none;
      border-radius: 10px;
      background: #ff4b5c;
      color: white;
      font-size: 16px;
      cursor: pointer;
    }

    .heart {
      position: absolute;
      color: #ff4b5c;
      font-size: 20px;
      animation: floatUp 5s linear infinite;
    }

    @keyframes floatUp {
      0% { transform: translateY(100vh); opacity: 1; }
      100% { transform: translateY(-10vh); opacity: 0; }
    }

    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }
  </style>
</head>

<body>

<div class="card">
  <h1>💖 Hai Nitaa 💖</h1>
  <div id="text">Klik tombolnya ya ayang 😊</div>
  <button onclick="nextText()">Klik Aku ❤️</button>
</div>

<!-- Musik Biola Romantis -->
<audio autoplay loop>
  <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_9f5b2b6d94.mp3?filename=romantic-violin-11017.mp3" type="audio/mpeg">
</audio>

<script>
let texts = [
"Hai ayang 😊",
"Aku punya sesuatu buat kamu...",
"Hari ini hari spesial banget 🎉",
"Karena hari ini kamu lahir ke dunia...",
"Selamat ulang tahun Nitaa ❤️",
"Ayang, cayang, yayangku...",
"Terima kasih sudah hadir di hidupku",
"Kamu itu bukan cuma pacarku...",
"Tapi kamu adalah rumah buat aku 💕",
"Aku bersyukur banget punya kamu",
"Semoga semua impian kamu tercapai ✨",
"Semoga kamu selalu bahagia",
"Kalau suatu hari kamu capek...",
"Ingat ya, aku selalu ada buat kamu",
"Aku mungkin bukan yang sempurna...",
"Tapi aku akan selalu berusaha jadi yang terbaik buat kamu",
"Aku mau terus bareng kamu",
"Hari ini, besok, dan seterusnya 💖",
"Dan di ulang tahunmu ini...",
"Aku cuma punya satu harapan...",
"Aku ingin tetap jadi bagian dari hidup kamu",
"I love you, Nitaa ❤️✨"
];

let index = 0;

function nextText() {
  if (index < texts.length) {
    document.getElementById("text").innerHTML = texts[index];
    index++;
  }
}

// efek hati jatuh
setInterval(() => {
  let heart = document.createElement("div");
  heart.className = "heart";
  heart.style.left = Math.random() * 100 + "vw";
  heart.innerHTML = "❤️";
  document.body.appendChild(heart);

  setTimeout(() => {
    heart.remove();
  }, 5000);
}, 500);
</script>

</body>
</html>
