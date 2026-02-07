<!DOCTYPE html>
<html lang="cs">
<head>
<meta charset="UTF-8" />
<title>Developerský projekt – Úvod</title>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<style>
* { box-sizing: border-box; margin: 0; padding: 0; font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif; }
body { color: #222; background-color: white; }

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
  color: #2f2f2f; /* antracitové logo */
}

.logo span { color: #2f2f2f; }

.nav-links {
  display: flex;
  gap: 24px;
  font-size: 14px;
}

.nav-links a {
  text-decoration: none;
  color: #2f2f2f; /* antracitové odkazy */
  font-weight: 500;
}

.nav-links a:hover { color: #000; }

.btn-primary {
  padding: 8px 18px;
  border-radius: 999px;
  border: none;
  background: #2f2f2f;
  color: #fff;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
}

.btn-primary:hover { background: #000; }

.btn-secondary {
  padding: 8px 18px;
  border-radius: 999px;
  border: 1px solid #2f2f2f;
  background: transparent;
  color: #2f2f2f;
  font-size: 14px;
  font-weight: 500;
  cursor: pointer;
}

.btn-secondary:hover { background: #f0f0f0; }

.hero {
  background: url('https://copilot.microsoft.com/th/id/BCO.e579fb29-d8fc-45d0-94fb-61222e622c61.png') no-repeat center center/cover;
  color: #000;
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

.section-header h2 {
  font-size: 22px;
  color: #2f2f2f;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 20px;
}

.project-card {
  background: #f0f0f0; /* šedé boxy */
  border-radius: 16px;
  overflow: hidden;
  box-shadow: 0 8px 20px rgba(0,0,0,0.06);
  display: flex;
  flex-direction: column;
}

.project-body { padding: 16px 18px; flex: 1; display: flex; flex-direction: column; gap: 8px; }
.project-title { font-size: 16px; font-weight: 600; color: #2f2f2f; }
.project-meta { font-size: 13px; color: #666; }
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
      <div class="hero-kicker">Nové bydlení v Chrudimi a okolí</div>
      <h1 class="hero-title">Moderní byty a domy pro skutečný život.</h1>
      <p class="hero-subtitle">Vyberte si z nabídky nových bytů a rodinných domů v nejžádanějších lokalitách. Kvalitní standard, promyšlené dispozice a důraz na detail.</p>
    </div>
    <aside class="hero-card">
      <div class="hero-card-label">Aktuálně v nabídce</div>
      <div class="hero-card-main">Klenovka</div>
      <div class="hero-card-sub">Dům 5+kk</div>
      <div class="hero-card-grid">
        <div>Cena: 10 000 000 Kč</div>
      </div>
    </aside>
  </div>
</section>

<main>
  <section id="projekty">
    <div class="section-header">
      <h2>Přehled projektů v nabídce</h2>
      <p>Prohlédněte si aktuální projekty dostupné v našem portfoliu.</p>
    </div>

    <div class="projects-grid">
      <article class="project-card">
        <div class="project-body">
          <div class="project-title">Rezidence Chrudim</div>
          <div class="project-meta">Moderní byty v centru Chrudimi.</div>
        </div>
      </article>

      <article class="project-card">
        <div class="project-body">
          <div class="project-title">Klenovka</div>
          <div class="project-meta">
