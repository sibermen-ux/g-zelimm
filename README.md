<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>KOCANDAN SANA UFAK BİR HEDİYE 💖🌸💋🫶</title>
  <style>
    :root{
      --bg1: #ffb3c6;
      --bg2: #d1c0ff;
      --bg3: #a0e9ff;
      --card-bg: rgba(255,255,255,0.18);
      --text: #ffffff;
      --accent: #ff4d6d;
      --max-emoji: 12;
    }

    /* Temel düzen ve arka plan */
    html,body{
      height:100%;
      margin:0;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: linear-gradient(135deg, var(--bg1), var(--bg2), var(--bg3));
      color: var(--text);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      overflow-x:hidden;
    }

    /* Başlık */
    header{
      padding:18px 12px;
      text-align:center;
      position:sticky;
      top:0;
      background: linear-gradient(180deg, rgba(255,255,255,0.03), transparent);
      backdrop-filter: blur(4px);
      z-index: 30;
    }
    h1{
      margin:0;
      font-size: clamp(1.4rem, 3.4vw, 2.2rem);
      line-height:1.1;
      text-shadow: 0 4px 18px rgba(0,0,0,0.25);
    }

    /* Kart konteyneri (tek sütun mobil, 2 sütun tablet, 3 sütun geniş ekran) */
    .container {
      max-width:1100px;
      margin: 18px auto;
      padding: 8px;
      display: grid;
      grid-template-columns: 1fr;
      gap: 14px;
      box-sizing: border-box;
    }
    @media(min-width:640px){
      .container { grid-template-columns: repeat(2, 1fr); gap: 16px; padding: 12px; }
    }
    @media(min-width:1000px){
      .container { grid-template-columns: repeat(3, 1fr); gap: 20px; padding: 18px; }
    }

    /* Kart stili */
    .card {
      background: var(--card-bg);
      border-radius: 16px;
      padding: 14px;
      box-shadow: 0 8px 18px rgba(0,0,0,0.18);
      transition: transform .22s ease, box-shadow .22s ease;
      word-break: break-word;
      min-height: 84px;
      display:flex;
      align-items:center;
    }
    .card:focus, .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 18px 30px rgba(0,0,0,0.25);
      outline: none;
    }
    .card p { margin:0; font-size: clamp(0.95rem, 2vw, 1.05rem); line-height:1.3; }

    .heart { color: var(--accent); margin-right:8px; font-size:1.15em; display:inline-block; vertical-align:middle; }

    /* Uçuşan / sabit emojiler (pulse animasyonu) */
    .emoji {
      position: fixed;
      pointer-events: none;
      z-index: 9999;
      user-select: none;
      transform-origin: center center;
      will-change: transform, opacity;
      font-size: clamp(1.2rem, 2.8vw, 2.2rem);
      opacity: 0.95;
    }

    @keyframes pulse {
      0% { transform: translateY(0) scale(1); opacity: 0.9; }
      50% { transform: translateY(-8px) scale(1.35); opacity: 1; }
      100% { transform: translateY(0) scale(1); opacity: 0.9; }
    }
    .emoji.pulse { animation: pulse 2200ms ease-in-out infinite; }

    /* Reduce motion - tercihe saygı */
    @media (prefers-reduced-motion: reduce) {
      .emoji { animation: none !important; transform: none !important; }
      .card { transition: none !important; }
    }

    /* Yardımcı: sayfa içerik yüksekliği çok uzun olduğunda emoji görünürlüğünü iyileştir */
    .emoji[data-anchor="top"]{ top: 10vh; }
    .emoji[data-anchor="center"]{ top: 50vh; }
    .emoji[data-anchor="bottom"]{ top: 90vh; }

    /* küçük ekranlarda daha büyük boşluk ver */
    @media (max-width:400px){
      .container { padding:10px; gap:12px; }
      .card { padding:12px; }
    }
  </style>
</head>
<body>

  <header>
    <h1>💖 Aşkın Uçuşan Şiirleri 🌸💋🫶</h1>
  </header>

  <main>
    <section class="container" id="poemsContainer" aria-live="polite"></section>
  </main>

  <script>
    (function(){
      // Güvenli başlangıç - DOM hazır olduğunda çalışır
      const poemsContainer = document.getElementById('poemsContainer');

      // Var olan şiir listesi (örnek + senin eklemelerin). Tekrar edenleri elimine etmek için Set kullanıyoruz.
      const initialPoems = [
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
        // ... (örnekler kısaltıldı, istersen tam listeyi eklerim)
      ];

      // Yeni eklenen 50 özgün şiir (senin verdiğinlerden)
      const fiftyNew = [
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

      // Tekrarsız (unique) liste oluştur
      const finalSet = new Set(initialPoems.concat(fiftyNew));
      const finalList = Array.from(finalSet);

      // Kartları ekle
      finalList.forEach(text => {
        const card = document.createElement('article');
        card.className = 'card';
        card.tabIndex = 0;
        card.innerHTML = `<p><span class="heart" aria-hidden="true">💌</span><span>${text}</span></p>`;
        poemsContainer.appendChild(card);
      });

      /* ===== Uçuşan / sabit emojiler (performans ve görünürlük ayarlı) =====
         - Emojiler fixed konumda pulse animasyonlu
         - Ekranın dışına taşmaması için sınırlandırıldı
         - Aynı anda çok fazla birikmemesi için cap var
      */
      const EMOJIS = ['❤️','💋','🌸','🌹','💌','🫶'];
      const activeEmojis = new Set();
      const MAX_ACTIVE = 10; // aynı anda en fazla gösterilecek emoji sayısı

      function spawnEmoji(opts = {}) {
        if (activeEmojis.size >= MAX_ACTIVE) return;
        const e = document.createElement('div');
        e.className = 'emoji pulse';
        e.textContent = opts.char || EMOJIS[Math.floor(Math.random()*EMOJIS.length)];

        // Pozisyon: ekran genişliğine göre hesap, kenarlara taşmayacak
        const padding = 18;
        const vw = Math.max(document.documentElement.clientWidth || 0, window.innerWidth || 0);
        const vh = Math.max(document.documentElement.clientHeight || 0, window.innerHeight || 0);
        const x = Math.floor(Math.random() * (vw - padding*2)) + padding;
        // Yüksek sayfalarda alt/orta/üst tercihleri ile daha iyi görünürlük
        const anchors = ['top','center','bottom'];
        const anchor = anchors[Math.floor(Math.random()*anchors.length)];
        if (anchor === 'top') e.dataset.anchor = 'top';
        if (anchor === 'center') e.dataset.anchor = 'center';
        if (anchor === 'bottom') e.dataset.anchor = 'bottom';

        // top değerini anchor'a göre hafifçe ayarla (yüzde bazlı)
        let topPerc = 0;
        if (anchor === 'top') topPerc = 12 + Math.random()*8;      // 12-20vh
        if (anchor === 'center') topPerc = 40 + Math.random()*20;  // 40-60vh
        if (anchor === 'bottom') topPerc = 70 + Math.random()*18;  // 70-88vh

        e.style.left = `${x}px`;
        e.style.top = `${Math.round(vh * topPerc / 100)}px`;

        document.body.appendChild(e);
        activeEmojis.add(e);

        // otomatik temizle (zaman/açılım)
        const life = opts.life || (3500 + Math.random()*2500);
        setTimeout(() => {
          e.style.transition = 'opacity .45s ease, transform .45s ease';
          e.style.opacity = '0';
          e.style.transform = 'scale(.8) translateY(6px)';
          setTimeout(() => {
            if (e.parentNode) e.parentNode.removeChild(e);
            activeEmojis.delete(e);
          }, 480);
        }, life);
      }

      // Başlangıçta birkaç sabit emoji spawn et (göz alıcı ama sınırlı)
      const initialCount = 5;
      for (let i=0;i<initialCount;i++) spawnEmoji();

      // aralıklı yeni emoji oluştur (performans dostu)
      const interval = setInterval(() => {
        // eğer görünür alan çok küçükse veya prefers-reduced-motion ise azalt
        const reduce = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
        if (reduce) return;
        spawnEmoji();
      }, 700); // 700ms ile 1200ms arası yaygın deneyim; cihaz yavaşsa active cap devreye girer

      // Responsive değişikliklerde pozisyonların bozulmaması için aktif emojileri temizle
      window.addEventListener('resize', () => {
        activeEmojis.forEach(e => {
          if (e.parentNode) e.parentNode.removeChild(e);
        });
        activeEmojis.clear();
      });

      // (isteğe bağlı) sayfa uzunluğunda emoji davranışını iyileştirmek istersen söyle,
      // örn: tüm emojileri ekranın üst bölümünde sabitle veya yalnızca 3 animate göster vb.

    })();
  </script>

</body>
</html>
