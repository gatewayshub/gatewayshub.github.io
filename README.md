<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<title>Startseite</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
:root {
  --bg:#0e1117; --fg:#e6e6e6; --card:#161b22;
  --card-hover:#1f2937; --accent:#1f6feb; --muted:#9aa0a6;
}
body.light {
  --bg:#f3f4f6; --fg:#1f2937; --card:#ffffff;
  --card-hover:#e5e7eb; --accent:#2563eb; --muted:#555;
}
body {
  margin:0;
  font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;
  background:var(--bg);
  color:var(--fg);
}
header {
  text-align:center;
  padding:0.8rem;
  position:relative;
}
.theme-toggle {
  position:absolute; top:0.45rem; right:0.45rem;
  background:var(--card); border:none; color:var(--fg);
  padding:0.25rem 0.45rem; border-radius:5px; cursor:pointer;
  font-size:0.8rem;
}
.search-box form {
  max-width:480px; margin:0 auto;
  display:flex; gap:0.35rem;
}
.search-box input {
  flex:1; padding:0.45rem 0.6rem;
  font-size:0.9rem; border-radius:6px;
  border:none; outline:none;
}
.search-box button {
  padding:0.45rem 0.8rem;
  font-size:0.9rem; border-radius:6px;
  border:none; cursor:pointer;
  background:var(--accent); color:white;
}
main {
  max-width:1300px;
  margin:0 auto;
  padding:0.6rem 0.8rem 1.5rem;
}
section { margin-bottom:1.2rem; }
section h2 {
  font-size:0.95rem;
  margin-bottom:0.35rem;
  border-bottom:1px solid var(--card-hover);
  padding-bottom:0.15rem;
}
.tiles {
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(145px,1fr));
  gap:0.45rem;
}
.tile {
  background:var(--card);
  padding:0.4rem 0.5rem;
  border-radius:6px;
  text-decoration:none;
  color:inherit;
  box-shadow:0 1px 3px rgba(0,0,0,0.25);
  transition:background 0.12s ease, transform 0.12s ease;
}
.tile:hover {
  background:var(--card-hover);
  transform:translateY(-1px);
}
.tile-header {
  display:flex;
  align-items:center;
  gap:0.35rem;
}
.tile-icon {
  width:16px;
  height:16px;
  border-radius:3px;
}
.tile h3 {
  margin:0;
  font-size:0.78rem;
  font-weight:600;
}
.tile p {
  margin-left:1.45rem;
  margin-top:0.05rem;
  font-size:0.62rem;
  color:var(--muted);
}
</style>
</head>

<body>

<header>
<button class="theme-toggle" onclick="toggleTheme()">🌙 / ☀️</button>
<div class="search-box">
<form action="https://www.google.com/search" method="get">
<input type="text" name="q" placeholder="Google Suche …" autofocus>
<button type="submit">🔍</button>
</form>
</div>
</header>

<main>

<section>
<h2>⚡ Schnellnavigation</h2>
<div class="tiles">
<a class="tile" href="https://youtube.com" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=youtube.com&sz=32"><h3>YouTube</h3></div><p>Videos</p></a>
<a class="tile" href="https://chat.openai.com" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=openai.com&sz=32"><h3>ChatGPT</h3></div><p>AI Assistant</p></a>
<a class="tile" href="https://www.amazon.de" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=amazon.de&sz=32"><h3>Amazon</h3></div><p>Shopping</p></a>
<a class="tile" href="https://www.krone.at" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=krone.at&sz=32"><h3>Kronen Zeitung</h3></div><p>News</p></a>
<a class="tile" href="https://www.derstandard.at" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=derstandard.at&sz=32"><h3>Der Standard</h3></div><p>Nachrichten</p></a>
<a class="tile" href="https://www.facebook.com" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=facebook.com&sz=32"><h3>Facebook</h3></div><p>Social</p></a>
<a class="tile" href="https://web.telegram.org" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=telegram.org&sz=32"><h3>Telegram</h3></div><p>Messenger</p></a>
<a class="tile" href="https://web.whatsapp.com" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=whatsapp.com&sz=32"><h3>WhatsApp</h3></div><p>Web</p></a>
</div>
</section>

<section>
<h2>💬 Foren</h2>
<div class="tiles">
<a class="tile" href="https://www.astronomieforum.at" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=astronomieforum.at&sz=32"><h3>astronomieforum.at</h3></div><p>AT</p></a>
<a class="tile" href="https://forum.astronomie.de" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=astronomie.de&sz=32"><h3>astronomie.de</h3></div><p>DE</p></a>
<a class="tile" href="https://www.astrotreff.de" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=astrotreff.de&sz=32"><h3>Astrotreff</h3></div><p>Community</p></a>
<a class="tile" href="https://www.cloudynights.com" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=cloudynights.com&sz=32"><h3>Cloudy Nights</h3></div><p>Int.</p></a>
<a class="tile" href="https://stargazerslounge.com" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=stargazerslounge.com&sz=32"><h3>Stargazers Lounge</h3></div><p>UK</p></a>
</div>
</section>

<section>
<h2>🏛 Institutionen</h2>
<div class="tiles">
<a class="tile" href="http://www.esa.int/esaCP/Germany.html" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=esa.int&sz=32"><h3>ESA</h3></div><p>Europa</p></a>
<a class="tile" href="http://www.eso.org/public/outreach/press-rel/" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=eso.org&sz=32"><h3>ESO</h3></div><p>Observatorium</p></a>
<a class="tile" href="http://www.jpl.nasa.gov/" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=jpl.nasa.gov&sz=32"><h3>JPL</h3></div><p>NASA Lab</p></a>
<a class="tile" href="https://hubblesite.org/home" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=hubblesite.org&sz=32"><h3>Hubble</h3></div><p>HST</p></a>
<a class="tile" href="http://www.nasa.gov/home/index.html" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=nasa.gov&sz=32"><h3>NASA</h3></div><p>Agency</p></a>
<a class="tile" href="https://webb.nasa.gov/" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=webb.nasa.gov&sz=32"><h3>JWST</h3></div><p>Webb Telescope</p></a>
<a class="tile" href="https://soho.nascom.nasa.gov/data/realtime/realtime-update.html" target="_blank" rel="noopener noreferrer"><div class="tile-header"><img loading="lazy" class="tile-icon" src="https://www.google.com/s2/favicons?domain=soho.nascom.nasa.gov&sz=32"><h3>SOHO</h3></div><p>Solar Observatory</p></a>
</div>
</section>

</main>

<script>
function toggleTheme(){
  document.body.classList.toggle('light');
  localStorage.setItem(
    'theme',
    document.body.classList.contains('light') ? 'light' : 'dark'
  );
}
if(localStorage.getItem('theme') === 'light'){
  document.body.classList.add('light');
}
</script>

</body>
</html>
