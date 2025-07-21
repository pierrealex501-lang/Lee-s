# Lee-s
Fashion 
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Lee’s – Boutique de Mode</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header>
    <nav class="navbar">
      <a href="#accueil" class="logo">Lee’s</a>
      <ul class="nav-links">
        <li><a href="#accueil">Accueil</a></li>
        <li><a href="#a-propos">À propos</a></li>
        <li><a href="#collections">Collections</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
    <section id="accueil" class="hero">
      <h1>Mode élégante, tendance française</h1>
      <p>Découvrez nos collections sélectionnées avec soin.</p>
      <a href="#collections" class="btn">Voir les collections</a>
    </section>
  </header>

  <main>
    <section id="a-propos" class="about">
      <h2>À propos de Lee’s</h2>
      <p>Lee’s est une boutique de mode dédiée à l’élégance et au style moderne. Nous sélectionnons des pièces uniques pour sublimer votre quotidien.</p>
    </section>

    <section id="collections" class="collections">
      <h2>Nos collections</h2>
      <div class="gallery">
        <!-- remplacez les images ci-dessous par vos propres visuels -->
        <div class="item"><img src="https://via.placeholder.com/300" alt="Collection 1"><p>Collection 1</p></div>
        <div class="item"><img src="https://via.placeholder.com/300" alt="Collection 2"><p>Collection 2</p></div>
        <div class="item"><img src="https://via.placeholder.com/300" alt="Collection 3"><p>Collection 3</p></div>
      </div>
    </section>

    <section id="contact" class="contact">
      <h2>Contactez-nous</h2>
      <form action="#" method="post">
        <label for="name">Nom</label>
        <input type="text" id="name" name="name" placeholder="Votre nom" required />

        <label for="email">Email</label>
        <input type="email" id="email" name="email" placeholder="Votre email" required />

        <label for="message">Message</label>
        <textarea id="message" name="message" rows="4" placeholder="Votre message"></textarea>

        <button type="submit" class="btn">Envoyer</button>
      </form>
    </section>
  </main>

  <footer class="footer">
    <p>&copy; 2025 Lee’s. Tous droits réservés.</p>
    <p><a href="#mentions-legales">Mentions légales</a></p>
  </footer>
</body>
</html>/* Reset de base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: Arial, sans-serif;
  color: #333;
  line-height: 1.6;
}
a {
  text-decoration: none;
  color: inherit;
}

/* En‑tête et navigation */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background: #fafafa;
  border-bottom: 1px solid #eee;
}
.nav-links {
  list-style: none;
  display: flex;
  gap: 1rem;
}
.nav-links a {
  padding: 0.5rem;
  transition: color 0.3s;
}
.nav-links a:hover {
  color: #a67;
}

/* Hero */
.hero {
  text-align: center;
  padding: 4rem 2rem;
  background: #f5f5f5;
}
.hero h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}
.hero p {
  font-size: 1.2rem;
  margin-bottom: 1.5rem;
}
.btn {
  background: #a67;
  color: #fff;
  padding: 0.75rem 1.5rem;
  border: none;
  border-radius: 25px;
  cursor: pointer;
  transition: background 0.3s;
}
.btn:hover {
  background: #8b5;
}

/* À propos */
.about {
  padding: 3rem 2rem;
  text-align: center;
}

/* Gallery Collections */
.collections {
  padding: 3rem 2rem;
}
.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
}
.item {
  text-align: center;
}
.item img {
  width: 100%;
  border-radius: 10px;
}
.item p {
  margin-top: 0.5rem;
}

/* Formulaire Contact */
.contact {
  padding: 3rem 2rem;
}
.contact form {
  max-width: 500px;
  margin: auto;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}
.contact input,
.contact textarea {
  padding: 0.75rem;
  border: 1px solid #ccc;
  border-radius: 5px;
}
.contact input:focus,
.contact textarea:focus {
  border-color: #a67;
  outline: none;
}

/* Footer */
.footer {
  background: #fafafa;
  text-align: center;
  padding: 1.5rem;
  border-top: 1px solid #eee;
}
.footer a {
  color: #a67;
}
