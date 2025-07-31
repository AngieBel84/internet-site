<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <title>Contact - Angela Bellini</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <link rel="stylesheet" href="style.css" />
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display&family=Montserrat&display=swap" rel="stylesheet" />
  <style>

  .hero {
   margin-top: 200px; /* ajuste à ta convenance */
  }

  .body {
    font-family: 'Montserrat', sans-serif;
  }

  .categorie {
    overflow: hidden;
    border-radius: 8px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .categorie img {
    width: 100%;
    height: auto;
    display: block;
    transition: transform 0.4s ease;
  }

  .categorie:hover img {
    transform: scale(1.05);
    }

  .navbar {
    width: 100%;
    max-width: 1200px; /* même valeur utilisée pour centrer le contenu */
    margin: 0 auto;
    padding: 0 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .categorie:hover {
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.25);
    transform: translateY(-5px);
  }

  .hero {
    position: relative;
    height: 100vh;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
    padding: 0 20px;
  }

  .hero::before {
    content: "";
    position: absolute;
    inset: 0;
    background-image: url('images/Angela-atelier.jpg'), url('images/Galaxie-astrocytes-2020.jpg'), url('images/detail diablEspie.jpg');
    background-size: 33.34% 100%;
    background-repeat: no-repeat;
    background-position: left, center, right;
    z-index: 0;
    filter: brightness(1);
  }

  .hero-text {
    position: relative;
    z-index: 1;
    background-color: rgba(0, 0, 0, 0.4);
    padding: 20px;
    border-radius: 10px;
    max-width: 800px;
    width: 100%;
  }

  .hero-text h1 {
    font-size: 3em;
    margin-bottom: 0.3em;
  }

  .hero-text p {
    font-size: 1.5em;
    line-height: 1.4;
  }

  @media (max-width: 768px) {
    .hero {
      flex-direction: column;
      padding: 0 10px;
    }

    .hero-text h1 {
      font-size: 2em;
    }

    .hero-text p {
      font-size: 1.2em;
    }
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

  <main>
    <section class="hero">
      <div class="container"></div>
        <div class="hero-text">
          <h1>Bienvenue dans l'univers d’Angela Bellini</h1>
          <p>Peindre l’essentiel, révéler l’invisible entre science, art et voyages.</p>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 – Angela Bellini</p>
  </footer>
</body>
</html>


