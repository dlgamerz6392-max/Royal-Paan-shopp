<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Royal Paan Shop — Katwa Mod, Kasimabad Road</title>
<meta name="description" content="Royal Paan Shop, Katwa Mod, Kasimabad Road — Meetha, Banarasi, Gulkand, Chocolate, Fire & Shahi Dry Fruit Paan. Fresh, hand-rolled, royally loaded.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Yatra+One&family=Mukta:wght@300;400;500;600;700&family=Rajdhani:wght@500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --maroon-deep:#240B10;
    --maroon-card:#34121A;
    --maroon-card-2:#3D161F;
    --gold:#D4AF37;
    --gold-soft:#EAD089;
    --leaf:#4C8B5A;
    --leaf-deep:#1F4D2C;
    --cream:#F6EEE0;
    --cream-dim:#CDBBA7;
    --ember:#D24B3E;
    --line: rgba(212,175,55,0.22);
  }

  *{box-sizing:border-box; margin:0; padding:0;}

  html{scroll-behavior:smooth;}

  body{
    background:var(--maroon-deep);
    color:var(--cream);
    font-family:'Mukta', sans-serif;
    font-weight:400;
    line-height:1.6;
    overflow-x:hidden;
  }

  img{max-width:100%; display:block;}

  .eyebrow{
    font-family:'Rajdhani', sans-serif;
    font-weight:600;
    letter-spacing:0.28em;
    text-transform:uppercase;
    font-size:0.72rem;
    color:var(--gold-soft);
  }

  h1, h2, h3, .display{
    font-family:'Yatra One', cursive;
    font-weight:400;
    letter-spacing:0.01em;
  }

  a{color:inherit; text-decoration:none;}

  .wrap{
    max-width:1180px;
    margin:0 auto;
    padding:0 28px;
  }

  /* ---------- NAV ---------- */
  header.nav{
    position:sticky; top:0; z-index:50;
    background:rgba(36,11,16,0.88);
    backdrop-filter:blur(8px);
    border-bottom:1px solid var(--line);
  }
  .nav-inner{
    max-width:1180px; margin:0 auto; padding:14px 28px;
    display:flex; align-items:center; justify-content:space-between;
  }
  .brandmark{
    display:flex; align-items:center; gap:10px;
  }
  .brandmark svg{width:30px; height:30px; flex-shrink:0;}
  .brand-text{
    font-family:'Yatra One', cursive;
    font-size:1.3rem;
    color:var(--gold);
    line-height:1;
  }
  .brand-text small{
    display:block;
    font-family:'Rajdhani', sans-serif;
    font-size:0.6rem;
    letter-spacing:0.25em;
    color:var(--cream-dim);
    margin-top:3px;
  }
  .nav-links{display:flex; gap:28px; align-items:center;}
  .nav-links a{
    font-family:'Rajdhani', sans-serif;
    font-weight:600;
    font-size:0.85rem;
    letter-spacing:0.06em;
    text-transform:uppercase;
    color:var(--cream-dim);
    transition:color .2s ease;
  }
  .nav-links a:hover{color:var(--gold);}
  .nav-call{
    background:var(--gold);
    color:var(--maroon-deep) !important;
    padding:9px 18px;
    border-radius:3px;
    font-weight:700 !important;
  }
  .nav-burger{display:none;}

  @media(max-width:760px){
    .nav-links a:not(.nav-call){display:none;}
  }

  /* ---------- HERO ---------- */
  .hero{
    position:relative;
    min-height:92vh;
    display:flex;
    align-items:flex-end;
    background:#000;
  }
  .hero-img{
    position:absolute; inset:0;
    width:100%; height:100%;
    object-fit:cover;
    object-position:60% 30%;
    opacity:0.62;
  }
  .hero::after{
    content:"";
    position:absolute; inset:0;
    background:
      linear-gradient(0deg, var(--maroon-deep) 4%, rgba(36,11,16,0.35) 48%, rgba(36,11,16,0.55) 100%),
      linear-gradient(90deg, rgba(36,11,16,0.92) 0%, rgba(36,11,16,0.25) 62%);
  }
  .hero-content{
    position:relative; z-index:2;
    padding:120px 28px 64px;
    max-width:1180px;
    margin:0 auto;
    width:100%;
  }
  .hero-devanagari{
    font-family:'Yatra One', cursive;
    font-size:1.5rem;
    color:var(--gold-soft);
    margin-bottom:6px;
    opacity:0.9;
  }
  .hero h1{
    font-size:clamp(2.6rem, 7vw, 5.2rem);
    color:var(--cream);
    line-height:1.02;
    max-width:780px;
  }
  .hero h1 span{color:var(--gold);}
  .hero-tag{
    font-family:'Rajdhani', sans-serif;
    font-size:clamp(1rem, 2vw, 1.3rem);
    font-weight:600;
    letter-spacing:0.04em;
    color:var(--leaf);
    margin-top:18px;
    max-width:520px;
  }
  .hero-loc{
    margin-top:10px;
    font-size:0.95rem;
    color:var(--cream-dim);
  }
  .hero-cta{
    display:flex; gap:14px; margin-top:34px; flex-wrap:wrap;
  }
  .btn{
    display:inline-flex; align-items:center; gap:9px;
    padding:13px 26px;
    border-radius:3px;
    font-family:'Rajdhani', sans-serif;
    font-weight:700;
    font-size:0.95rem;
    letter-spacing:0.04em;
    text-transform:uppercase;
    border:1px solid transparent;
    transition:transform .18s ease, box-shadow .18s ease;
  }
  .btn:hover{transform:translateY(-2px);}
  .btn-gold{background:var(--gold); color:var(--maroon-deep);}
  .btn-gold:hover{box-shadow:0 10px 26px -8px rgba(212,175,55,0.55);}
  .btn-outline{border-color:var(--cream-dim); color:var(--cream);}
  .btn-outline:hover{border-color:var(--gold); color:var(--gold);}

  /* ---------- TICKER ---------- */
  .ticker{
    background:var(--leaf-deep);
    border-top:1px solid rgba(212,175,55,0.3);
    border-bottom:1px solid rgba(212,175,55,0.3);
    overflow:hidden;
    white-space:nowrap;
    padding:13px 0;
  }
  .ticker-track{
    display:inline-block;
    animation:scrollTicker 32s linear infinite;
    font-family:'Rajdhani', sans-serif;
    font-weight:600;
    letter-spacing:0.1em;
    text-transform:uppercase;
    font-size:0.92rem;
    color:var(--gold-soft);
  }
  .ticker-track span{margin:0 22px;}
  .ticker-track span.dot{color:var(--leaf); opacity:0.7;}
  @keyframes scrollTicker{
    from{transform:translateX(0);}
    to{transform:translateX(-50%);}
  }

  /* ---------- SECTION GENERIC ---------- */
  section{padding:96px 0;}
  .section-head{
    text-align:center;
    max-width:640px;
    margin:0 auto 56px;
  }
  .section-head h2{
    font-size:clamp(2rem, 4vw, 2.8rem);
    color:var(--cream);
    margin-top:10px;
  }
  .section-head p{
    color:var(--cream-dim);
    margin-top:14px;
    font-size:1.02rem;
  }
  .divider-leaf{
    width:34px; height:34px;
    margin:0 auto 14px;
    color:var(--leaf);
  }

  /* ---------- ABOUT ---------- */
  .about-grid{
    display:grid;
    grid-template-columns:0.85fr 1.15fr;
    gap:64px;
    align-items:center;
  }
  .about-img-wrap{
    position:relative;
  }
  .leaf-frame{
    clip-path: url(#leafClip);
    width:100%;
    aspect-ratio: 1/1.05;
    object-fit:cover;
    background:#111;
  }
  .about-img-wrap::after{
    content:"";
    position:absolute; top:18px; left:18px; right:-18px; bottom:-18px;
    border:1px solid var(--gold);
    opacity:0.45; z-index:-1;
    clip-path: url(#leafClip);
  }
  .about-body .eyebrow{margin-bottom:10px; display:block;}
  .about-body h2{font-size:clamp(1.8rem,3.4vw,2.4rem); color:var(--cream); margin-bottom:18px;}
  .about-body p{color:var(--cream-dim); margin-bottom:14px; max-width:520px;}
  .about-stats{
    display:flex; gap:36px; margin-top:30px; flex-wrap:wrap;
  }
  .about-stats div b{
    display:block;
    font-family:'Yatra One', cursive;
    font-size:1.7rem;
    color:var(--gold);
  }
  .about-stats div span{
    font-family:'Rajdhani', sans-serif;
    font-size:0.78rem;
    letter-spacing:0.08em;
    text-transform:uppercase;
    color:var(--cream-dim);
  }

  /* ---------- SIGNATURE ---------- */
  .signature{background:var(--maroon-card);}
  .sig-grid{
    display:grid;
    grid-template-columns:repeat(3, 1fr);
    gap:28px;
  }
  .sig-card{
    background:var(--maroon-card-2);
    border:1px solid var(--line);
    border-radius:6px;
    overflow:hidden;
    transition:transform .25s ease, border-color .25s ease;
  }
  .sig-card:hover{transform:translateY(-6px); border-color:var(--gold);}
  .sig-img{width:100%; height:230px; object-fit:cover;}
  .sig-body{padding:24px 22px 28px;}
  .sig-badge{
    display:inline-block;
    font-family:'Rajdhani', sans-serif;
    font-size:0.68rem;
    letter-spacing:0.12em;
    text-transform:uppercase;
    color:var(--ember);
    border:1px solid var(--ember);
    padding:3px 9px;
    border-radius:20px;
    margin-bottom:12px;
  }
  .sig-body h3{font-size:1.4rem; color:var(--gold-soft); margin-bottom:8px;}
  .sig-body p{font-size:0.92rem; color:var(--cream-dim);}
  .flame{
    display:inline-block;
    animation:flicker 1.6s infinite ease-in-out;
  }
  @keyframes flicker{
    0%,100%{transform:scale(1) rotate(-1deg); opacity:1;}
    50%{transform:scale(1.08) rotate(2deg); opacity:0.85;}
  }

  /* ---------- MENU ---------- */
  .menu-grid{
    display:grid;
    grid-template-columns:repeat(3, 1fr);
    gap:16px;
  }
  .menu-item{
    background:var(--maroon-card);
    border:1px solid var(--line);
    border-radius:6px;
    padding:20px 22px;
    display:flex; align-items:center; gap:14px;
    transition:border-color .2s ease, background .2s ease;
  }
  .menu-item:hover{border-color:var(--gold); background:var(--maroon-card-2);}
  .menu-item .leaf-ico{width:22px; height:22px; color:var(--leaf); flex-shrink:0;}
  .menu-item span{
    font-family:'Mukta', sans-serif;
    font-weight:600;
    font-size:1rem;
    color:var(--cream);
  }
  .menu-note{
    text-align:center;
    margin-top:30px;
    color:var(--cream-dim);
    font-size:0.92rem;
  }

  /* ---------- GALLERY ---------- */
  .gallery{background:var(--maroon-card);}
  .gal-grid{
    display:grid;
    grid-template-columns:repeat(4, 1fr);
    grid-auto-rows:160px;
    gap:14px;
  }
  .gal-grid img{
    width:100%; height:100%; object-fit:cover;
    border-radius:6px;
    transition:transform .35s ease, filter .35s ease;
    filter:saturate(1.05);
  }
  .gal-grid img:hover{transform:scale(1.035);}
  .gal-grid a:nth-child(1){grid-column:span 2; grid-row:span 2;}
  .gal-grid a:nth-child(4){grid-column:span 2;}

  /* ---------- VISIT ---------- */
  .visit-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:0;
    border:1px solid var(--line);
    border-radius:8px;
    overflow:hidden;
  }
  .visit-info{
    background:var(--maroon-card);
    padding:52px 48px;
  }
  .visit-info h2{font-size:2rem; color:var(--cream); margin-bottom:24px;}
  .visit-row{
    display:flex; gap:16px; margin-bottom:22px; align-items:flex-start;
  }
  .visit-row svg{width:20px; height:20px; color:var(--gold); flex-shrink:0; margin-top:3px;}
  .visit-row b{display:block; color:var(--cream); font-size:0.98rem; margin-bottom:2px;}
  .visit-row span, .visit-row a{color:var(--cream-dim); font-size:0.92rem;}
  .visit-row a:hover{color:var(--gold);}
  .visit-cta{display:flex; gap:12px; margin-top:30px; flex-wrap:wrap;}
  .visit-map{
    position:relative;
    background:
      repeating-linear-gradient(45deg, rgba(212,175,55,0.05) 0 2px, transparent 2px 14px),
      var(--leaf-deep);
    display:flex; align-items:center; justify-content:center;
    min-height:340px;
  }
  .visit-map-pin{
    text-align:center;
  }
  .visit-map-pin svg{width:46px; height:46px; color:var(--gold); margin-bottom:10px;}
  .visit-map-pin p{
    font-family:'Rajdhani', sans-serif;
    font-weight:600;
    letter-spacing:0.06em;
    text-transform:uppercase;
    font-size:0.85rem;
    color:var(--cream);
  }
  .visit-map-pin span{
    display:block;
    font-size:0.78rem;
    color:var(--cream-dim);
    margin-top:4px;
  }

  /* ---------- FOOTER ---------- */
  footer{
    background:var(--maroon-deep);
    border-top:1px solid var(--line);
    padding:48px 0 28px;
  }
  .foot-inner{
    display:flex; justify-content:space-between; align-items:center; flex-wrap:wrap; gap:20px;
  }
  .foot-brand{font-family:'Yatra One', cursive; font-size:1.3rem; color:var(--gold);}
  .foot-brand small{display:block; font-family:'Mukta',sans-serif; font-size:0.78rem; color:var(--cream-dim); margin-top:4px;}
  .foot-links{display:flex; gap:22px;}
  .foot-links a{font-size:0.85rem; color:var(--cream-dim);}
  .foot-links a:hover{color:var(--gold);}
  .foot-bottom{
    text-align:center; margin-top:34px; padding-top:22px;
    border-top:1px solid rgba(212,175,55,0.12);
    font-size:0.8rem; color:var(--cream-dim);
  }

  /* ---------- WHATSAPP FLOAT ---------- */
  .wa-float{
    position:fixed; bottom:24px; right:24px; z-index:60;
    width:58px; height:58px; border-radius:50%;
    background:#2EAD53;
    display:flex; align-items:center; justify-content:center;
    box-shadow:0 10px 28px -6px rgba(0,0,0,0.55);
    transition:transform .2s ease;
  }
  .wa-float:hover{transform:scale(1.08);}
  .wa-float svg{width:28px; height:28px; color:#fff;}

  /* ---------- RESPONSIVE ---------- */
  @media(max-width:900px){
    .about-grid{grid-template-columns:1fr; gap:40px;}
    .sig-grid{grid-template-columns:1fr;}
    .menu-grid{grid-template-columns:repeat(2,1fr);}
    .gal-grid{grid-template-columns:repeat(2,1fr); grid-auto-rows:150px;}
    .gal-grid a:nth-child(1){grid-column:span 2; grid-row:span 1;}
    .visit-grid{grid-template-columns:1fr;}
    .visit-info{padding:40px 26px;}
  }
  @media(max-width:560px){
    .menu-grid{grid-template-columns:1fr;}
    .hero-content{padding-top:100px;}
  }

  @media (prefers-reduced-motion: reduce){
    *{animation-duration:0.001ms !important; animation-iteration-count:1 !important; transition-duration:0.001ms !important; scroll-behavior:auto !important;}
  }

  :focus-visible{outline:2px solid var(--gold); outline-offset:3px;}
</style>
</head>
<body>

<svg width="0" height="0" style="position:absolute" aria-hidden="true">
  <defs>
    <clipPath id="leafClip" clipPathUnits="objectBoundingBox">
      <path d="M0.03,0.49 C0.03,0.20 0.30,0.02 0.67,0.02 C1.00,0.02 0.98,0.49 0.67,0.84 C0.33,0.98 0.03,0.79 0.03,0.49 Z"/>
    </clipPath>
  </defs>
</svg>

<header class="nav">
  <div class="nav-inner">
    <div class="brandmark">
      <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
        <path d="M20 4C12 4 5 12 5 21C5 30 11 35 20 35C29 35 35 30 35 21C35 12 28 4 20 4Z" stroke="#D4AF37" stroke-width="1.6"/>
        <path d="M20 9C24 13 27 17 27 22C27 27 24 30 20 30C16 30 13 27 13 22C13 17 16 13 20 9Z" fill="#4C8B5A"/>
      </svg>
      <div class="brand-text">Royal Paan<small>SHOP &nbsp;•&nbsp; EST. KATWA MOD</small></div>
    </div>
    <nav class="nav-links">
      <a href="#signature">Signature</a>
      <a href="#menu">Menu</a>
      <a href="#gallery">Gallery</a>
      <a href="#visit">Visit Us</a>
      <a href="tel:+919415970125" class="nav-call">Call Now</a>
    </nav>
  </div>
</header>

<section class="hero">
  <img class="hero-img" src="assets/fire-paan.jpg" alt="Flaming Fire Paan held in hand, signature of Royal Paan Shop">
  <div class="hero-content">
    <div class="hero-devanagari">रॉयल पान भंडार</div>
    <h1>Royal <span>Paan</span> Shop</h1>
    <p class="hero-tag">All Varieties of Paan Available — Hand-Rolled, Royally Loaded.</p>
    <p class="hero-loc">📍 Katwa Mod, Kasimabad Road</p>
    <div class="hero-cta">
      <a class="btn btn-gold" href="https://wa.me/919415970125" target="_blank" rel="noopener">WhatsApp Order</a>
      <a class="btn btn-outline" href="tel:+919415970125">Call 94159 70125</a>
    </div>
  </div>
</section>

<div class="ticker" aria-hidden="true">
  <div class="ticker-track">
    <span>Meetha Paan</span><span class="dot">•</span>
    <span>Banarasi Paan</span><span class="dot">•</span>
    <span>Gulkand Paan</span><span class="dot">•</span>
    <span>Chocolate Paan</span><span class="dot">•</span>
    <span>Fire Paan</span><span class="dot">•</span>
    <span>Shahi Dry Fruit Paan</span><span class="dot">•</span>
    <span>Meetha Paan</span><span class="dot">•</span>
    <span>Banarasi Paan</span><span class="dot">•</span>
    <span>Gulkand Paan</span><span class="dot">•</span>
    <span>Chocolate Paan</span><span class="dot">•</span>
    <span>Fire Paan</span><span class="dot">•</span>
    <span>Shahi Dry Fruit Paan</span><span class="dot">•</span>
  </div>
</div>

<section class="about">
  <div class="wrap about-grid">
    <div class="about-img-wrap">
      <img class="leaf-frame" src="assets/gulkand-paan.jpg" alt="Gulkand-stuffed betel leaf paan resting on flower petals">
    </div>
    <div class="about-body">
      <span class="eyebrow">Our Story</span>
      <h2>From One Leaf, a Hundred Flavours</h2>
      <p>Every paan at Royal Paan Shop starts the same way — a fresh betel leaf, washed and trimmed by hand at the counter on Kasimabad Road. What goes inside it after that is where things get royal.</p>
      <p>Owner Dharmendra Prajapati has spent years building a paan corner where the classics sit beside theatrical specials — rose-soaked gulkand, melting chocolate, crushed dry fruits, edible silver foil, and even paan served lit with fire. Stop by, and you'll usually find a small crowd waiting to watch one get made.</p>
      <div class="about-stats">
        <div><b>15+</b><span>Paan Varieties</span></div>
        <div><b>100%</b><span>Made to Order</span></div>
        <div><b>Daily</b><span>Fresh Leaves</span></div>
      </div>
    </div>
  </div>
</section>

<section class="signature" id="signature">
  <div class="wrap">
    <div class="section-head">
      <span class="eyebrow">What Makes Us Royal</span>
      <h2>Signature Creations</h2>
      <p>Three paans you won't find at every shop on the road — each one built, not just rolled.</p>
    </div>
    <div class="sig-grid">
      <div class="sig-card">
        <img class="sig-img" src="assets/fire-paan.jpg" alt="Fire Paan served lit with an open flame">
        <div class="sig-body">
          <span class="sig-badge"><span class="flame">🔥</span> Showstopper</span>
          <h3>Fire Paan</h3>
          <p>Lit tableside and served while the flame is still alive — a Royal Paan Shop original that's part dessert, part spectacle.</p>
        </div>
      </div>
      <div class="sig-card">
        <img class="sig-img" src="assets/shahi-loaded.png" alt="Shahi Dry Fruit Paan loaded with almonds, cashews, chocolate and silver foil">
        <div class="sig-body">
          <span class="sig-badge">House Special</span>
          <h3>Shahi Dry Fruit Paan</h3>
          <p>Almonds, cashews, chocolate chunks and silver foil piled onto a single leaf — our own recipe, made nowhere else nearby.</p>
        </div>
      </div>
      <div class="sig-card">
        <img class="sig-img" src="assets/gulkand-paan.jpg" alt="Gulkand Paan with rose petal stuffing">
        <div class="sig-body">
          <span class="sig-badge">Classic, Done Right</span>
          <h3>Gulkand Paan</h3>
          <p>Sweet rose petal preserve, slow-set and glistening, wrapped fresh in a single betel leaf. The one regulars keep coming back for.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="menu" id="menu">
  <div class="wrap">
    <div class="section-head">
      <span class="eyebrow">On The Leaf</span>
      <h2>Our Varieties</h2>
      <p>A full spread of sweet, traditional and festive paans — all rolled fresh on order.</p>
    </div>
    <div class="menu-grid">
      <div class="menu-item"><svg class="leaf-ico" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6 2 2 8 2 13c0 5 4 8 10 8s10-3 10-8c0-5-4-11-10-11zm0 4c2.5 2 4 5 4 7.5 0 2.5-1.8 4-4 4s-4-1.5-4-4C8 11 9.5 8 12 6z"/></svg><span>Meetha Paan</span></div>
      <div class="menu-item"><svg class="leaf-ico" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6 2 2 8 2 13c0 5 4 8 10 8s10-3 10-8c0-5-4-11-10-11zm0 4c2.5 2 4 5 4 7.5 0 2.5-1.8 4-4 4s-4-1.5-4-4C8 11 9.5 8 12 6z"/></svg><span>Banarasi Paan</span></div>
      <div class="menu-item"><svg class="leaf-ico" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6 2 2 8 2 13c0 5 4 8 10 8s10-3 10-8c0-5-4-11-10-11zm0 4c2.5 2 4 5 4 7.5 0 2.5-1.8 4-4 4s-4-1.5-4-4C8 11 9.5 8 12 6z"/></svg><span>Gulkand Paan</span></div>
      <div class="menu-item"><svg class="leaf-r
