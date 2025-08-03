<!DOCTYPE html>  
<html lang="es">  
<head>  
  <meta charset="UTF-8" />  
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>  
  <title>Para Ti, Génesis</title>  
  <style>  
    body {  
      margin: 0;  
      font-family: 'Comic Sans MS', cursive;  
      background: linear-gradient(to bottom right, #ffb6c1, #ffc0cb);  
      overflow: hidden;  
      text-align: center;  
    }  
    h1 {  
      margin-top: 80px;  
      font-size: 3em;  
      color: #ff1493;  
    }  
    h2 {  
      font-size: 1.5em;  
      color: #8b008b;  
      margin-bottom: 40px;  
      padding: 0 20px;  
    }  
    .floating-text {  
      position: absolute;  
      font-size: 1.1em;  
      color: white;  
      animation: float 10s linear infinite;  
      opacity: 0.9;  
      pointer-events: none;  
    }  
    @keyframes float {  
      0% {  
        transform: translateY(100vh) rotate(0deg);  
        opacity: 0;  
      }  
      50% {  
        opacity: 1;  
      }  
      100% {  
        transform: translateY(-100vh) rotate(360deg);  
        opacity: 0;  
      }  
    }  
    .music {  
      position: fixed;  
      bottom: 20px;  
      right: 20px;  
      background: white;  
      padding: 10px 15px;  
      border-radius: 15px;  
      box-shadow: 0 0 10px rgba(0,0,0,0.2);  
    }  
  </style>  
</head>  
<body>  
  <h1>Para ti, Génesis</h1>  
  <h2>Que eres mi persona favorita. Te amo ❤️ 🥺</h2>  
  <audio autoplay loop class="music" controls>  
    <source src="https://www.bensound.com/bensound-music/bensound-love.mp3" type="audio/mpeg">  
    Tu navegador no soporta audio :(  
  </audio>  
  <script>  
    const frases = [  
      "Te amo ❤️", "Mi niña 🥰", "Mi persona favorita 💕",  
      "Abracito 🥺", "Contigo todo 💖", "Te extraño",   
      "Mi sol ☀️", "Eres todo para mí", "Siempre tú 🌙",  
      "Mi corazón", "Mi ternura 💘", "Eres única 🌸"  
    ];  
    for (let i = 0; i < 50; i++) {  
      const span = document.createElement('span');  
      span.className = 'floating-text';  
      span.textContent = frases[Math.floor(Math.random() * frases.length)];  
      span.style.left = Math.random() * 100 + 'vw';  
      span.style.top = Math.random() * 100 + 'vh';  
      span.style.animationDuration = (Math.random() * 5 + 5) + 's';  
      document.body.appendChild(span);  
    }  
  </script>  
</body>  
</html>
