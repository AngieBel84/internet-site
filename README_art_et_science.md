<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Art et Science - Angela Bellini</title>
  <link rel="stylesheet" href="style.css">
  <!-- Ajout pour la lightbox -->
  <style>
  
    .galerie-main {
      margin-top: 100px; /* Ajuste selon la hauteur de ta navbar */
    }
  
    .page-title {
      text-align: center;
      margin-top: 80px;
      font-size: 2em;
    }

    .galerie-grid {
      display: flex;
      justify-content: center;
      gap: 20px;
      flex-wrap: wrap;
      padding: 20px;
    }

    .oeuvre img {
      width: 300px;
      height: 300px;
      object-fit: cover;
      cursor: pointer;
      transition: transform 0.3s ease;
}

    .oeuvre img:hover {
      transform: scale(1.05);
    }

    .oeuvre p {
      text-align: center;
      margin-top: 10px;
    }

    /* Lightbox (image en grand) */
    .lightbox {
      display: none;
      position: fixed;
      z-index: 999;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.8);
      justify-content: center;
      align-items: center;
    }

    .lightbox img {
      max-width: 90%;
      max-height: 90%;
    }

    .lightbox:target {
      display: flex;
    }

    .header {
  padding-bottom: 100px;
}
  </style>
</head>
<body>
  <header>
    <nav class="navbar">
      <div class="logo">
        <a href="index.html">
          <img src="images/Logo artiste.jpg" alt="Logo Angela Bellini" class="logo-img">
        </a>
      </div>
      <ul class="menu">
        <li><a href="index.html">Accueil</a></li>
        <li><a href="artiste.html">L'artiste</a></li>
        <li><a href="galerie.html">Les Œuvres</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="galerie-main">
    <h1 class="page-title">Art et Science</h1>

    <div class="galerie-grid">
      <div class="oeuvre">
        <a href="#img1">
          <img src="images/oeuvre1.jpg" alt="Chimeres toxiques">
        </a>
        <p>Chimeres toxiques – 500€</p>
      </div>
      <div class="oeuvre">
        <a href="#img2">
          <img src="images/oeuvre2.jpg" alt="La cicatrice de la terre">
      </a>
        <p>La cicatrice de la terre – 450€</p>
      </div>
      <div class="oeuvre">
        <a href="#img3">
        <img src="images/oeuvre3.jpg" alt="Eclats de vie">
      </a>
        <p>Eclats de vie – 450€</p>
      </div>
    </div>
  </main>
  <!-- Lightbox modals -->
  <div id="img1" class="lightbox">
    <a href="#!"><img src="images/oeuvre1.jpg" alt="Chimères toxiques"></a>
  </div>
  <div id="img2" class="lightbox">
    <a href="#!"><img src="images/oeuvre2.jpg" alt="La cicatrice de la terre"></a>
  </div>
  <div id="img3" class="lightbox">
    <a href="#!"><img src="images/oeuvre3.jpg" alt="Éclats de vie"></a>
  </div>

  <footer>
    <p>&copy; 2025 - Angela Bellini</p>
  </footer>
</body>
</html>

