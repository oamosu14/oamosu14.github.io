<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cybersecurity & DevOps Portfolio</title>

<style>
:root {
    --bg: #0f172a;
    --text: #e2e8f0;
    --card: rgba(255,255,255,0.05);
    --accent: #38bdf8;
}

.light-mode {
    --bg: #f8fafc;
    --text: #0f172a;
    --card: rgba(0,0,0,0.05);
}

body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    background: var(--bg);
    color: var(--text);
    transition: 0.3s;
}

/* HEADER */
header {
    text-align: center;
    padding: 60px 20px;
}

header h1 {
    font-size: 2.5em;
}

header p {
    color: gray;
}

/* TOGGLE */
.toggle {
    position: fixed;
    top: 20px;
    right: 20px;
    cursor: pointer;
    padding: 10px 15px;
    border-radius: 20px;
    background: var(--card);
    backdrop-filter: blur(10px);
}

/* SECTION */
section {
    max-width: 1100px;
    margin: auto;
    padding: 40px 20px;
}

/* PROJECT GRID */
.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
}

/* CARD */
.card {
    background: var(--card);
    padding: 20px;
    border-radius: 15px;
    backdrop-filter: blur(12px);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
    transform: translateY(-8px);
    box-shadow: 0 10px 30px rgba(0,0,0,0.3);
}

/* HEADINGS */
h2 {
    border-bottom: 2px solid var(--accent);
    display: inline-block;
    margin-bottom: 20px;
}

/* BUTTON */
.btn {
    display: inline-block;
    margin-top: 10px;
    padding: 8px 12px;
    border-radius: 8px;
    background: var(--accent);
    color: white;
    text-decoration: none;
}

/* ANIMATION */
.fade-in {
    opacity: 0;
    transform: translateY(20px);
    animation: fadeIn 1s forwards;
}

@keyframes fadeIn {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
</style>
</head>

<body>

<div class="toggle" onclick="toggleMode()">🌙 / ☀️</div>

<header class="fade-in">
    <h1>🚀 Cybersecurity & DevOps Portfolio</h1>
    <p>Enterprise Projects | Security-First Engineering</p>
</header>

<section class="fade-in">
<h2>👤 Professional Summary</h2>
<p>
I am a DevOps and Systems Engineer with 11+ years of experience in Linux, cybersecurity, and cloud infrastructure. I focus on integrating security into DevOps pipelines and building resilient, automated systems.
</p>
</section>

<section class="fade-in">
<h2>🛠️ Technical Skills</h2>
<p>Ansible, Jenkins, AWS, Azure, Docker, Kubernetes, Nagios, Splunk, Linux, Windows Server</p>
</section>

<section class="fade-in">
<h2>💼 Projects</h2>

<div class="grid">

<div class="card">
<h3>🔐 Security Hardening</h3>
<p>Firewall, IDS/IPS, monitoring, and DevSecOps integration.</p>
<a class="btn" href="#">View Project</a>
</div>

<div class="card">
<h3>🔐 VPN & Secure Workstation</h3>
<p>Enterprise endpoint with MFA and VPN enforcement.</p>
<a class="btn" href="#">View Project</a>
</div>

<div class="card">
<h3>⚙️ DevOps Pipeline</h3>
<p>CI/CD automation using Jenkins and Ansible.</p>
<a class="btn" href="#">View Project</a>
</div>

<div class="card">
<h3>🛡️ SOC Lab</h3>
<p>Threat detection and incident response simulation.</p>
<a class="btn" href="#">View Project</a>
</div>

<div class="card">
<h3>🖥️ Linux Home Lab</h3>
<p>Enterprise Linux environment with automation.</p>
<a class="btn" href="#">View Project</a>
</div>

<div class="card">
<h3>🎓 IT Resource Hub</h3>
<p>Learning platform for certifications and labs.</p>
<a class="btn" href="#">View Project</a>
</div>

</div>
</section>

<section class="fade-in">
<h2>🌟 Final Note</h2>
<p>
These projects demonstrate real-world cybersecurity and DevOps skills with a focus on automation and enterprise design.
</p>
</section>

<section class="fade-in">
<h2>📫 Contact</h2>
<p>Email: your@email.com</p>
</section>

<script>
function toggleMode() {
    document.body.classList.toggle("light-mode");
}
</script>

</body>
</html>
