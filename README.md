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

.hero-card {
  position: absolute;
  bottom: 30px;
  right: 30px;
  background: #f0f0f0;
  color: #111;
  border-radius: 50%;
  width: 220px;
  height: 220px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  box-shadow: 0 12px 30px rgba(0,0,0,0.18);
  text-align: center;
}

.hero-card-label {
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: 0.16em;
  color: #555;
  margin-bottom: 8px;
}

.hero-card-main {
  font-size: 18px;
  font-weight: 700;
  margin-bottom: 6px;
}

.hero-card-sub {
  font-size: 13px;
  color: #666;
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
  <div class="hero-card">
    <div class="hero-card-label">Aktuálně v nabídce</div>
    <div class="hero-card-main">Klenovka</div>
    <div class="hero-card-sub">Dům 5+kk<br>Cena: 10 000 000 Kč</div>
  </div>
</section>

</body>
</html>
