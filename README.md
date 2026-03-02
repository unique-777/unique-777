<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Your Name | Research Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Inter', sans-serif;
    background: #0f172a;
    color: #e2e8f0;
    scroll-behavior: smooth;
    overflow-x: hidden;
}

/* Animated Background */
body::before {
    content: "";
    position: fixed;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle at 20% 20%, #2563eb33, transparent),
                radial-gradient(circle at 80% 80%, #9333ea33, transparent);
    animation: move 18s infinite alternate;
    z-index: -1;
}

@keyframes move {
    from { transform: translate(-10%, -10%); }
    to { transform: translate(10%, 10%); }
}

header {
    text-align: center;
    padding: 100px 20px 60px;
}

header h1 {
    font-size: 50px;
    font-weight: 800;
    margin-bottom: 15px;
}

header p {
    font-size: 18px;
    color: #94a3b8;
}

nav {
    display: flex;
    justify-content: center;
    gap: 35px;
    padding-bottom: 50px;
    flex-wrap: wrap;
}

nav a {
    text-decoration: none;
    color: #e2e8f0;
    font-weight: 500;
    transition: 0.3s;
}

nav a:hover {
    color: #38bdf8;
}

section {
    max-width: 1000px;
    margin: auto;
    padding: 70px 25px;
}

section h2 {
    font-size: 30px;
    margin-bottom: 30px;
    border-left: 4px solid #38bdf8;
    padding-left: 15px;
}

.card {
    background: #1e293b;
    padding: 25px;
    border-radius: 12px;
    margin-bottom: 25px;
    transition: 0.4s;
    opacity: 0;
    transform: translateY(40px);
}

.card:hover {
    transform: translateY(-5px);
}

ul {
    padding-left: 20px;
    line-height: 1.8;
}

.timeline {
    border-left: 2px solid #334155;
    padding-left: 20px;
}

.timeline-item {
    margin-bottom: 25px;
}

.skills {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
}

.skill-tag {
    background: #334155;
    padding: 8px 14px;
    border-radius: 20px;
    font-size: 14px;
    transition: 0.3s;
}

.skill-tag:hover {
    background: #38bdf8;
    color: #0f172a;
}

.contact a {
    color: #38bdf8;
    text-decoration: none;
}

footer {
    text-align: center;
    padding: 40px 20px;
    color: #64748b;
}

@media(max-width: 768px) {
    header h1 {
        font-size: 36px;
    }
}
</style>
</head>

<body>

<header>
    <h1>Your Name</h1>
    <p>Machine Learning Researcher | Computer Vision | AI Systems</p>
</header>

<nav>
    <a href="#about">About</a>
    <a href="#research">Research</a>
    <a href="#projects">Projects</a>
    <a href="#experience">Experience</a>
    <a href="#skills">Skills</a>
    <a href="#contact">Contact</a>
</nav>

<section id="about">
    <h2>About Me</h2>
    <div class="card">
        <p>
            I am a research student focused on Machine Learning, Computer Vision,
            and scalable AI systems. My work involves designing intelligent models
            for real-world applications including facial recognition, clustering,
            deep learning pipelines, and AutoML frameworks.
        </p>
    </div>
</section>

<section id="research">
    <h2>Research Interests</h2>
    <div class="card">
        <ul>
            <li>Deep Learning & Representation Learning</li>
            <li>Face Recognition & Embedding Systems</li>
            <li>Meta-Learning & AutoML</li>
            <li>Scalable AI Architectures</li>
            <li>Medical AI & Secure ML Systems</li>
        </ul>
    </div>
</section>

<section id="projects">
    <h2>Selected Projects</h2>

    <div class="card">
        <h3>Face Clustering Pipeline</h3>
        <p>Developed embedding-based clustering using RetinaFace, FaceNet and HDBSCAN for automated identity grouping across videos.</p>
    </div>

    <div class="card">
        <h3>AutoML Framework</h3>
        <p>Implemented automated model selection and hyperparameter tuning using AutoKeras for optimal performance.</p>
    </div>

    <div class="card">
        <h3>Deep Image Restoration</h3>
        <p>Designed neural networks for denoising and super-resolution in biomedical and space imaging domains.</p>
    </div>

</section>

<section id="experience">
    <h2>Research Experience</h2>
    <div class="card timeline">
        <div class="timeline-item">
            <strong>Computer Vision Intern</strong><br>
            SPCV Lab – IIT Tirupati<br>
            Jan 2026 – Present<br>
            Working on object recognition and advanced face clustering systems.
        </div>
    </div>
</section>

<section id="skills">
    <h2>Technical Skills</h2>
    <div class="card">
        <div class="skills">
            <div class="skill-tag">Python</div>
            <div class="skill-tag">PyTorch</div>
            <div class="skill-tag">TensorFlow</div>
            <div class="skill-tag">OpenCV</div>
            <div class="skill-tag">Scikit-learn</div>
            <div class="skill-tag">AutoML</div>
            <div class="skill-tag">HDBSCAN</div>
            <div class="skill-tag">Git</div>
            <div class="skill-tag">Linux</div>
        </div>
    </div>
</section>

<section id="contact">
    <h2>Contact</h2>
    <div class="card contact">
        <p>Email: yourmail@example.com</p>
        <p>GitHub: <a href="#">github.com/yourprofile</a></p>
        <p>LinkedIn: <a href="#">linkedin.com/in/yourprofile</a></p>
    </div>
</section>

<footer>
    © 2026 Your Name | Research Portfolio
</footer>

<script>
/* Fade-in Animation on Scroll */
const cards = document.querySelectorAll('.card');

const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.style.opacity = 1;
            entry.target.style.transform = "translateY(0)";
        }
    });
}, { threshold: 0.2 });

cards.forEach(card => observer.observe(card));
</script>

</body>
</html>
