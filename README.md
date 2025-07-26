<!DOCTYPE html><html lang="ar"><head><meta http-equiv="Content-Security-Policy" content="default-src 'self' 'unsafe-inline' 'unsafe-eval' data: blob: https://cdnjs.cloudflare.com https://cdn.jsdelivr.net https://code.jquery.com https://unpkg.com https://d3js.org https://threejs.org https://cdn.plot.ly https://stackpath.bootstrapcdn.com https://maps.googleapis.com https://cdn.tailwindcss.com https://ajax.googleapis.com https://kit.fontawesome.com https://cdn.datatables.net https://maxcdn.bootstrapcdn.com https://code.highcharts.com https://tako-static-assets-production.s3.amazonaws.com https://www.youtube.com https://fonts.googleapis.com https://fonts.gstatic.com https://pfst.cf2.poecdn.net https://puc.poecdn.net https://i.imgur.com https://wikimedia.org https://*.icons8.com https://*.giphy.com https://picsum.photos https://images.unsplash.com; frame-src 'self' https://www.youtube.com https://trytako.com; child-src 'self'; manifest-src 'self'; worker-src 'self'; upgrade-insecure-requests; block-all-mixed-content;">
  <meta charset="UTF-8">
  <title>Maison Cesar Caftan</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <!-- Google Fonts for Arabic and Latin -->
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@700&amp;family=Montserrat:wght@700&amp;display=swap" rel="stylesheet">
  <style>
    :root {
      --gold1: #bfa14c;
      --gold2: #f7e18b;
      --blue: #497bb1;
      --bg: #f6f9fc;
    }
    body {
      background: var(--bg);
      margin: 0;
      font-family: 'Montserrat', 'Cairo', Arial, sans-serif;
      color: #222;
    }
    .header {
      background: #fff;
      border-bottom: 1.5px solid var(--blue);
      box-shadow: 0 3px 16px 0 rgba(80,130,210,0.07);
      padding: 0;
      position: relative;
    }
    .logo-box {
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 32px 0 14px 0;
      gap: 18px;
    }
    .logo-svg {
      width: 70px;
      height: 70px;
      flex-shrink: 0;
    }
    .shop-name {
      font-family: 'Montserrat', 'Cairo', sans-serif;
      font-size: 2.1rem;
      font-weight: 700;
      letter-spacing: 1.5px;
      background: linear-gradient(92deg, var(--gold1) 10%, var(--gold2) 60%, var(--gold1) 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      color: var(--gold1);
      margin: 0;
      line-height: 1.1;
      text-align: left;
      text-shadow: 0 2px 10px #fff6;
    }
    .subtitle {
      font-family: 'Cairo', sans-serif;
      font-size: 1.18rem;
      color: var(--blue);
      margin: 0 0 18px 0;
      text-align: center;
      letter-spacing: 1px;
      font-weight: 500;
    }
    .hero {
      max-width: 600px;
      margin: 0 auto;
      padding: 28px 5vw 34px 5vw;
      text-align: center;
    }
    .hero-title {
      font-family: 'Cairo', sans-serif;
      font-size: 2rem;
      font-weight: 700;
      margin-bottom: 16px;
      background: linear-gradient(92deg, var(--gold1) 10%, var(--gold2) 60%, var(--gold1) 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      color: var(--gold1);
      text-shadow: 0 2px 10px #fff8;
      letter-spacing: 2px;
    }
    .hero-desc {
      font-size: 1.12rem;
      color: #3d3a36;
      line-height: 1.8;
      margin-bottom: 30px;
      font-family: 'Cairo', sans-serif;
    }
    .cta-btn {
      font-family: 'Montserrat', 'Cairo', sans-serif;
      font-size: 1.17rem;
      padding: 12px 36px;
      background: linear-gradient(90deg, var(--gold2) 10%, var(--gold1) 100%);
      color: var(--blue);
      border: none;
      border-radius: 28px;
      font-weight: 700;
      letter-spacing: 1px;
      box-shadow: 0 2px 8px 0 #bfa14c33;
      cursor: pointer;
      transition: background 0.2s, color 0.2s, box-shadow 0.2s;
      margin-bottom: 20px;
    }
    .cta-btn:hover {
      background: linear-gradient(90deg, var(--gold1) 10%, var(--gold2) 100%);
      color: #fff;
      box-shadow: 0 4px 14px 0 #bfa14c44;
    }
    /* Contact Section */
    .contact-section {
      background: #fff;
      border-radius: 18px;
      box-shadow: 0 2px 8px #bfa14c22;
      max-width: 400px;
      margin: 34px auto 0 auto;
      padding: 22px 10px 8px 10px;
      text-align: center;
      border: 1.5px solid #e4e6ea;
    }
    .contact-title {
      font-family: 'Cairo', sans-serif;
      font-size: 1.18rem;
      font-weight: 700;
      margin-bottom: 12px;
      background: linear-gradient(90deg, var(--gold1) 40%, var(--gold2) 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      color: var(--gold1);
    }
    .contact-icons {
      display: flex;
      justify-content: center;
      gap: 24px;
      margin-bottom: 10px;
      flex-wrap: wrap;
    }
    .contact-link {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      color: var(--blue);
      text-decoration: none;
      font-size: 1.05rem;
      font-family: 'Cairo', sans-serif;
      transition: color 0.18s;
      font-weight: 600;
    }
    .contact-link:hover {
      color: var(--gold1);
    }
    .contact-icon {
      width: 30px;
      height: 30px;
      fill: url(#gold-gradient);
      vertical-align: middle;
    }
    .contact-phone {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 6px;
      color: var(--blue);
      font-size: 1.08rem;
      font-weight: 600;
      direction: ltr;
      margin: 8px 0 0 0;
      font-family: 'Montserrat', 'Cairo', sans-serif;
    }
    .phone-icon {
      width: 23px;
      height: 23px;
      fill: url(#gold-gradient);
      vertical-align: middle;
    }
    .footer {
      text-align: center;
      color: #497bb1;
      font-size: 1rem;
      padding: 20px 0 10px 0;
      border-top: 1px solid #e0e8f0;
      background: #fafdff;
      margin-top: 36px;
    }
    @media (max-width: 600px) {
      .logo-svg {
        width: 48px;
        height: 48px;
      }
      .shop-name {
        font-size: 1.25rem;
      }
      .hero {
        padding: 17px 2vw 20px 2vw;
      }
      .hero-title {
        font-size: 1.18rem;
      }
      .subtitle {
        font-size: 1rem;
      }
      .contact-section {
        max-width: 95vw;
        padding: 10px 3vw 8px 3vw;
      }
      .footer {
        font-size: 0.94rem;
      }
    }
  </style>
</head>
<body>
  <header class="header">
    <div class="logo-box">
      <!-- Caftan Logo SVG - gold gradient -->
      <svg class="logo-svg" viewBox="0 0 64 64">
        <defs>
          <linearGradient id="gold-gradient" x1="0" y1="0" x2="1" y2="1">
            <stop offset="0%" stop-color="#f7e18b"></stop>
            <stop offset="65%" stop-color="#bfa14c"></stop>
            <stop offset="100%" stop-color="#e7cb7a"></stop>
          </linearGradient>
        </defs>
        <path d="M32 6
          Q36 14, 44 10
          L58 38
          Q52 40, 54 58
          Q47 62, 32 57
          Q17 62, 10 58
          Q12 40, 6 38
          L20 10
          Q28 14, 32 6
          Z" fill="url(#gold-gradient)" stroke="#bfa14c" stroke-width="2.2"></path>
        <circle cx="32" cy="16" r="1.3" fill="#fff"></circle>
        <circle cx="32" cy="22" r="1.3" fill="#fff"></circle>
        <circle cx="32" cy="28" r="1.3" fill="#fff"></circle>
      </svg>
      <span class="shop-name">Maison Cesar Caftan</span>
    </div>
    <div class="subtitle">دار القيصر للقفطان</div>
  </header>
  
  <main class="hero">
    <div class="hero-title">تألق مع أجمل القفاطين الاصلية الفاخرة</div>
    <div class="hero-desc">
      اكتشفي تشكيلتنا الراقية من القفاطين بجودة عالية وتصاميم عصرية بلمسة ذهبية.<br>
      <b>Maison Cesar Caftan</b>، عنوان الأناقة والرقي.<br>
      <br>
      <span style="color:#4176c5;font-family:'Montserrat',sans-serif;">Explore our luxurious caftans with gold details and modern style.<br>Elegance for every occasion.</span>
    </div>
    <a href="https://wa.me/213699947881" class="cta-btn">تواصلي معنا عبر واتساب</a>
  </main>

  <!-- Contact Section -->
  <section class="contact-section">
    <div class="contact-title">معلومات التواصل</div>
    <div class="contact-icons">
      <a class="contact-link" href="https://www.instagram.com/maison_cesar_cafton/" target="_blank" title="Instagram">
        <!-- Instagram Icon SVG -->
        <svg class="contact-icon" viewBox="0 0 32 32">
          <defs>
            <linearGradient id="ig-gold" x1="0" y1="0" x2="1" y2="1">
              <stop offset="0%" stop-color="#f7e18b"></stop>
              <stop offset="70%" stop-color="#bfa14c"></stop>
            </linearGradient>
          </defs>
          <rect x="3" y="3" width="26" height="26" rx="7" fill="none" stroke="url(#ig-gold)" stroke-width="2"></rect>
          <circle cx="16" cy="16" r="6" fill="none" stroke="url(#ig-gold)" stroke-width="2"></circle>
          <circle cx="23.5" cy="8.5" r="1.2" fill="url(#ig-gold)"></circle>
        </svg>
        Instagram
      </a>
      <a class="contact-link" href="https://www.facebook.com/share/1KzRWNRN6g/?mibextid=wwXIfr" target="_blank" title="Facebook">
        <!-- Facebook Icon SVG -->
        <svg class="contact-icon" viewBox="0 0 32 32">
          <defs>
            <linearGradient id="fb-gold" x1="0" y1="0" x2="1" y2="1">
              <stop offset="0%" stop-color="#f7e18b"></stop>
              <stop offset="70%" stop-color="#bfa14c"></stop>
            </linearGradient>
          </defs>
          <circle cx="16" cy="16" r="13" fill="none" stroke="url(#fb-gold)" stroke-width="2"></circle>
          <path d="M18 16h2.2l.4-2.6H18V12.6c0-.7.2-1.1 1.2-1.1h1V9.2c-.2 0-.9-.1-1.8-.1-1.8 0-3 1-3 2.9v1.4H12v2.6h2.4V22h3v-6z" fill="url(#fb-gold)"></path>
        </svg>
        Facebook
      </a>
    </div>
    <div class="contact-phone">
      <!-- Phone Icon SVG -->
      <svg class="phone-icon" viewBox="0 0 24 24">
        <defs>
          <linearGradient id="phone-gold" x1="0" y1="0" x2="1" y2="1">
            <stop offset="0%" stop-color="#f7e18b"></stop>
            <stop offset="100%" stop-color="#bfa14c"></stop>
          </linearGradient>
        </defs>
        <path d="M6.6,10.8c1.6,3.2,4,5.6,7.2,7.2l1.6-1.6c0.3-0.3,0.7-0.4,1.1-0.3c1.2,0.4,2.5,0.6,3.8,0.6
          c0.6,0,1,0.4,1,1V21c0,0.6-0.4,1-1,1C11.1,22,2,12.9,2,2c0-0.6,0.4-1,1-1h3.5c0.6,0,1,0.4,1,1c0,1.3,0.2,2.6,0.6,3.8
          c0.1,0.4,0,0.8-0.3,1.1L6.6,10.8z" fill="url(#phone-gold)"></path>
      </svg>
      +213 699 94 78 81
    </div>
  </section>

  <footer class="footer">
    © 2025 Maison Cesar Caftan. جميع الحقوق محفوظة.<br>
    Designed with <span style="color: #bfa14c; font-size:1.1em;">❤</span> for algerian elegance.
  </footer>


</body></html>
