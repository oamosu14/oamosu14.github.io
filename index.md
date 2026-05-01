<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cybersecurity & DevOps Portfolio</title>

<style>
:root {
  --bg: #0f172a;
  --text: #e5e7eb;
  --accent: #22c55e;
}

body.light {
  --bg: #ffffff;
  --text: #111827;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: var(--bg);
  color: var(--text);
}

/* NAVBAR */
nav {
  display: flex;
  justify-content: space-between;
  padding: 15px 30px;
  background: #020617;
  position: sticky;
  top: 0;
}

nav a {
  color: var(--text);
  margin: 0 10px;
  text-decoration: none;
}

/* HERO */
.hero {
  text-align: center;
  padding: 80px 20px;
}

.hero h1 {
  font-size: 2.5em;
}

.typing {
  color: var(--accent);
  font-weight: bold;
}

/* BUTTON */
.btn {
  padding: 10px 20px;
  background: var(--accent);
  border: none;
  cursor: pointer;
  margin-top: 15px;
}

/* PROJECTS */
.section {
  padding: 50px 20px;
  max-width: 1000px;
  margin: auto;
}

.project {
  border: 1px solid #1f2937;
  padding: 20px;
  margin-bottom: 20px;
  border-radius: 10px;
}

.project img {
  width: 100%;
  margin-top: 10px;
  border-radius: 8px;
}

/* FOOTER */
footer {
  text-align: center;
  padding: 20px;
  background: #020617;
}
</style>
</head>

<body>

<!-- NAVBAR -->
<nav>
  <div><strong>Portfolio</strong></div>
  <div>
    <a href="#home">Home</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
    <button onclick="toggleMode()">🌙</button>
  </div>
</nav>

<!-- HERO -->
<section id="home" class="hero">
  <h1>Cybersecurity & DevOps Engineer</h1>
  <p>I specialize in <span class="typing"></span></p>

  <a href="resume.pdf" download>
    <button class="btn">Download Resume</button>
  </a>
</section>

<!-- PROJECTS -->
<section id="projects" class="section">
  <h2>Projects</h2>

  <div class="project">
    <h3>🔐 Security Hardening Lab</h3>
    <p>Firewall, IDS/IPS, and monitoring implementation with automation.</p>
    <img src="images/nmap.png" alt="Nmap Scan">
  </div>

  <div class="project">
    <h3>🔐 Enterprise VPN Simulation</h3>
    <p>Zero-trust workstation with MFA and VPN enforcement.</p>
    <img src="images/vpn.png" alt="VPN Screenshot">
  </div>

  <div class="project">
    <h3>⚙️ DevOps CI/CD Pipeline</h3>
    <p>Automated deployment pipeline using Jenkins and Ansible.</p>
    <img src="images/jenkins.png" alt="Pipeline">
  </div>

  <div class="project">
    <h3>🛡️ SOC Virtual Lab</h3>
    <p>Threat detection and incident response environment.</p>
    <img src="images/soc.png" alt="SOC Dashboard">
  </div>

</section>

<!-- CONTACT -->
<section id="contact" class="section">
  <h2>Contact</h2>
  <p>Email: your@email.com</p>
  <p>GitHub: github.com/yourusername</p>
</section>

<!-- FOOTER -->
<footer>
  <p>© 2026 Cybersecurity Portfolio</p>
</footer>

<!-- SCRIPTS -->
<script>
// DARK MODE
function toggleMode() {
  document.body.classList.toggle("light");
}

// TYPING EFFECT
const words = ["Cybersecurity", "DevOps", "Cloud Engineering", "Automation"];
let i = 0, j = 0, current = "", isDeleting = false;

function type() {
  current = words[i];

  if (isDeleting) {
    document.querySelector(".typing").textContent = current.substring(0, j--);
    if (j < 0) {
      isDeleting = false;
      i = (i + 1) % words.length;
    }
  } else {
    document.querySelector(".typing").textContent = current.substring(0, j++);
    if (j > current.length) {
      isDeleting = true;
      setTimeout(type, 1000);
      return;
    }
  }
  setTimeout(type, 100);
}

type();
</script>

</body>
</html>
