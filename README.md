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
