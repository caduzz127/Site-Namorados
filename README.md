<!DOCTYPE html>
<html lang="pt-br">

<head>
  <meta charset="UTF-8">
  <title>Página Fofa com Música</title>
  <style>
    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background: #fff0f5;
      overflow-x: hidden;
    }

    .emoji {
      position: fixed;
      top: -50px;
      font-size: 24px;
      animation: fall linear infinite;
      z-index: 0;
      opacity: 0.7;
    }

    @keyframes fall {
      0% {
        transform: translateY(-50px) rotate(0deg);
        opacity: 1;
      }

      100% {
        transform: translateY(110vh) rotate(360deg);
        opacity: 0;
      }
    }

    .container {
      position: relative;
      text-align: center;
      padding-top: 60px;
      z-index: 1;
    }

    iframe {
      border-radius: 12px;
      width: 80%;
      height: 152px;
      border: none;
    }

    img {
      margin-top: 20px;
      max-width: 80%;
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
    }

    .texto-fofo {
      margin: 30px auto;
      font-size: 22px;
      color: #d63384;
      max-width: 700px;
      padding: 20px;
      background: #fff;
      border-radius: 16px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    img.imagem-fofa {
      display: block;
      margin: 20px auto;
      width: 600px;
      max-width: 100%;
      /* Garante que em telas pequenas ela não estoure */
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
    }
  </style>
</head>

<body>



  <div class="container">


    <!-- Música do Spotify -->
    <iframe style="border-radius:12px"
      src="https://open.spotify.com/embed/track/5KvRObAybDCjaZC58Vcp4U?utm_source=generator"
      allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy">
    </iframe>

    <img src="images.jpeg" alt="Imagem fofa" class="imagem-fofa">

    <!-- Texto bonitinho -->
    <div class="texto-fofo">
      Você é a razão do meu sorriso todos os dias! 🌸<br>
      Que a sua vida seja sempre cheia de amor, paz e muitos corações! 💖💫✨
    </div>
  </div>

</body>

<!-- Emojis de coração caindo -->
<script>
  const emojiCount = 40;
  for (let i = 0; i < emojiCount; i++) {
    const emoji = document.createElement("div");
    emoji.className = "emoji";
    emoji.style.left = Math.random() * 100 + "vw";
    emoji.style.animationDuration = 4 + Math.random() * 6 + "s";
    emoji.style.fontSize = 16 + Math.random() * 24 + "px";
    emoji.innerText = "❤️";
    document.body.appendChild(emoji);
  }
</script>

</html>
