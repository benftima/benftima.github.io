
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Ben Ftima — Cours, exercices et vidéos de mathématiques pour le Bac en Tunisie.">
<title>Ben Ftima — Mathématiques</title>

<style>
:root{
  --green:#6db33f;
  --green-dark:#4f8f2b;
  --ink:#24313a;
  --muted:#66727a;
  --line:#e5e8ea;
  --bg:#f7f9fa;
  --white:#ffffff;
}

*{box-sizing:border-box}
html{scroll-behavior:smooth}

body{
  margin:0;
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Arial,sans-serif;
  color:var(--ink);
  background:var(--white);
  line-height:1.65;
}

a{color:inherit;text-decoration:none}

.topbar{
  height:4px;
  background:var(--green);
}

header{
  border-bottom:1px solid var(--line);
  background:#fff;
  position:sticky;
  top:0;
  z-index:10;
}

.nav{
  max-width:1180px;
  margin:auto;
  min-height:68px;
  padding:0 24px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:20px;
}

.logo{
  font-size:1.25rem;
  font-weight:700;
  letter-spacing:-.3px;
}

.logo span{color:var(--green)}

nav{
  display:flex;
  gap:6px;
  flex-wrap:wrap;
}

nav a{
  padding:9px 13px;
  border-radius:5px;
  color:#53616a;
  font-size:.94rem;
}

nav a:hover{
  background:#f0f4f5;
  color:var(--ink);
}

.hero{
  background:linear-gradient(to bottom,#f7faf8,#fff);
  border-bottom:1px solid var(--line);
}

.hero-inner{
  max-width:1180px;
  margin:auto;
  padding:90px 24px 82px;
  display:grid;
  grid-template-columns:1.2fr .8fr;
  gap:70px;
  align-items:center;
}

.eyebrow{
  color:var(--green-dark);
  font-weight:700;
  font-size:.88rem;
  text-transform:uppercase;
  letter-spacing:1.2px;
  margin-bottom:12px;
}

h1{
  font-size:clamp(2.5rem,5vw,4.5rem);
  line-height:1.08;
  letter-spacing:-2px;
  margin:0 0 22px;
  font-weight:700;
}

h1 .accent{color:var(--green)}

.hero p{
  max-width:700px;
  font-size:1.12rem;
  color:var(--muted);
  margin:0 0 30px;
}

.actions{
  display:flex;
  gap:12px;
  flex-wrap:wrap;
}

.btn{
  display:inline-block;
  padding:12px 20px;
  border-radius:5px;
  border:1px solid var(--green);
  font-weight:600;
  transition:.15s ease;
}

.btn-primary{
  background:var(--green);
  color:#fff;
}

.btn-primary:hover{background:var(--green-dark)}

.btn-secondary{
  background:#fff;
  color:var(--ink);
  border-color:#cfd6da;
}

.btn-secondary:hover{border-color:var(--green)}

.math-box{
  border:1px solid #dfe5e8;
  border-radius:8px;
  background:#fff;
  padding:28px;
  box-shadow:0 8px 30px rgba(30,45,55,.07);
}

.math-title{
  font-size:.82rem;
  color:var(--muted);
  margin-bottom:22px;
  text-transform:uppercase;
  letter-spacing:.8px;
}

.formula{
  font-family:Georgia,"Times New Roman",serif;
  font-size:2rem;
  text-align:center;
  padding:25px 8px;
  border-top:1px solid var(--line);
  border-bottom:1px solid var(--line);
}

.graph{
  margin-top:22px;
  height:120px;
  position:relative;
  overflow:hidden;
}

.graph .axis-x{
  position:absolute;
  left:0;right:0;top:75%;
  border-top:1px solid #9aa4aa;
}

.graph .axis-y{
  position:absolute;
  left:50%;top:0;bottom:0;
  border-left:1px dashed #9aa4aa;
}

.graph svg{
  position:absolute;
  inset:0;
  width:100%;
  height:100%;
}

.section{
  max-width:1180px;
  margin:auto;
  padding:75px 24px;
}

.section-header{
  margin-bottom:34px;
  max-width:760px;
}

.section-header h2{
  font-size:2rem;
  margin:0 0 10px;
  letter-spacing:-.6px;
}

.section-header p{
  color:var(--muted);
  margin:0;
}

.grid{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:18px;
}

.card{
  border:1px solid var(--line);
  border-radius:7px;
  padding:25px;
  background:#fff;
  transition:.15s ease;
}

.card:hover{
  border-color:#b8c7b0;
  transform:translateY(-2px);
  box-shadow:0 8px 24px rgba(30,45,55,.06);
}

.card .number{
  color:var(--green);
  font-weight:700;
  font-size:.85rem;
}

.card h3{
  margin:10px 0 8px;
  font-size:1.2rem;
}

.card p{
  color:var(--muted);
  font-size:.93rem;
  margin:0 0 17px;
}

.card .more{
  color:var(--green-dark);
  font-weight:600;
  font-size:.9rem;
}

.bac{
  background:var(--bg);
  border-top:1px solid var(--line);
  border-bottom:1px solid var(--line);
}

.bac-inner{
  max-width:1180px;
  margin:auto;
  padding:65px 24px;
  display:flex;
  justify-content:space-between;
  gap:35px;
  align-items:center;
}

.bac h2{
  margin:0 0 10px;
  font-size:2rem;
}

.bac p{
  margin:0;
  color:var(--muted);
  max-width:720px;
}

.sections{
  display:flex;
  flex-wrap:wrap;
  gap:8px;
  margin-top:20px;
}

.tag{
  border:1px solid #d5dde0;
  background:#fff;
  padding:6px 11px;
  border-radius:4px;
  font-size:.84rem;
}

footer{
  border-top:1px solid var(--line);
  color:#748087;
  font-size:.88rem;
}

.footer-inner{
  max-width:1180px;
  margin:auto;
  padding:30px 24px;
  display:flex;
  justify-content:space-between;
  gap:20px;
}

@media(max-width:850px){
  .hero-inner{
    grid-template-columns:1fr;
    padding-top:60px;
  }
  .grid{grid-template-columns:repeat(2,1fr)}
  .bac-inner{flex-direction:column;align-items:flex-start}
}

@media(max-width:560px){
  .nav{padding:0 15px}
  nav a:nth-child(n+3){display:none}
  .hero-inner,.section,.bac-inner{padding-left:18px;padding-right:18px}
  h1{font-size:2.7rem}
  .grid{grid-template-columns:1fr}
  .formula{font-size:1.55rem}
  .footer-inner{flex-direction:column;padding-left:18px;padding-right:18px}
}
</style>
</head>

<body>

<div class="topbar"></div>

<header>
  <div class="nav">
    <a class="logo" href="index.html">Ben <span>Ftima</span></a>

    <nav aria-label="Navigation principale">
      <a href="cours/">Cours</a>
      <a href="exercices/">Exercices</a>
      <a href="videos/">Vidéos</a>
      <a href="bac2027/">Bac 2027</a>
    </nav>
  </div>
</header>

<main>

<section class="hero">
  <div class="hero-inner">

    <div>
      <div class="eyebrow">Mathématiques · Tunisie</div>

      <h1>
        Comprendre les maths,<br>
        <span class="accent">pas seulement les apprendre.</span>
      </h1>

      <p>
        Cours structurés, exercices progressifs et vidéos explicatives
        pour accompagner les élèves dans leur préparation au Bac.
      </p>

      <div class="actions">
        <a class="btn btn-primary" href="cours/">Découvrir les cours</a>
        <a class="btn btn-secondary" href="exercices/">Voir les exercices</a>
      </div>
    </div>

    <div class="math-box">
      <div class="math-title">Exemple — étude d'une fonction</div>

      <div class="formula">
        f(x) = x² + 1/x²
      </div>

      <div class="graph" aria-label="Illustration graphique">
        <div class="axis-x"></div>
        <div class="axis-y"></div>
        <svg viewBox="0 0 400 120" preserveAspectRatio="none">
          <path d="M8,18 C48,25 78,52 115,72 C138,84 153,84 168,78
                   M232,78 C247,84 262,84 285,72 C322,52 352,25 392,18"
                fill="none" stroke="#24313a" stroke-width="2"/>
          <circle cx="151" cy="83" r="3.5" fill="#6db33f"/>
          <circle cx="249" cy="83" r="3.5" fill="#6db33f"/>
        </svg>
      </div>
    </div>

  </div>
</section>

<section class="section" id="ressources">

  <div class="section-header">
    <h2>Ressources</h2>
    <p>
      Un espace organisé pour retrouver rapidement les notions,
      les méthodes et les entraînements.
    </p>
  </div>

  <div class="grid">

    <a class="card" href="cours/">
      <div class="number">01</div>
      <h3>Cours</h3>
      <p>
        Notions, théorèmes, méthodes et exemples expliqués
        progressivement.
      </p>
      <span class="more">Accéder aux cours →</span>
    </a>

    <a class="card" href="exercices/">
      <div class="number">02</div>
      <h3>Exercices</h3>
      <p>
        Exercices classés par chapitre et par niveau,
        avec corrections détaillées.
      </p>
      <span class="more">Voir les exercices →</span>
    </a>

    <a class="card" href="videos/">
      <div class="number">03</div>
      <h3>Vidéos</h3>
      <p>
        Explications pas à pas pour revoir les notions
        et les méthodes essentielles.
      </p>
      <span class="more">Voir les vidéos →</span>
    </a>

    <a class="card" href="bac2027/">
      <div class="number">04</div>
      <h3>Bac 2027</h3>
      <p>
        Préparation, révisions et ressources destinées
        aux élèves du Bac 2027.
      </p>
      <span class="more">Préparer le Bac →</span>
    </a>

  </div>
</section>

<section class="bac">
  <div class="bac-inner">

    <div>
      <h2>Préparation Bac 2027</h2>
      <p>
        Une partie dédiée aux révisions et à la construction progressive
        des connaissances : fonctions, dérivation, limites, nombres
        complexes, transformations du plan et autres chapitres.
      </p>

      <div class="sections">
        <span class="tag">Sciences expérimentales</span>
        <span class="tag">Mathématiques</span>
        <span class="tag">Technique</span>
        <span class="tag">Informatique</span>
      </div>
    </div>

    <a class="btn btn-primary" href="bac2027/">Entrer dans Bac 2027</a>

  </div>
</section>

<section class="section">
  <div class="section-header">
    <h2>Une méthode progressive</h2>
    <p>
      Chaque chapitre peut suivre la même logique pédagogique :
      prérequis → découverte → cours → théorèmes → méthode →
      application → exercices → correction.
    </p>
  </div>
</section>

</main>

<footer>
  <div class="footer-inner">
    <div>© 2026 Ben Ftima — Mathématiques</div>
    <div>benftima.github.io</div>
  </div>
</footer>

</body>
</html>
