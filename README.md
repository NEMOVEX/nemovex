<!DOCTYPE html>
<html lang="cs">
<head>
<meta charset="UTF-8" />
<title>NEMOVEX Group – Developerské projekty</title>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<style>
body {
  margin: 0;
  font-family: system-ui, sans-serif;
  background-color: white;
  color: #2f2f2f;
}

header {
  background: #fff;
  border-bottom: 1px solid #ddd;
  padding: 14px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 36px;
  font-weight: 800;
  text-transform: uppercase;
}

.nav-links {
  display: flex;
  gap: 24px;
}

.nav-links a {
  text-decoration: none;
  color: #2f2f2f;
  font-weight: 500;
}

.nav-links a:hover {
  color: #000;
}

.btn-primary {
  padding: 8px 18px;
  border-radius: 999px;
  border: none;
  background: #2f2f2f;
  color: #fff;
  font-weight: 600;
  cursor: pointer;
}

.hero {
  position: relative;
  height: 500px;
  background: url('https://copilot.microsoft.com/th/id/BCO.e579fb29-d8fc-45d0-94fb-61222e622c61.png') no-repeat center center/cover;
}

.hero-text {
  position: absolute;
  bottom: 30px;
  left: 30px;
  background-color: rgba(0,0,0,0.4);
  padding: 20px 30px;
  border-radius: 12px;
}

.hero-text h2 {
  color: white;
  font-size: 24px;
  margin-bottom: 8px;
}

.hero-text p {
  color: white;
  font-size: 16px;
}

main {
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
}

.section-header h2 {
  font-size: 22px;
  margin-bottom: 10px;
}

.section-header p {
  font-size: 14px;
  color: #555;
  margin-bottom: 30px;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 20px;
}

.project-card {
  background: #f0f0f0;
  border-radius: 16px;
  padding: 20px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.06);
}

.project-title {
  font-size: 16px;
  font-weight: 600;
  margin-bottom: 6px;
}

.project-meta {
  font-size: 13px;
  color: #666;
}

footer {
  text-align: center;
  font-size: 12px;
  color: #777;
  padding: 30px 20px;
}
</style>
</head>
<body>

<header>
  <div class="logo"><span>NEMOVEX</span> Group</div>
  <nav class="nav-links">
    <a href="#projekty">Projekty</a>
    <a href="#lokality">Lokality</a>
    <a href="#kontakt">Kontakt</a>
  </nav>
  <button class="btn-primary">Chci bydlet</button>
</header>

<section class="hero">
  <div class="hero-text">
    <h2>Klenovka</h2>
    <p>Dům 5+kk &nbsp; | &nbsp; Cena: 10 000 000 Kč</p>
  </div>
</section>

<main>
  <section id="projekty">
    <div class="section-header">
      <h2>Přehled projektů v nabídce</h2>
      <p>Prohlédněte si aktuální projekty dostupné v našem portfoliu.</p>
    </div>

    <div class="projects-grid">
      <div class="project-card">
        <div class="project-title">Rezidence Chrudim</div>
        <div class="project-meta">Byty 2+kk – 4+kk &nbsp; | &nbsp; Cena od 5 500 000 Kč</div>
      </div>
      <div class="project-card">
        <div class="project-title">Klenovka</div>
        <div class="project-meta">Rodinné domy 5+kk &nbsp; | &nbsp; Cena od 10 000 000 Kč</div>
      </div>
      <div class="project-card">
        <div class="project-title">Voleč</div>
        <div class="project-meta">Domy 3+kk – 5+kk &nbsp; | &nbsp; Cena od 7 800 000 Kč</div>
      </div>
      <div class="project-card">
        <div class="project-title">Kutná Hora</div>
        <div class="project-meta">Byty 1+kk – 3+kk &nbsp; | &nbsp; Cena od 4 200 000 Kč</div>
      </div>
    </div>
  </section>
</main>

<footer>
  © 2026 NEMOVEX Group a.s. | Přehled developerských projektů.
</footer>

</body>
</html>
