# ananya-surprise
<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ananya ji ke liye 💖</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom right, #fff0f5, #ffe4e1);
      color: #333;
      text-align: center;
      overflow-x: hidden;
    }
    h1 {
      font-size: 32px;
      color: #d63384;
      margin-top: 30px;
      animation: fadeInDown 1.5s ease-out;
    }
    p {
      font-size: 18px;
      margin: 15px 0;
      padding: 0 10px;
      animation: fadeIn 2s ease-in-out;
    }
    img {
      width: 85%;
      max-width: 320px;
      border-radius: 15px;
      margin: 20px 0;
      box-shadow: 0 6px 16px rgba(0,0,0,0.2);
      animation: popUp 1s ease;
    }
    .heart {
      position: fixed;
      width: 20px;
      height: 20px;
      background: pink;
      transform: rotate(45deg);
      animation: float 6s infinite ease-in-out;
      opacity: 0.7;
      z-index: -1;
    }
    .heart::before,
    .heart::after {
      content: "";
      position: absolute;
      width: 20px;
      height: 20px;
      background: pink;
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
    @keyframes fadeInDown {
      from { opacity: 0; transform: translateY(-30px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    @keyframes popUp {
      from { opacity: 0; transform: scale(0.95); }
      to { opacity: 1; transform: scale(1); }
    }
    @keyframes float {
      0% { transform: translateY(0) rotate(45deg); }
      100% { transform: translateY(-100vh) rotate(45deg); }
    }
    audio {
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <h1>Ananya ji ke liye ek chhota sa surprise 💌</h1>

  <img src="ananya1.jpg" alt="Ananya Photo 1">
  <p>Chaand toh sabne dekha hai...<br>Par aapke aage toh chaand bhi feeka pad jata hai</p>

  <img src="ananya2.jpg" alt="Ananya Photo 2">
  <p>Aapki muskaan wo jaadu hai jo seedha dil ko chhoo jata hai</p>

  <img src="ananya3.jpg" alt="Ananya Photo 3">
  <p>Kabhi socha nahi tha AI se likhwaunga...<br>Par feelings toh dil se hi nikli hain</p>

  <img src="ananya4.jpg" alt="Ananya Photo 4">
  <p>Aapko dekhkar lagta hai...<br>Khuda ne fursat se banaya hoga aapko</p>

  <p><em>Ek ladka jo sirf aapki ek muskurahat ke liye kuch bhi kar sakta hai...</em></p>

  <audio controls autoplay loop>
    <source src="romantic-music.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <!-- Floating Hearts -->
  <script>
    for(let i = 0; i < 30; i++) {
      let heart = document.createElement('div');
      heart.classList.add('heart');
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (5 + Math.random() * 5) + 's';
      document.body.appendChild(heart);
    }
  </script>
</body>
</html>
