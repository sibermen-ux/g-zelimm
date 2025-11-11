karıcımmmmmmmmmmmmm
<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>KOCANDAN SANA UFAK BİR HEDİYE 💖🌸💋🫶</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #ffb3c6, #d1c0ff, #a0e9ff);
      overflow-x: hidden;
      color: #fff;
      position: relative;
    }

    h1 {
      text-align: center;
      padding: 20px;
      font-size: 2.2em;
      text-shadow: 2px 2px 5px #000;
    }

    .container {
      padding: 10px;
    }

    .card {
      background: rgba(255, 255, 255, 0.2);
      border-radius: 20px;
      padding: 15px;
      margin: 10px auto;
      width: 95%;
      max-width: 400px;
      box-shadow: 0 6px 12px rgba(0,0,0,0.2);
      transition: transform 0.3s, box-shadow 0.3s;
      word-wrap: break-word;
    }

    .card:hover {
      transform: scale(1.03);
      box-shadow: 0 10px 18px rgba(0,0,0,0.3);
    }

    .heart {
      color: #ff4d6d;
      font-size: 1.2em;
      margin-right: 5px;
    }

    .emoji {
      position: fixed;
      font-size: 1.5em;
      pointer-events: none;
      z-index: 1000;
      animation: floatPulse 3s infinite;
    }

    @keyframes floatPulse {
      0%, 100% { transform: scale(1) translateY(0); opacity: 1; }
      50% { transform: scale(1.5) translateY(-20px); opacity: 0.8; }
    }

    @media (max-width: 600px) {
      h1 { font-size: 1.8em; }
      .card { width: 95%; padding: 10px; }
    }
  </style>
</head>
<body>

<h1>💖 Aşkın Uçuşan Şiirleri 🌸💋🫶</h1>
<div class="container" id="poemsContainer"></div>

<script>
  const emojis = ['❤️','💋','🌸','🌹','💌','🫶'];

  function createEmoji() {
    const emoji = document.createElement('div');
    emoji.className = 'emoji';
    emoji.textContent = emojis[Math.floor(Math.random() * emojis.length)];
    emoji.style.left = Math.random() * window.innerWidth + 'px';
    emoji.style.top = Math.random() * window.innerHeight + 'px';
    document.body.appendChild(emoji);
    setTimeout(() => emoji.remove(), 5000);
  }

  setInterval(createEmoji, 500);

  const poems = [
    'Seninle her an bir şiir... 🌸💋🫶',
    'Kalbim sadece senin melodinle çarpıyor. 🌹🫶',
    'Gözlerin bir yıldız, ruhum onun ışığında. 🌟🫶',
    'Sesin bir melodi, kalbim onun ritminde dans eder. 🎶',
    'Gülüşün bahar gibi, içimde çiçekler açtırır. 🌸',
    'Varlığın bir şiir, her dizede sana aşık olurum. 📖',
    'Kalbinin sesi, en güzel duamdır gecelere. 🌙',
    'Bakışların bir kıvılcım, içimde sonsuz bir yangın. 🔥',
    'Adını her nefeste sevda gibi içime çekerim. 💨',
    'Seninle zaman durur, kalbim sadece seni sayar. ⏳',
    'Hayalin bir masal, her gece onunla uyurum. 💤',
    'Dokunuşun bir dua, ruhum onunla huzur bulur. 🙏',
    'Seninle her an, sonsuzluğun tadı gibi. ♾️',
    'Kalbim senin adını ezberlemiş, her atışta seni söyler. ❤️',
    'Geceler senin hayalinle aydınlanır. 🌌'
  ];

  const container = document.getElementById('poemsContainer');
  poems.forEach(text => {
    const card = document.createElement('div');
    card.className = 'card';
    card.innerHTML = `<p><span class="heart">💌</span>${text}</p>`;
    container.appendChild(card);
  });
</script>

</body>
</html>
