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
<a class="tile" href="https://youtube.com" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=youtube.com&sz=32"><h3>Youtube</h3></div><p>Videos</p></a>
<a class="tile" href="https://chat.openai.com" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=openai.com&sz=32"><h3>ChatGPT</h3></div><p>AI Assistant</p></a>
<a class="tile" href="https://www.amazon.de" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=amazon.de&sz=32"><h3>Amazon</h3></div><p>Shopping</p></a>
<a class="tile" href="https://www.krone.at" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=krone.at&sz=32"><h3>Kronen Zeitung</h3></div><p>News</p></a>
<a class="tile" href="https://www.derstandard.at" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=derstandard.at&sz=32"><h3>Der Standard</h3></div><p>Nachrichten</p></a>
<a class="tile" href="https://www.facebook.com" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=facebook.com&sz=32"><h3>Facebook</h3></div><p>Social</p></a>
<a class="tile" href="https://web.telegram.org" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=telegram.org&sz=32"><h3>Telegram</h3></div><p>Messenger</p></a>
<a class="tile" href="https://web.whatsapp.com" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=whatsapp.com&sz=32"><h3>WhatsApp</h3></div><p>Web</p></a>
</div>
</section>

<section>
<h2>💬 Foren</h2>
<div class="tiles">
<a class="tile" href="https://www.astronomieforum.at" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=astronomieforum.at&sz=32"><h3>astronomieforum.at</h3></div><p>AT</p></a>
<a class="tile" href="https://forum.astronomie.de" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=astronomie.de&sz=32"><h3>astronomie.de</h3></div><p>DE</p></a>
<a class="tile" href="https://www.astrotreff.de" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=astrotreff.de&sz=32"><h3>Astrotreff</h3></div><p>Community</p></a>
<a class="tile" href="https://www.cloudynights.com" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=cloudynights.com&sz=32"><h3>Cloudy Nights</h3></div><p>Int.</p></a>
<a class="tile" href="https://stargazerslounge.com" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=stargazerslounge.com&sz=32"><h3>Stargazers Lounge</h3></div><p>UK</p></a>
</div>
</section>

<section>
<h2>📰 News</h2>
<div class="tiles">
<a class="tile" href="https://esahubble.org" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=esahubble.org&sz=32"><h3>ESA Hubble</h3></div><p>Weltraum</p></a>
<a class="tile" href="https://www.starobserver.org" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=starobserver.org&sz=32"><h3>Star Observer</h3></div><p>APOD</p></a>
<a class="tile" href="https://www.astronomy.com/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=astronomy.com&sz=32"><h3>Astronomy</h3></div><p>Magazin</p></a>
<a class="tile" href="https://skyandtelescope.org/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=skyandtelescope.org&sz=32"><h3>Sky & Telescope</h3></div><p>Beobachtung</p></a>
<a class="tile" href="https://www.scinexx.de/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=scinexx.de&sz=32"><h3>scinexx</h3></div><p>Wissenschaft</p></a>
<a class="tile" href="https://www.nationalgeographic.de/wissenschaft" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=nationalgeographic.de&sz=32"><h3>NatGeo</h3></div><p>Wissenschaft</p></a>
<a class="tile" href="https://www.astronews.com/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=astronews.com&sz=32"><h3>astronews</h3></div><p>DE News</p></a>
<a class="tile" href="https://www.raumfahrer.net/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=raumfahrer.net&sz=32"><h3>Raumfahrer.net</h3></div><p>Raumfahrt</p></a>
</div>
</section>

<section>
<h2>🏛 Institutionen</h2>
<div class="tiles">
<a class="tile" href="http://www.esa.int/esaCP/Germany.html" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=esa.int&sz=32"><h3>ESA</h3></div><p>Europa</p></a>
<a class="tile" href="http://www.eso.org/public/outreach/press-rel/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=eso.org&sz=32"><h3>ESO</h3></div><p>Press</p></a>
<a class="tile" href="http://www.jpl.nasa.gov/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=jpl.nasa.gov&sz=32"><h3>JPL</h3></div><p>NASA</p></a>
<a class="tile" href="https://hubblesite.org/home" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=hubblesite.org&sz=32"><h3>HubbleSite</h3></div><p>HST</p></a>
<a class="tile" href="http://www.nasa.gov/home/index.html" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=nasa.gov&sz=32"><h3>NASA</h3></div><p>Home</p></a>
<a class="tile" href="https://webb.nasa.gov/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=webb.nasa.gov&sz=32"><h3>JWST</h3></div><p>Webb</p></a>
<a class="tile" href="https://soho.nascom.nasa.gov/data/realtime/realtime-update.html" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=soho.nascom.nasa.gov&sz=32"><h3>SOHO</h3></div><p>Soho</p></a>
</div>
</section>

<section>
<h2>ℹ️ Infosites</h2>
<div class="tiles">
<a class="tile" href="https://www.freunde-der-nacht.net" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=freunde-der-nacht.net&sz=32"><h3>Freunde der Nacht</h3></div><p>Lichtschutz</p></a>
<a class="tile" href="https://cseligman.com/text/atlas.htm" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=cseligman.com&sz=32"><h3>Seligman Atlas</h3></div><p>Deep Sky</p></a>
<a class="tile" href="https://astrofan80.de/html/links.html" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=astrofan80.de&sz=32"><h3>Astrofan80</h3></div><p>Links</p></a>
<a class="tile" href="https://www.der-mond.de/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=der-mond.de&sz=32"><h3>Der Mond</h3></div><p>Mond</p></a>
</div>
</section>

<section>
<h2>🌌 Beobachtungsbedingungen</h2>
<div class="tiles">
<a class="tile" href="https://www.lightpollutionmap.info" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=lightpollutionmap.info&sz=32"><h3>Light Pollution</h3></div><p>Bortle</p></a>
<a class="tile" href="https://www.wetteronline.at/wetter/stockerau" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=wetteronline.at&sz=32"><h3>Wetter</h3></div><p>Stockerau</p></a>
<a class="tile" href="https://www.wetteronline.at/wetterradar/oesterreich" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=wetteronline.at&sz=32"><h3>Radar</h3></div><p>AT</p></a>
<a class="tile" href="https://www.meteoblue.com/de/wetter/outdoorsports/seeing/stockerau_%c3%96sterreich_2764279" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=meteoblue.com&sz=32"><h3>Meteoblue</h3></div><p>Seeing</p></a>
<a class="tile" href="https://sdo.gsfc.nasa.gov/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=nasa.gov&sz=32"><h3>SDO</h3></div><p>Solar</p></a>
<a class="tile" href="https://www.solarmonitor.org/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=solarmonitoring.org&sz=32"><h3>Solar</h3></div><p>Monitoring</p></a>
</div>
</section>

<section>
<h2>🛒 Shops</h2>
<div class="tiles">
<a class="tile" href="https://www.teleskop-austria.at" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=teleskop-austria.at&sz=32"><h3>Teleskop Austria</h3></div><p>AT</p></a>
<a class="tile" href="https://www.teleskop-spezialisten.de" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=teleskop-spezialisten.de&sz=32"><h3>Spezialisten</h3></div><p>Beratung</p></a>
<a class="tile" href="https://www.teleskop-express.de" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=teleskop-express.de&sz=32"><h3>Teleskop Express</h3></div><p>Zubehör</p></a>
<a class="tile" href="https://www.astroshop.de" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=astroshop.de&sz=32"><h3>Astroshop</h3></div><p>EU</p></a>
<a class="tile" href="http://www.intercon-spacetec.de/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=intercon-spacetec.de&sz=32"><h3>Intercon Spacetec</h3></div><p>Industrie</p></a>
</div>
</section>

<section>
<h2>🔬 Research</h2>
<div class="tiles">
<a class="tile" href="https://aladin.cds.unistra.fr/AladinLite/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=unistra.fr&sz=32"><h3>Aladin</h3></div><p>Atlas</p></a>
<a class="tile" href="https://portal.cds.unistra.fr/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=unistra.fr&sz=32"><h3>CDS</h3></div><p>Kataloge</p></a>
<a class="tile" href="https://www.stelledoppie.it/index2.php?section=1" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=stelledoppie.it&sz=32"><h3>Doppelsterne</h3></div><p>SD</p></a>
<a class="tile" href="https://physics.nist.gov/PhysRefData/ASD/lines_form.html" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=nist.gov&sz=32"><h3>NIST</h3></div><p>Linien</p></a>
<a class="tile" href="https://www.aavso.org/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=aavso.org&sz=32"><h3>AAVSO</h3></div><p>Variabel</p></a>
</div>
</section>

<section>
<h2>🏛 Vereine & Sternwarten</h2>
<div class="tiles">
<a class="tile" href="https://www1.astroverein.at/beobachten" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=astroverein.at&sz=32"><h3>Astroverein AT</h3></div><p>Beob.</p></a>
<a class="tile" href="https://www.waa.at/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=waa.at&sz=32"><h3>WAA</h3></div><p>Wien</p></a>
<a class="tile" href="https://astronomie-burgenland.at/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=astronomie-burgenland.at&sz=32"><h3>Burgenland</h3></div><p>Verein</p></a>
<a class="tile" href="https://brentenriegel.at/" target="_blank"><div class="tile-header"><img class="tile-icon" src="https://www.google.com/s2/favicons?domain=brentenriegel.at&sz=32"><h3>Brentenriegel</h3></div><p>Sternwarte</p></a>
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
