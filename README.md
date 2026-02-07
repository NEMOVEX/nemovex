<!DOCTYPE html>
<html lang="cs">
<head>
  <meta charset="UTF-8" />
  <title>Developerský projekt – Úvod</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif; }

    body { color: #222; background-color: #f5f5f5; }

    header {
      position: sticky;
      top: 0;
      z-index: 10;
      background: #ffffffee;
      backdrop-filter: blur(8px);
      border-bottom: 1px solid #e0e0e0;
    }

    .nav {
      max-width: 1200px;
      margin: 0 auto;
      padding: 14px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-weight: 800;
      letter-spacing: 0.08em;
      font-size: 18px;
      text-transform: uppercase;
    }

    .logo span {
      color: #0070c9;
    }

    .nav-links {
      display: flex;
      gap: 24px;
      font-size: 14px;
    }

    .nav-links a {
      text-decoration: none;
      color: #333;
      font-weight: 500;
    }

    .nav-links a:hover {
      color: #0070c9;
    }

    .btn-primary {
      padding: 8px 18px;
      border-radius: 999px;
      border: none;
      background: #0070c9;
      color: #fff;
      font-size: 14px;
      font-weight: 600;
      cursor: pointer;
    }

    .btn-primary:hover {
      background: #005da4;
    }

    .hero {
      background: linear-gradient(135deg, #0b2347 0%, #174f8a 50%, #f5f5f5 50%);
      color: #fff;
    }

    .hero-inner {
      max-width: 1200px;
      margin: 0 auto;
      padding: 80px 20px 90px;
      display: grid;
      grid-template-columns: minmax(0, 1.2fr) minmax(0, 1fr);
      gap: 40px;
      align-items: center;
    }

    .hero-kicker {
      text-transform: uppercase;
      letter-spacing: 0.18em;
      font-size: 11px;
      opacity: 0.8;
      margin-bottom: 10px;
    }

    .hero-title {
      font-size: clamp(32px, 4vw, 44px);
      line-height: 1.1;
      margin-bottom: 18px;
      max-width: 18ch;
    }

    .hero-subtitle {
      font-size: 15px;
      line-height: 1.6;
      opacity: 0.9;
      max-width: 40ch;
      margin-bottom: 26px;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      align-items: center;
    }

    .btn-secondary {
      padding: 8px 18px;
      border-radius: 999px;
      border: 1px solid #ffffff55;
      background: transparent;
      color: #fff;
      font-size: 14px;
      font-weight: 500;
      cursor: pointer;
    }

    .btn-secondary:hover {
      background: #ffffff11;
    }

    .hero-meta {
      margin-top: 18px;
      font-size: 12px;
      opacity: 0.8;
      display: flex;
      flex-wrap: wrap;
      gap: 16px;
    }

    .hero-card {
      background: #fff;
      color: #111;
      border-radius: 18px;
      padding: 22px 22px 20px;
      box-shadow: 0 18px 40px rgba(0,0,0,0.18);
    }

    .hero-card-label {
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      color: #888;
      margin-bottom: 10px;
    }

    .hero-card-main {
      font-size: 22px;
      font-weight: 700;
      margin-bottom: 6px;
    }

    .hero-card-sub {
      font-size: 13px;
      color: #666;
      margin-bottom: 14px;
    }

    .hero-card-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 10px 18px;
      font-size: 12px;
    }

    .hero-card-grid span:first-child {
      color: #777;
    }

    main {
      max-width: 1200px;
      margin: 0 auto;
      padding: 40px 20px 60px;
    }

    .section-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      margin-bottom: 22px;
      gap: 16px;
    }

    .section-header h2 {
      font-size: 22px;
    }

    .section-header p {
      font-size: 13px;
      color: #666;
      max-width: 40ch;
    }

    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 20px;
    }

    .project-card {
      background: #fff;
      border-radius: 16px;
      overflow: hidden;
      box-shadow: 0 8px 20px rgba(0,0,0,0.06);
      display: flex;
      flex-direction: column;
    }

    .project-image {
      background: linear-gradient(135deg, #174f8a, #00a0b0);
      height: 160px;
      position: relative;
      overflow: hidden;
    }

    .project-image::after {
      content: "";
      position: absolute;
      inset: 18% 10%;
      border-radius: 18px;
      border: 1px solid rgba(255,255,255,0.35);
      opacity: 0.7;
    }

    .project-body {
      padding: 16px 18px 16px;
      flex: 1;
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .project-location {
      font-size: 11px;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      color: #888;
    }

    .project-title {
      font-size: 16px;
      font-weight: 600;
    }

    .project-meta {
      font-size: 13px;
      color: #666;
    }

    .project-price {
      font-size: 14px;
      font-weight: 600;
      margin-top: 4px;
    }

    .project-footer {
      padding: 0 18px 16px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 12px;
      color: #777;
    }

    .badge {
      padding: 3px 9px;
      border-radius: 999px;
      background: #e6f2ff;
      color: #005da4;
      font-size: 11px;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.12em;
    }

    .contact {
      margin-top: 50px;
      padding: 26px 22px;
      border-radius: 18px;
      background: #0b2347;
      color: #fff;
      display: flex;
      flex-wrap: wrap;
      gap: 18px;
      align-items: center;
      justify-content: space-between;
    }

    .contact h3 {
      font-size: 18px;
      margin-bottom: 6px;
    }

    .contact p {
      font-size: 13px;
      opacity: 0.9;
      max-width: 40ch;
    }

    .contact-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .contact .btn-secondary {
      border-color: #ffffff55;
    }

    footer {
      padding: 24px 20px 30px;
      font-size: 12px;
      color: #777;
      text-align: center;
    }

    @media (max-width: 800px) {
      .hero-inner {
        grid-template-columns: minmax(0, 1fr);
        padding-top: 60px;
      }
      .hero {
        background: linear-gradient(150deg, #0b2347 0%, #174f8a 60%, #f5f5f5 60%);
      }
      .nav-links {
        display: none;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="nav">
      <div class="logo"><span>DEVELOP</span>CITY</div>
      <nav class="nav-links">
        <a href="#projekty">Projekty</a>
        <a href="#lokality">Lokality</a>
        <a href="#kontakt">Kontakt</a>
      </nav>
      <button class="btn-primary">Chci bydlet</button>
    </div>
  </header>

  <section class="hero">
    <div class="hero-inner">
      <div>
        <div class="hero-kicker">Nové bydlení v Praze a okolí</div>
        <h1 class="hero-title">Moderní byty a domy pro skutečný život.</h1>
        <p class="hero-subtitle">
          Vyberte si z nabídky nových bytů a rodinných domů v nejžádanějších lokalitách.
          Kvalitní standard, promyšlené dispozice a důraz na detail.
        </p>
        <div class="hero-actions">
          <button class="btn-primary">Zobrazit všechny projekty</button>
          <button class="btn-secondary">Najít byt podle parametrů</button>
        </div>
        <div class="hero-meta">
          <span>Více než 2 000 prodaných bytů</span>
          <span>15 let zkušeností s výstavbou</span>
        </div>
      </div>
      <aside class="hero-card">
        <div class="hero-card-label">Aktuálně v nabídce</div>
        <div class="hero-card-main">Praha – Zelené Město</div>
        <div class="hero-card-sub">Nová etapa moderního bydlení v dosahu centra.</div>
        <div class="hero-card-grid">
          <span>Dispozice</span><span>1+kk – 4+kk</span>
          <span>Cena od</span><span>4 890 000 Kč</span>
          <span>Dostupnost</span><span>Q4 2026</span>
          <span>Metro</span><span>do 8 minut MHD</span>
        </div>
      </aside>
    </div>
  </section>

  <main>
    <section id="projekty">
      <div class="section-header">
        <div>
          <h2>Vybrané projekty</h2>
        </div>
        <p>
          Prohlédněte si několik aktuálních projektů. Všechny nabízejí kvalitní standard,
          dobrou dopravní dostupnost a občanskou vybavenost.
        </p>
      </div>

      <div class="projects-grid">
        <article class="project-card">
          <div class="project-image"></div>
          <div class="project-body">
            <div class="project-location">Praha 9 – Vysočany</div>
            <div class="project-title">Rezidence Park Vysočany</div>
            <div class="project-meta">Byty 1+kk až 4+kk s výhledem do zeleně.</div>
            <div class="project-price">Ceny od 4,6 mil. Kč</div>
          </div>
          <div class="project-footer">
            <span>Dokončení 2027</span>
            <span class="badge">Novinka</span>
          </div>
        </article>

        <article class="project-card">
          <div class="project-image"></div>
          <div class="project-body">
            <div class="project-location">Praha-západ</div>
            <div class="project-title">Rodinné domy Javorová čtvrť</div>
            <div class="project-meta">Moderní domy s vlastní zahradou v klidné lokalitě.</div>
            <div class="project-price">Ceny od 12,9 mil. Kč</div>
          </div>
          <div class="project-footer">
            <span>Dokončení 2026</span>
            <span class="badge">Domy</span>
          </div>
        </article>

        <article class="project-card">
          <div class="project-image"></div>
          <div class="project-body">
            <div class="project-location">Praha 5 – Smíchov</div>
            <div class="project-title">City Living Smíchov</div>
            <div class="project-meta">Městské bydlení v docházkové vzdálenosti centra.</div>
            <div class="project-price">Ceny od 6,9 mil. Kč</div>
          </div>
          <div class="project-footer">
            <span>Dokončení 2028</span>
            <span class="badge">Město</span>
          </div>
        </article>
      </div>
    </section>

    <section id="kontakt" class="contact">
      <div>
        <h3>Máte zájem o nezávaznou schůzku?</h3>
        <p>
          Nechte nám na sebe kontakt a společně vybereme projekt i konkrétní byt,
          který vám bude dávat smysl.
        </p>
      </div>
      <div class="contact-actions">
        <button class="btn-primary">Chci být kontaktován</button>
        <button class="btn-secondary">Zobrazit kontakty</button>
      </div>
    </section>
  </main>

  <footer>
    © 2026 DevelopCity a.s. | Vzorová úvodní stránka inspirovaná stylem velkých developerů.
  </footer>
</body>
</html>
