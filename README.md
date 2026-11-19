# PoBop-Motion-Pictures-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PoBop Motion Pictures | Cinematic Excellence</title>
<meta name="description" content="PoBop Motion Pictures - Film production, music videos, cinematography and visual storytelling.">

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html { scroll-behavior: smooth; }

body {
  background: #090909;
  color: white;
  font-family: Arial, sans-serif;
}

header {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 100;
  background: rgba(5,5,5,.94);
  border-bottom: 1px solid #292929;
  padding: 18px 7%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  font-size: 21px;
  font-weight: 900;
  letter-spacing: 2px;
}

.logo span { color: #d4a644; }

nav {
  display: flex;
  gap: 25px;
}

nav a {
  text-decoration: none;
  color: white;
  font-size: 13px;
  transition: .3s;
}

nav a:hover { color: #d4a644; }

.menu {
  display: none;
  font-size: 27px;
  cursor: pointer;
  color: #d4a644;
}

.hero {
  min-height: 100vh;
  display: flex;
  align-items: center;
  padding: 130px 9% 70px;
  background:
  linear-gradient(90deg,rgba(0,0,0,.92),rgba(0,0,0,.25)),
  url("https://images.unsplash.com/photo-1485846234645-a62644f84728?auto=format&fit=crop&w=2000&q=85");
  background-size: cover;
  background-position: center;
}

.hero-content { max-width: 720px; }

.tag {
  color: #d4a644;
  letter-spacing: 5px;
  font-size: 12px;
  margin-bottom: 25px;
}

.hero h1 {
  font-size: clamp(45px, 8vw, 90px);
  line-height: 1.05;
  font-weight: 900;
}

.hero h1 span { color: #d4a644; }

.hero p {
  color: #ccc;
  font-size: 17px;
  line-height: 1.8;
  margin: 25px 0 35px;
}

.btn {
  display: inline-block;
  padding: 15px 30px;
  background: #d4a644;
  color: #080808;
  text-decoration: none;
  font-weight: bold;
  transition: .3s;
}

.btn:hover {
  background: white;
  transform: translateY(-3px);
}

section {
  padding: 100px 9%;
}

.section-title {
  font-size: 38px;
  margin-bottom: 15px;
}

.section-title span { color: #d4a644; }

.subtitle {
  color: #999;
  line-height: 1.7;
  margin-bottom: 45px;
}

.about {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 50px;
  align-items: center;
}

.about img {
  width: 100%;
  height: 400px;
  object-fit: cover;
}

.about p {
  color: #aaa;
  line-height: 1.9;
  margin: 20px 0;
}

.projects {
  background: #111;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.project {
  position: relative;
  height: 280px;
  overflow: hidden;
  background: #222;
}

.project img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: .5s;
}

.project:hover img { transform: scale(1.1); }

.project-info {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 25px 15px 15px;
  background: linear-gradient(transparent, black);
}

.project-info h3 { color: #d4a644; }

.services-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.service {
  background: #151515;
  padding: 35px 25px;
  border: 1px solid #292929;
  transition: .3s;
}

.service:hover {
  border-color: #d4a644;
  transform: translateY(-5px);
}

.service .number {
  color: #d4a644;
  font-size: 30px;
  margin-bottom: 20px;
}

.service h3 { margin-bottom: 15px; }

.service p {
  color: #999;
  line-height: 1.8;
}

.contact {
  background: #121212;
  text-align: center;
}

.contact p {
  color: #aaa;
  margin: 20px 0 30px;
  line-height: 1.8;
}

footer {
  text-align: center;
  padding: 30px;
  background: #050505;
  color: #777;
  font-size: 13px;
}

footer span { color: #d4a644; }

@media(max-width: 768px) {
  nav {
    display: none;
    position: absolute;
    top: 65px;
    left: 0;
    width: 100%;
    background: #080808;
    flex-direction: column;
    padding: 25px;
    gap: 25px;
  }

  nav.active { display: flex; }

  .menu { display: block; }

  .about { grid-template-columns: 1fr; }

  .gallery { grid-template-columns: 1fr; }

  .services-grid { grid-template-columns: 1fr; }

  section { padding: 75px 7%; }
}
</style>
</head>

<body>

<header>
  <div class="logo">PoBop <span>MOTION PICTURES</span></div>
  <div class="menu" onclick="toggleMenu()">☰</div>

  <nav id="navigation">
    <a href="#home" onclick="closeMenu()">HOME</a>
    <a href="#about" onclick="closeMenu()">ABOUT</a>
    <a href="#projects" onclick="closeMenu()">PROJECTS</a>
    <a href="#services" onclick="closeMenu()">SERVICES</a>
    <a href="#contact" onclick="closeMenu()">CONTACT</a>
  </nav>
</header>

<main>
<section class="hero" id="home">
  <div class="hero-content">
    <div class="tag">FILM • ART • CREATIVITY</div>
    <h1>WE CREATE<br><span>VISUAL</span><br>STORIES.</h1>
    <p>
      Bringing imagination to life through powerful cinematography,
      professional video production and unforgettable storytelling.
    </p>
    <a href="#projects" class="btn">EXPLORE OUR WORK</a>
  </div>
</section>

<section id="about">
  <div class="about">
    <div>
      <div class="tag">WHO WE ARE</div>
      <h2 class="section-title">ABOUT <span>PoBop</span></h2>
      <p>
        PoBop Motion Pictures is a creative motion picture brand
        dedicated to producing captivating visual experiences.
        We transform ideas into powerful stories through the art
        of filmmaking and cinematography.
      </p>
      <p>
        From music videos to creative films, our mission is to
        capture moments, inspire audiences and bring every vision
        to life.
      </p>
      <a href="#contact" class="btn">WORK WITH US</a>
    </div>

    <img src="https://images.unsplash.com/photo-1492619375914-88005aa9e8fb?auto=format&fit=crop&w=1000&q=85"
    alt="Professional film production camera">
  </div>
</section>

<section class="projects" id="projects">
  <div class="tag">OUR PORTFOLIO</div>
  <h2 class="section-title">FEATURED <span>PROJECTS</span></h2>
  <p class="subtitle">
    Every frame tells a story. Explore our creative world.
  </p>

  <div class="gallery">
    <div class="project">
      <img src="https://images.unsplash.com/photo-1516280440614-37939bbacd81?auto=format&fit=crop&w=800&q=85" alt="Music video production">
      <div class="project-info"><h3>Music Videos</h3></div>
    </div>

    <div class="project">
      <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=800&q=85" alt="Cinematic filming">
      <div class="project-info"><h3>Film Production</h3></div>
    </div>

    <div class="project">
      <img src="https://images.unsplash.com/photo-1478720568477-152d9b164e26?auto=format&fit=crop&w=800&q=85" alt="Movie camera production">
      <div class="project-info"><h3>Creative Visuals</h3></div>
    </div>
  </div>
</section>

<section id="services">
  <div class="tag">WHAT WE DO</div>
  <h2 class="section-title">OUR <span>SERVICES</span></h2>
  <p class="subtitle">Professional creativity from concept to final production.</p>

  <div class="services-grid">
    <div class="service">
      <div class="number">01</div>
      <h3>Music Video Production</h3>
      <p>Creative music videos that bring artists' musical visions to life.</p>
    </div>

    <div class="service">
      <div class="number">02</div>
      <h3>Film Making</h3>
      <p>Story development, filming and cinematic storytelling.</p>
    </div>

    <div class="service">
      <div class="number">03</div>
      <h3>Video Editing</h3>
      <p>Professional editing, colour grading and visual effects.</p>
    </div>

    <div class="service">
      <div class="number">04</div>
      <h3>Cinematography</h3>
      <p>Beautiful shots and professional camera operation.</p>
    </div>

    <div class="service">
      <div class="number">05</div>
      <h3>Event Coverage</h3>
      <p>Capturing special occasions and unforgettable moments.</p>
    </div>

    <div class="service">
      <div class="number">06</div>
      <h3>Creative Direction</h3>
      <p>Developing original concepts and creative visual identities.</p>
    </div>
  </div>
</section>

<section class="contact" id="contact">
  <div class="tag">LET'S CREATE SOMETHING</div>
  <h2 class="section-title">HAVE A PROJECT <span>IN MIND?</span></h2>
  <p>
    Let's turn your ideas into unforgettable visual experiences.
    Contact PoBop Motion Pictures today.
  </p>
  <a href="mailto:your@email.com" class="btn">CONTACT US</a>
</section>
</main>

<footer>
  © 2026 <span>PoBop Motion Pictures</span>. All Rights Reserved.
  <p style="margin-top:10px;">Creating Stories. Capturing Moments.</p>
</footer>

<script>
function toggleMenu() {
  document.getElementById("navigation").classList.toggle("active");
}

function closeMenu() {
  document.getElementById("navigation").classList.remove("active");
}
</script>

</body>
</html>
