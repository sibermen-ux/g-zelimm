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
    display: block;
    padding: 10px;
}

.card {
    background: rgba(255, 255, 255, 0.2);
    border-radius: 20px;
    padding: 15px;
    margin: 10px auto;
    width: 95%;
    max-width: 400px;
    min-height: 100px;
    box-shadow: 0 6px 12px rgba(0,0,0,0.2);
    transition: transform 0.3s, box-shadow 0.3s;
    word-wrap: break-word;
}
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
        document.body.appendChild(emoji);
        setTimeout(() => emoji.remove(), 5000);
    }

    setInterval(createEmoji, 500);

    const poemsContainer = document.getElementById('poemsContainer');
    const samplePoems = [
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
        'Geceler senin hayalinle aydınlanır. 🌌',
        'Bir gülüşünle bahar olur içimde. 🌷',
        'Seninle susmak bile şiir gibi. 🤫',
        'Adın, kalbimin en güzel melodisi. 🎵',
        'Seninle geçen zaman, cennetten bir parça. 🕊️',
        'Bir bakışınla dünyam değişir. 🌍',
        'Seninle her şey daha anlamlı. ✨',
        'Kalbim seni görünce şiir yazmaya başlar. 🖋️',
        'Seninle yürüdüğüm yollar, yıldızlarla döşeli. 🚶‍♀️🌠',
        'Bir kelimenle içim huzur bulur. 🧘‍♂️',
        'Senin adın, dualarımın en güzel cümlesi. 🙌',
        'Seninle her sabah, umutla başlar. 🌅',
        'Gözlerin, kalbimin pusulası. 🧭',
        'Seninle geçen her saniye, ömre bedel. ⏱️',
        'Bir dokunuşun, bin şiire ilham. ✍️',
        'Kalbim seni görünce dans eder. 💃',
        'Seninle her an, bir mucize gibi. 🌈',
        'Bir gülüşünle karanlık aydınlanır. 💡',
        'Seninle konuşmak, kalbimle sohbet etmek gibi. 🗣️',
        'Senin adın, içimde yankılanan sevda. 🔔',
        'Kalbim seninle tamamlanır. 🧩',
        'Seninle her gün, bir şiir gibi başlar. 📜',
        'Gözlerin, içimdeki huzurun aynası. 🪞',
        'Seninle olmak, yıldızlara dokunmak gibi. 🌠',
        'Bir kelimen, bin tebessüm. 😊',
        'Seninle geçen zaman, kalbimin en değerli hazinesi. 💎',
        'Seninle her an, bir şiirin içinde yaşamak gibi. 🖼️',
        'Kalbim seninle her gün yeniden doğar. 🌞',
        // Yeni eklenen 50 özgün şiir
        'Senin adınla başlar içimdeki her şiir. 📝',
        'Bir tebessümün, kalbimde bahar yaratır. 🌼',
        'Seninle geçen her dakika, sonsuzluk gibi. ⏳',
        'Kalbim seninle konuşur, sessizce. 🔇',
        'Senin varlığın, içimdeki en güzel huzur. 🕊️',
        'Bir bakışın, tüm kelimelerden daha anlamlı. 👀',
        'Seninle olmak, zamanın ötesinde yaşamak gibi. 🪐',
        'Kalbim seninle her gün yeniden yazılır. 📖',
        'Senin gülüşün, içimdeki en güzel şarkı. 🎤',
        'Bir dokunuşun, tüm dünyayı susturur. 🌍',
        'Seninle her an, bir tablo gibi eşsiz. 🖼️',
        'Kalbim seninle şiir gibi akar. 🪶',
        'Senin adın, içimde yankılanan sevgi. 🔊',
        'Bir gülüşünle tüm acılar unutur kendini. 💭',
        'Seninle olmak, gökyüzüne dokunmak gibi. ☁️',
        'Kalbim seninle her gece dua eder. 🙏',
        'Seninle susmak bile anlam taşır. 🧘',
        'Bir kelimen, içimde yıldızlar yakar. ✨',
        'Seninle geçen zaman, kalbimin en güzel anısı. 🎞️',
        'Kalbim seninle her gün şiir yazar. 🖊️',
        'Seninle olmak, rüzgarla dans etmek gibi. 🍃',
        'Bir bakışın, içimdeki tüm sessizliği konuşturur. 🎙️',
        'Seninle her şey daha renkli. 🎨',
        'Kalbim seninle her gece yıldızlara ulaşır. 🌌',
        'Senin adın, içimdeki en güzel melodi. 🎼',
        'Bir gülüşün, tüm karanlığı aydınlatır. 🔆',
        'Seninle olmak, kalbimin en doğal hali. 🌿',
        'Kalbim seninle her gün yeniden çiçek açar. 🌻',
        'Seninle susmak bile huzur verir. 🧘‍♂️',
        'Bir kelimen, içimdeki tüm duvarları yıkar. 🧱',
        'Seninle her an, bir sevda yolculuğu. 🚂',
        'Kalbim seninle her gün yeniden başlar. 🔄',
        'Seninle olmak, gökyüzüne şiir yazmak gibi. ✍️',
        'Bir bakışın, içimdeki tüm renkleri uyandırır. 🌈',
        'Seninle her şey daha yumuşak, daha nazik. 🧸',
        'Kalbim seninle her gün bir masal anlatır. 📚',
        'Seninle olmak, içimdeki tüm yıldızları parlatır. 💫',
        'Bir kelimen, içimdeki tüm şarkıları söyletir. 🎶',
        'Seninle her an, bir sevda resmi. 🖌️',
        'Kalbim seninle her gün bir dua gibi. 🕯️',
        'Seninle olmak, içimdeki tüm sessizliği sevgiyle doldurur. 🤍',
        'Bir gülüşün, içimdeki tüm kışları eritir. ❄️',
        'Seninle her an, bir sevda mevsimi. 🍂',
        'Kalbim seninle her gün bir şiir mırıldanır. 🎤',
        'Seninle olmak, içimdeki tüm boşlukları sevgiyle doldurur. 🧡',
        'Bir kelimen, içimdeki tüm duyguları uyandırır. 🫀',
        'Seninle her an, bir sevda dansı. 💃🕺',
        'Kalbim seninle her gün bir yıldız gibi parlar. ⭐'
    ];

    for (let i = 0; i < samplePoems.length; i++) {
        const card = document.createElement('div');
        card.className = 'card';
        card.innerHTML = `<p><span class='heart'>💌</span>${samplePoems[i]}</p>`;
        poemsContainer.appendChild(card);
    }
</script>

</body>
</html>
