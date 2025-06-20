<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Portfolio | Front-End Developer</title>
  <link rel="stylesheet" href="style.css"/>
</head>
<body>
  <header>
    <nav class="navbar">
      <h1 class="logo">Renu Wakode</h1>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="hero fade-in">
    <h2>Hello, I'm <span class="highlight">Renu</span></h2>
    <p>A passionate <strong>Front-End Developer</strong> building beautiful UIs</p>
    <a href="#projects" class="btn">View Projects</a>
  </section>

  <section id="about" class="section fade-in">
    <h2>About Me</h2>
    <p>I love crafting clean, elegant interfaces with HTML, CSS, and JavaScript. I'm constantly learning and enjoy turning ideas into reality.</p>
  </section>

  <section id="projects" class="section fade-in">
    <h2>My Projects</h2>
    <div class="project-container">
      <div class="project-card slide-in">
        <h3>Portfolio Website</h3>
        <p>My personal portfolio built with HTML, CSS, and JavaScript.</p>
      </div>
      <div class="project-card slide-in">
        <h3>To-Do App</h3>
        <p>Organize your tasks with a clean and responsive app.</p>
      </div>
      <div class="project-card slide-in">
        <h3>Weather App</h3>
        <p>Get real-time weather info with open APIs.</p>
      </div>
    </div>
  </section>

  <section id="contact" class="section fade-in">
    <h2>Contact Me</h2>
    <form id="contactForm">
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit" class="btn">Send Message</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Renu Wakode. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: 'Segoe UI', sans-serif;
  line-height: 1.6;
  color: #333;
  background: #fefefe;
  overflow-x: hidden;
}
a {
  text-decoration: none;
  color: inherit;
}
ul {
  list-style: none;
}

/* Navbar */
header {
  background: #222;
  color: white;
  padding: 15px 0;
}
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 90%;
  margin: auto;
}
.logo {
  font-size: 26px;
  color: #00dfc4;
}
.nav-links li {
  display: inline;
  margin-left: 20px;
}
.nav-links a {
  color: white;
  transition: color 0.3s;
}
.nav-links a:hover {
  color: #00dfc4;
}

/* Hero Section */
.hero {
  background: linear-gradient(to right, #00dfc4, #007cf0);
  color: white;
  text-align: center;
  padding: 80px 20px;
  animation: fadeIn 1.2s ease-in;
}
.hero .highlight {
  color: #fffb00;
}
.btn {
  display: inline-block;
  margin-top: 15px;
  padding: 10px 25px;
  background: #fff;
  color: #007cf0;
  font-weight: bold;
  border-radius: 30px;
  transition: 0.3s;
}
.btn:hover {
  background: #000;
  color: #fff;
}

/* Sections */
.section {
  padding: 60px 20px;
  max-width: 1000px;
  margin: auto;
  text-align: center;
}

/* Projects */
.project-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 25px;
  margin-top: 30px;
}
.project-card {
  background: #fff;
  padding: 25px;
  width: 280px;
  border-radius: 10px;
  box-shadow: 0 6px 12px rgba(0,0,0,0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.project-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 12px 24px rgba(0,0,0,0.15);
}

/* Contact Form */
form {
  max-width: 500px;
  margin: auto;
  display: flex;
  flex-direction: column;
  gap: 15px;
}
form input, form textarea {
  padding: 12px;
  border: 2px solid #007cf0;
  border-radius: 8px;
  font-size: 16px;
}
form button {
  cursor: pointer;
}

/* Footer */
footer {
  text-align: center;
  padding: 25px;
  background: #222;
  color: white;
  margin-top: 40px;
}

/* Animations */
.fade-in {
  opacity: 0;
  animation: fadeIn 1s ease forwards;
}
.slide-in {
  opacity: 0;
  transform: translateY(30px);
  animation: slideUp 0.8s ease-out forwards;
}
@keyframes fadeIn {
  to { opacity: 1; }
}
@keyframes slideUp {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Responsive */
@media (max-width: 768px) {
  .project-container {
    flex-direction: column;
    align-items: center;
  }
  .navbar {
    flex-direction: column;
  }
}
