# pyrenees-dogs-experiences
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pyrénées Dog Experience</title>
  <style>
    body {font-family: Arial; margin:0; background:#f5f5f5;}
    header {background:#2c3e50; color:white; padding:20px; text-align:center;}
    nav {background:#34495e; display:flex; justify-content:center; padding:10px; flex-wrap:wrap;}
    nav a {color:white; margin:10px; text-decoration:none; font-weight:bold;}
    section {padding:40px; text-align:center;}
    .hero {background:url('https://images.unsplash.com/photo-1500530855697-b586d89ba3ee') center/cover; color:white; padding:100px 20px;}
    .btn {background:#e67e22; color:white; padding:10px 20px; border-radius:5px; text-decoration:none;}
    .cards {display:grid; grid-template-columns:repeat(auto-fit,minmax(250px,1fr)); gap:20px;}
    .card {background:white; padding:20px; border-radius:10px; box-shadow:0 2px 5px rgba(0,0,0,0.1); cursor:pointer; transition:0.3s;}
    .card:hover {transform:scale(1.05);}
    .hidden {display:none;}
    .parcours-img {max-width:90%; border-radius:10px; margin-top:20px;}
    footer {background:#2c3e50; color:white; text-align:center; padding:20px;}
  </style>
</head>
<body>

<header>
  <h1>Pyrénées Dog Experience</h1>
  <p>Découvrez Argelès-Gazost et les montagnes avec des chiens issus de refuges</p>
</header>

<nav>
  <a href="#concept">Concept</a>
  <a href="#territoire">Territoire</a>
  <a href="#activites">Activités</a>
  <a href="#valeurs">Valeurs</a>
  <a href="#contact">Contact</a>
</nav>

<section class="hero">
  <h2>Une aventure immersive entre ville et montagne</h2>
  <p>Escape game en plein air avec des chiens pour découvrir les Pyrénées autrement</p>
  <a href="#contact" class="btn">Réserver</a>
</section>

<section id="concept">
  <h2>Notre concept</h2>
  <p>Une activité unique mêlant escape game, découverte du territoire et interaction avec des chiens issus de refuges. Les chiens vous aident à résoudre des énigmes en suivant des odeurs ou en retrouvant des objets cachés.</p>
</section>

<section id="territoire">
  <h2>Un territoire exceptionnel</h2>
  <p>Situé au cœur des Pyrénées, Argelès-Gazost offre un cadre naturel unique entre ville, vallée et montagne. Entre patrimoine local, nature préservée et activités touristiques, notre projet valorise ce territoire tout en sensibilisant à sa protection.</p>
</section>

<section id="activites">
  <h2>Choisissez votre parcours</h2>
  <div class="cards">
    <div class="card" onclick="showParcours('ville')">
      <h3>Parcours Ville</h3>
      <p>Cliquez pour découvrir le parcours en ville</p>
    </div>
    <div class="card" onclick="showParcours('montagne')">
      <h3>Parcours Montagne</h3>
      <p>Cliquez pour découvrir le parcours en montagne</p>
    </div>
  </div>

  <div id="ville" class="hidden">
    <h3>Parcours Ville — "Le secret d’Argelès"</h3>
    <p><strong>Durée :</strong> 1h30 à 2h • <strong>Distance :</strong> env. 3 km • <strong>Niveau :</strong> Facile</p>
    <ol style="text-align:left; max-width:800px; margin:20px auto;">
      <li><strong>Place de la Victoire (Départ)</strong> — Première énigme d’observation. Le chien aide à trouver un objet caché.</li>
      <li><strong>Parc Thermal d’Argelès-Gazost</strong> — Recherche dans le parc, énigme liée à l’histoire de la ville, interaction avec le chien (piste odorante).</li>
      <li><strong>Halle et centre-ville commerçant</strong> — Code à décrypter, indice caché chez un commerçant partenaire.</li>
      <li><strong>Église Saint-Saturnin (Arrivée)</strong> — Énigme finale pour débloquer le trésor.</li>
    </ol>
  </div>

  <div id="montagne" class="hidden">
    <h3>Parcours Montagne — "La trace des Pyrénées"</h3>
    <p><strong>Durée :</strong> 2h à 2h30 • <strong>Distance :</strong> env. 5 à 6 km • <strong>Niveau :</strong> Moyen</p>
    <ol style="text-align:left; max-width:800px; margin:20px auto;">
      <li><strong>Parc Thermal (Départ)</strong> — Introduction du scénario et début de la piste.</li>
      <li><strong>Chemin du Lavoir / Sentiers vers la montagne</strong> — Premières recherches d’indices naturels, le chien suit une piste odorante.</li>
      <li><strong>Forêt de la Vallée des Gaves</strong> — Énigmes sur la faune et la flore, indices cachés en pleine nature.</li>
      <li><strong>Point de vue sur la vallée (Arrivée)</strong> — Énigme logique finale avec récompense.</li>
    </ol>
  </div>
</section>

<section id="valeurs">
  <h2>Nos valeurs</h2>
  <p>🐾 Bien-être animal : réinsertion et formation de chiens de refuges<br>
  🌱 Écologie : respect de la montagne et limitation de l’impact environnemental<br>
  🤝 Partage : activité conviviale pour familles et amis<br>
  🌍 Transfrontalier : partenariat avec des refuges espagnols</p>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>Email : contact@pyreneesdogexperience.fr</p>
  <p>☎️ : 06 12 13 18 37</p>
  <p>📍 Argelès Gazost (65400) : 15 Place de la République</p>
  <p>Follow us on social media! 📱 @Pyrénéesdogexpérience</p>
</section>

<footer>
  <p>&copy; 2026 Pyrénées Dog Experience</p>
</footer>

<script>
function showParcours(type) {
  document.getElementById('ville').classList.add('hidden');
  document.getElementById('montagne').classList.add('hidden');
  document.getElementById(type).classList.remove('hidden');
}
</script>
