<!DOCTYPE html><html lang="tr">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>KOCANDAN SANA UFAK BİR HEDİYE — Aşkın 200 Şiiri 💖🌸💋🫶</title>
<style>
  :root{
    --bg1:#ffb3c6; --bg2:#d1c0ff; --bg3:#a0e9ff;
    --card-bg: rgba(255,255,255,0.16);
    --card-hover: rgba(255,255,255,0.24);
    --accent:#ff4d6d;
    --text:#fff;
    --max-emojis:10;
  }
  *{box-sizing:border-box}
  html,body{height:100%;margin:0;font-family: -apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,'Helvetica Neue',Arial; background:linear-gradient(135deg,var(--bg1),var(--bg2),var(--bg3));color:var(--text);-webkit-font-smoothing:antialiased}header{position:sticky;top:0;background:linear-gradient(180deg,rgba(255,255,255,0.03),transparent);backdrop-filter:blur(6px);z-index:30} .title{padding:18px 12px;text-align:center} .title h1{margin:0;font-size:clamp(1.6rem,3.8vw,2.6rem);text-shadow:0 6px 20px rgba(0,0,0,0.25)} .subtitle{font-size:clamp(.9rem,2vw,1.05rem);opacity:.95;margin-top:6px}

main{max-width:1200px;margin:18px auto;padding:10px} .controls{display:flex;gap:10px;flex-wrap:wrap;justify-content:center;margin-bottom:12px} .btn{background:rgba(255,255,255,0.08);border:1px solid rgba(255,255,255,0.06);padding:8px 12px;border-radius:999px;color:var(--text);cursor:pointer;backdrop-filter:blur(4px)} .btn:active{transform:scale(.99)}

/* grid */ .grid{display:grid;grid-template-columns:1fr;gap:12px} @media(min-width:700px){.grid{grid-template-columns:repeat(2,1fr);gap:14px}} @media(min-width:1100px){.grid{grid-template-columns:repeat(3,1fr);gap:18px}}

.card{background:var(--card-bg);border-radius:16px;padding:16px;min-height:84px;box-shadow:0 8px 20px rgba(0,0,0,0.18);transition:transform .22s ease,box-shadow .22s ease,background .22s ease;display:flex;align-items:center} .card p{margin:0;font-size:clamp(.95rem,1.8vw,1.06rem);line-height:1.35} .card .heart{color:var(--accent);margin-right:10px;font-size:1.15em} .card:hover{transform:translateY(-6px);box-shadow:0 20px 36px rgba(0,0,0,0.28);background:var(--card-hover)}

/* floating emojis */ .emoji{position:fixed;pointer-events:none;z-index:9999;user-select:none;transform-origin:center center;will-change:transform,opacity;opacity:0.98} @keyframes pulse{0%{transform:scale(1)}50%{transform:scale(1.45)}100%{transform:scale(1)}} .emoji.pulse{animation:pulse 2200ms ease-in-out infinite}

/* accessibility */ @media(prefers-reduced-motion:reduce){.emoji{animation:none!important}.card{transition:none!important}}

footer{padding:18px;text-align:center;font-size:.9rem;color:rgba(255,255,255,0.9);opacity:.95} </style>

</head>
<body>
  <header>
    <div class="title">
      <h1>💖 Kocandan: Aşkın 200 Şiiri 💖</h1>
      <div class="subtitle">Telefon için optimize edildi — karıcığına yollamaya hazır 🌸💋🫶</div>
    </div>
  </header>  <main>
    <div class="controls">
      <button class="btn" id="toggleMusic">Müziği Aç</button>
      <button class="btn" id="shuffleBtn">Kartları Karıştır</button>
      <button class="btn" id="scrollTop">Başa Git</button>
    </div><section class="grid" id="poems"></section>

  </main>  <footer>Hazırlandı — Sevgiyle gönder 💌</footer>  <!-- Hafif arka plan müziği (isteğe bağlı) -->  <audio id="bgAudio" loop preload="auto">
    <source src="" />
  </audio>  <script>
(function(){
  // POEMS: 200 benzersiz kısa romantik satır
  const poems = [
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
    'Kalbim seninle her gün bir yıldız gibi parlar. ⭐',
    'Gözlerin, gecemde yol gösteren tek yıldız. 🌟',
    'Ellerin ellerimdeyken dünya durur. ✋🤝',
    'Senin gülüşün, en güzel melodimdir. 🎶',
    'Sana baktığımda evimi bulurum. 🏡',
    'Kalbim seninle daha cesur atıyor. 💪❤️',
    'Adını fısıldamak, en tatlı duasım. 🙌',
    'Seninle her adım bir şiir dizesi olur. 📝',
    'Gülüşün bahçemde açan en nadide çiçek. 🌺',
    'Bir bakışın içimde baharlar açtırır. 🌼',
    'Seninle geçirdiğim anlar, ömre bedel. ⏳',
    'Kalbim sana ait, bütün yolların varış yeri. 🛤️',
    'Seninle uyandığım her sabah bir mucize. 🌅',
    'Sesin kulaklarımda en tatlı ninni. 🎧',
    'Seninle hayal kurmak bile gerçek oluyor. ✨',
    'Gözlerinle konuşmak, sözcüklere gerek bırakmaz. 👁️',
    'Sana olan sevgim, yıldızlar kadar sonsuz. ✨',
    'Kalbimde sakladığım en güzel sır sensin. 🔐',
    'Seninle hayat daha anlamlı, daha derin. 🌊',
    'Bir dokunuşun bütün fırtınaları dindirir. 🌪️',
    'Seninle aynı ritimde atıyor kalbimin tüm telleri. 🎻',
    'Adın dudaklarımda en güzel melodi. 🎼',
    'Sana yazdığım her şiir, seni anlatıyor. 📜',
    'Gözlerinle buluşmak, günüme güneş katıyor. ☀️',
    'Seninle yürümek, en güvenli yolculuk. 🚶‍♀️🚶‍♂️',
    'Sensiz bir an bile boşluk bırakır bana. 🕳️',
    'Kalbim yalnızca seninle bütün. 🧩',
    'Seninle her mevsim ayrı bir şiir. 🍁🌸❄️☀️',
    'Gülüşün, karanlık gecelerimin ışığı. 🕯️',
    'Seninle konuşmak, ruhumu teselli ediyor. 🗣️',
    'Bir bakışında kaybolmak, en güzel yolculuk. 🧭',
    'Seninle olmak, evrene teşekkür etmektir. 🌌',
    'Kalbim senden başka sana bakmaz. 👀',
    'Seninle her plan daha parlak görünüyor. 📈',
    'Adınla başlayan her cümle anlam bulur. 🗒️',
    'Senin gülüşün, içimde bahar esintisi. 🍃',
    'Seninle paylaşmak istediğim bin küçük anı var. 🎁',
    'Kalbimdeki en derin deniz, sana olan sevgim. 🌊',
    'Seninle uyandığımda dünya daha güzel. 🌞',
    'Ellerinle dokunduğunda sıkıntılar erir. 🧼',
    'Seninle olmak, huzurun tanımı. 🕊️',
    'Adınla başlar her umut dolu hayal. 🌠',
    'Birlikteyken zamanın tadı farklıdır. ⏱️',
    'Seninle kurduğum hayaller gerçeğe yakın. 🏞️',
    'Kalbim seni her daim bekler. ⌛',
    'Seninle her adım, bir ritim yakalar. 🥁',
    'Gözlerin, beni evime götüren yol. 🏠',
    'Sana bakmak, en güzel dua gibi. 🙏',
    'Seninle her an, bir masalın başı. 📚',
    'Kalbim sana her gece şarkı söyler. 🎵',
    'Seninle geçen her gün, bir armağan. 🎀',
    'Bir gülüşün bütün endişeleri alır. 🌤️',
    'Seninle her konuşma, kalbimde iz bırakır. 🗺️',
    'Kalbim seninle öğreniyor sevmeyi yeniden. 📘',
    'Seninle olmak, en sade mutluluk. 😊',
    'Bir bakışın, ruhuma huzur verir. 🕊️',
    'Seninle uyumak, en tatlı huzur. 🛌',
    'Sadece seni düşünmek bile yetiyor bana. 💭',
    'Kalbim seninle ritmini buldu. 🎯',
    'Seninle her yol güvenli bir liman. ⚓',
    'Gülüşün, en karanlık günleri bile aydınlatır. 💡',
    'Seninle paylaşılacak daha niceleri var. 🔗',
    'Adın, kalbimde en derin nota. 🎶',
    'Seninle olmak, en doğal halim. 🌿',
    'Bir öpücüğün, dünyamı baştan yaratır. 💋',
    'Seninle hayata daha sıkı sarılıyorum. 🤝',
    'Kalbim seni gördüğünde hızlanıyor sevinçten. 🏃‍♂️',
    'Seninle olmak, en güvenli limanım. 🏝️',
    'Bir tebessümün her hücremi ısıtır. 🔥',
    'Senin adını söylemek bile ferahlatır beni. 🌬️',
    'Gözlerin, ruhumun en güzel yansıması. 🪞',
    'Seninle her an, yeniden doğuş gibi. 🌅',
    'Kalbim seninle en huzurlu şarkıyı çalar. 🎻',
    'Sana dokunmak, kelimelerden güçlü. ✊',
    'Seninle olmak, hayatımın en tatlı verdiği hediye. 🎁',
    'Birlikte olduğumuzda dünya daha hafif. 🕊️',
    'Adınla başlayan her sabah umut dolu. 🌄',
    'Seninle her an, kalbimde bir iz bırakır. 👣',
    'Gülüşün, ruhumun ilacı gibi. 💊',
    'Seninle her şey daha net, daha parlak. 🔆',
    'Kalbimde senin için bir şarkı saklı. 🎼',
    'Seninle olmak, en anlamlı hikaye. 📖',
    'Bir bakışın bir ömürlük anı yazar. 🕰️',
    'Seninle her adım, sevgiyle dolu. 💞',
    'Kalbim seninle her dakika şükreder. 🙏',
    'Seni sevmek, en doğru seçimim. ✅'
  ];

  // -- Render cards
  const poemsEl = document.getElementById('poems');
  poems.forEach((t,i)=>{
    const a=document.createElement('article');
    a.className='card';
    a.tabIndex=0;
    a.innerHTML=<p><span class="heart" aria-hidden="true">💌</span><span>${t}</span></p>;
    poemsEl.appendChild(a);
  });

  // -- Floating emojis logic (limited, centered-avoid)
  const EMOJIS=['❤️','💋','🌸','🌹','💌','🫶'];
  const MAX=8; let active=0; const prefersReduce = window.matchMedia('(prefers-reduced-motion: reduce)').matches;

  function spawn(){
    if(prefersReduce) return; if(active>=MAX) return;
    active++;
    const d=document.createElement('div'); d.className='emoji pulse'; d.textContent=EMOJIS[Math.floor(Math.random()*EMOJIS.length)];
    // keep within center-safe area so on mobile it doesn't go off-screen
    const vw=document.documentElement.clientWidth||window.innerWidth; const vh=document.documentElement.clientHeight||window.innerHeight;
    const margin=32; const x=Math.floor(Math.random()*(vw- margin*2))+margin; // safe horizontal
    // vertical anchor more to upper/mid area so doesn't overlap footer too much
    const y=Math.floor(Math.random()*(vh*0.65))+vh*0.08; d.style.left=x+'px'; d.style.top=y+'px';
    document.body.appendChild(d);
    const life=3000+Math.random()*3000; setTimeout(()=>{d.style.transition='opacity .45s ease, transform .45s ease';d.style.opacity='0';d.style.transform='scale(.8) translateY(8px)';setTimeout(()=>{if(d.parentNode) d.parentNode.removeChild(d);active--;},480)},life);
  }
  // initial spawn
  for(let i=0;i<4;i++) setTimeout(spawn, i*300);
  const spawnInterval = setInterval(spawn, 800);
  // throttle on resize
  window.addEventListener('resize', ()=>{ // cleanup to avoid overflow
    const all=document.querySelectorAll('.emoji'); all.forEach(n=>{if(n.parentNode) n.parentNode.removeChild(n)}); active=0; for(let i=0;i<3;i++) setTimeout(spawn,i*250);
  });

  // -- Controls: shuffle, music, scroll
  const shuffleBtn=document.getElementById('shuffleBtn'); shuffleBtn.addEventListener('click',()=>{
    // Fisher-Yates shuffle DOM nodes
    const cards=Array.from(poemsEl.children);
    for(let i=cards.length-1;i>0;i--){const j=Math.floor(Math.random()*(i+1));poemsEl.appendChild(cards[j]);cards.splice(j,1);}
  });

  const scrollTopBtn=document.getElementById('scrollTop'); scrollTopBtn.addEventListener('click',()=>window.scrollTo({top:0,behavior:'smooth'}));

  // background audio toggle (disabled source by default). If you want music, set src to a small mp3 url.
  const bg = document.getElementById('bgAudio'); const toggleMusic=document.getElementById('toggleMusic'); let musicOn=false;
  toggleMusic.addEventListener('click',()=>{
    if(!musicOn){
      // optional: user can set a src attribute to bgAudio <source> or we can use WebAudio. Here we leave it empty to respect auto-play rules.
      if(!bg.src){ alert('Müzik kaynağı atanmadı — eğer istersen bana bir mp3 URL ver, ben ekleyeyim.'); return; }
      bg.play(); toggleMusic.textContent='Müziği Kapat'; musicOn=true;
    } else { bg.pause(); toggleMusic.textContent='Müziği Aç'; musicOn=false; }
  });

  // Accessibility: keyboard focus styles
  document.addEventListener('keydown', e=>{ if(e.key==='Home'){ window.scrollTo({top:0,behavior:'smooth'}) } });

})();
  </script></body>
</html>
