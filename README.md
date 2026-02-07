<!DOCTYPE html>
<html lang="cs">
<head>
<meta charset="UTF-8" />
<title>Developerský projekt – Úvod</title>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<style>
* { box-sizing: border-box; margin: 0; padding: 0; font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif; }
body { color: #222; background-color: white; } /* bílé pozadí */

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
  font-size: 36px;
  text-transform: uppercase;
  color: pink; /* růžový nápis */
}

.logo span { color: pink; }

.nav-links {
  display: flex;
  gap: 24px;
  font-size: 14px;
}

.nav-links a {
  text-decoration: none;
  color: #2f2f2f; /* antracitová barva */
  font-weight: 500;
}

.nav-links a:hover {
  color: #555; /* jemný hover */
}

.hero {
  background: linear-gradient(135deg, lightgreen 0%, lightgreen 50%, white 50%);
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

.hero-card {
  background: #f0f0f0; /* světle šedý box */
  color: #111;
  border-radius: 50%;
  width: 280px;
  height: 280px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  box-shadow: 0 18px 40px rgba(0,0,0,0.18);
  text-align: center;
  margin: auto;
}

.hero-card-label { font-size: 11px; text-transform: uppercase; letter-spacing: 0.16em; color: #888; margin-bottom: 10px; }
.hero-card-main { font-size: 20px; font-weight: 700; margin-bottom: 6px; }
.hero-card-sub { font-size: 13px; color: #666; margin-bottom: 14px; }
.hero-card-grid { font-size: 12px; color: #555; }

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
  background: linear-gradient(135deg, lightgreen, #a8e6a1);
  height: 160px;
}

.project-body { padding: 16px 18px; flex: 1; display: flex; flex-direction: column; gap: 8px; }
.project-location { font-size: 11px; text-transform: uppercase; letter-spacing: 0.16em; color: #888; }
.project-title { font-size: 16px; font-weight: 600; }
.project-meta { font-size: 13px; color: #666; }
.project-price { font-size: 14px; font-weight: 600; margin-top: 4px; }
.project-footer { padding: 0 18px 16px; display: flex; justify-content: space-between; font-size: 12px; color: #777; }
.badge { padding: 3px 9px; border-radius: 999px; background: #e6f2ff; color: #005da4; font-size: 11px; font-weight: 600; text-transform: uppercase; letter-spacing: 0.12em; }

.contact { margin-top: 50px; padding: 26px 22px; border-radius: 18px; background: #0b2347; color: #fff; display: flex; flex-wrap: wrap; gap: 18px; justify-content: space-between; }
footer { padding: 24px 20px 30px; font-size: 12px; color: #777; text-align: center; }
</style>
</head>
<body>

<header>
  <div class="nav">
    <div class="logo"><span>NEMOVEX</span> Group</div>
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
      <p class="hero-subtitle">Vyberte si z nabídky nových bytů a rodinných domů v nejžádanějších lokalitách. Kvalitní standard, promyšlené dispozice a důraz na detail.</p>
    </div>
    <aside class="hero-card">
      <div class="hero-card-label">Aktuálně v nabídce</div>
      <div class="hero-card-main">Praha – Zelené Město</div>
      <div class="hero-card-sub">Nová etapa moderního bydlení v dosahu centra.</div>
      <div class="hero-card-grid">
        <div>Dispozice: 1+kk – 4+kk</div>
        <div>Cena od: 4 890 000 Kč</div>
        <div>Dostupnost: Q4 2026</div>
        <div>Metro: do 8 minut MHD</div>
      </div>
    </aside>
  </div>
</section>

<main>
  <section id="projekty">
    <div class="section-header">
      <h2>Vybrané projekty</h2>
      <p>Prohlédněte si několik aktuálních projektů. Všechny nabízejí kvalitní standard, dobrou dopravní dostupnost a občanskou vybavenost.</p>
    </div>

    <div class="projects-grid">
      <!-- původní tři projekty -->
      <article class="project-card"><div class="project-image"></div><div class="project-body"><div class="project-location">Praha 9 – Vysočany</div><div class="project-title">Rezidence Park Vysočany</div><div class="project-meta">Byty 1+kk až 4+kk s výhledem do zeleně.</div><div class="project-price">Ceny od 4,6 mil. Kč</div></div><div class="project-footer"><span>Dokončení 2027</span><span class="badge">Novinka</span></div></article>
      <article class="project-card"><div class="project-image"></div><div class="project-body"><div class="project-location">Praha-západ</div><div class="project-title">Rodinné domy Javorová čtvrť</div><div class="project-meta">Moderní domy s vlastní zahradou v klidné lokalitě.</div><div class="project-price">Ceny od 12,9 mil. Kč</div></div><div class="project-footer"><span>Dokončení 2026</span><span class="badge">Domy</span></div></article>
      <article class="project-card"><div class="project-image"></div><div class="project-body"><div class="project-location">Praha 5 – Smíchov</div><div class="project-title">City Living Smíchov</div><div class="project-meta">Městské bydlení v docházkové vzdálenosti centra
