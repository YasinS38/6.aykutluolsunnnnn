<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Aleyna & Yasin – 6. Ayımız 💖</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to bottom, #fce4ec, #f3e5f5);
      font-family: 'Segoe UI', sans-serif;
      overflow-x: hidden;
      position: relative;
    }
    .container {
      max-width: 800px;
      margin: auto;
      padding: 30px 20px;
      text-align: center;
    }
    h1 {
      color: #d63384;
      margin-bottom: 30px;
    }
    .message {
      margin-top: 20px;
      font-size: 18px;
      line-height: 1.6;
    }
    .photo-block {
      margin-bottom: 40px;
    }
    .photo-block img {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }
    .photo-block p {
      font-size: 17px;
      margin-top: 10px;
      color: #6a1b9a;
      font-style: italic;
    }
    footer {
      margin-top: 50px;
      font-size: 16px;
      color: #777;
    }

    /* Kalpler */
    .heart {
      position: fixed;
      width: 20px;
      height: 20px;
      background-color: pink;
      transform: rotate(45deg);
      animation: float 6s infinite;
      opacity: 0.8;
    }
    .heart::before,
    .heart::after {
      content: "";
      position: absolute;
      width: 20px;
      height: 20px;
      background-color: pink;
      border-radius: 50%;
    }
    .heart::before {
      top: -10px;
      left: 0;
    }
    .heart::after {
      left: -10px;
      top: 0;
    }
    @keyframes float {
      0% { transform: translateY(0) rotate(45deg); opacity: 1; }
      100% { transform: translateY(-100vh) rotate(45deg); opacity: 0; }
    }

    /* Papatyalar */
    .daisy {
      position: fixed;
      width: 30px;
      height: 30px;
      background: url('https://upload.wikimedia.org/wikipedia/commons/thumb/e/e6/Leucanthemum_vulgare_-_Köhler%E2%80%93s_Medizinal-Pflanzen-088.jpg/240px-Leucanthemum_vulgare_-_Köhler%E2%80%93s_Medizinal-Pflanzen-088.jpg') no-repeat center center / cover;
      animation: fall 10s infinite linear;
    }
    @keyframes fall {
      0% { transform: translateY(-10%); opacity: 1; }
      100% { transform: translateY(110vh); opacity: 0; }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>💖 6. Ayımız Kutlu Olsun Aleynam 💖</h1>
    <p class="message">
      Bu küçük sayfa; hem bir özür, hem bir teşekkür, hem de bir kutlama... Seni çok seviyorum. 💞
    </p>

    <div class="photo-block"><img src="foto1.jpg"><p>Gözlerine bakamıyorum çünkü o an sadece şımarıyoruz.</p></div>
    <div class="photo-block"><img src="foto2.jpg"><p>Güneş seninle yarışıyordu. Ama senin gözlerin daha çok parlıyordu...</p></div>
    <div class="photo-block"><img src="foto3.jpg"><p>Bir gün bu karelere çocuklarımızla bakacağız.</p></div>
    <div class="photo-block"><img src="foto4.jpg"><p>Küçük şeylerle mutlu olduğumuz günler... En büyük mutluluklarımız.</p></div>
    <div class="photo-block"><img src="foto5.jpg"><p>Pijamalarla bile dünyanın en güzeli sensin.</p></div>
    <div class="photo-block"><img src="foto6.jpg"><p>Dil çıkarmışsın, çocuk gibisin… Ama ben o çocuk yanına da, kadın yanına da aşığım.</p></div>
    <div class="photo-block"><img src="foto7.jpg"><p>Hayalim: Uyanınca seni görmek, uyurken seni izlemek. Her sabah ve her gece...</p></div>

    <footer>
      Aleyna & Yasin 🌙 30.12.2024 <br> Kalbim hep seninle...
    </footer>
  </div>

  <!-- Kalpler -->
  <script>
    function createHeart() {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.top = "100vh";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 6000);
    }
    setInterval(createHeart, 300);
  </script>

  <!-- Papatyalar -->
  <script>
    function createDaisy() {
      const daisy = document.createElement("div");
      daisy.className = "daisy";
      daisy.style.left = Math.random() * 100 + "vw";
      document.body.appendChild(daisy);
      setTimeout(() => daisy.remove(), 10000);
    }
    setInterval(createDaisy, 2000);
  </script>
</body>
</html>
