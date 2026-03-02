<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Your Name | AI Research Portfolio</title>

<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">

<!-- Font Awesome Icons -->
<script src="https://kit.fontawesome.com/yourkit.js" crossorigin="anonymous"></script>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Poppins',sans-serif;
    background:#0a0f1f;
    color:#e6f1ff;
}

/* Animated AI Background */
body::before{
    content:"";
    position:fixed;
    width:100%;
    height:100%;
    background: radial-gradient(circle at 20% 30%, #00f2ff22 0%, transparent 40%),
                radial-gradient(circle at 80% 70%, #8a2be222 0%, transparent 40%);
    animation: move 10s infinite alternate;
    z-index:-1;
}

@keyframes move{
    from{transform:translateY(-20px);}
    to{transform:translateY(20px);}
}

section{
    padding:80px 10%;
}

h1,h2{
    font-family:'Orbitron',sans-serif;
    color:#00f2ff;
    margin-bottom:20px;
}

.card{
    background:#11182e;
    padding:20px;
    margin:20px 0;
    border-radius:12px;
    box-shadow:0 0 20px #00f2ff22;
    transition:0.3s;
}

.card:hover{
    transform:translateY(-5px);
    box-shadow:0 0 25px #00f2ff88;
}

/* Skills Bar */
.skill{
    margin:15px 0;
}

.bar{
    background:#1c2545;
    border-radius:20px;
    overflow:hidden;
}

.progress{
    height:8px;
    background:#00f2ff;
    width:0;
    animation:load 2s forwards;
}

@keyframes load{
    to{width:90%;}
}

footer{
    text-align:center;
    padding:30px;
    background:#11182e;
}
a{
    color:#00f2ff;
    text-decoration:none;
}
</style>
</head>

<body>

<!-- HERO SECTION -->
<section>
    <h1>🤖 Your Name</h1>
    <p>AI / ML Research Enthusiast | Deep Learning | Computer Vision | NLP</p>
    <p>
        📍 Location | 
        📧 yourmail@gmail.com | 
        🔗 <a href="#">LinkedIn</a> | 
        💻 <a href="#">GitHub</a>
    </p>
</section>

<!-- ABOUT -->
<section>
    <h2>🧠 About Me</h2>
    <div class="card">
        Research-driven AI Engineer focused on intelligent systems, scalable ML pipelines, and impactful research solutions. Seeking international internships, MS/MTech, and research collaborations.
    </div>
</section>

<!-- EDUCATION -->
<section>
    <h2>🎓 Education</h2>
    <div class="card">
        <strong>B.Tech in Computer Science</strong><br>
        University Name | 2022–2026<br>
        CGPA: 9.1/10
    </div>
</section>

<!-- PROJECTS -->
<section>
    <h2>🚀 Research Projects</h2>

    <div class="card">
        <strong>AI Medical Diagnosis System</strong><br>
        Deep Learning, CNN, PyTorch<br>
        Built intelligent disease prediction model with 94% accuracy.
    </div>

    <div class="card">
        <strong>Autonomous Vision System</strong><br>
        Computer Vision, OpenCV<br>
        Real-time object detection and tracking system.
    </div>

</section>

<!-- INTERNSHIPS -->
<section>
    <h2>🏢 Internships</h2>
    <div class="card">
        <strong>AI Research Intern</strong><br>
        Organization Name | 2025<br>
        Worked on NLP-based sentiment modeling and deployment.
    </div>
</section>

<!-- WORK EXPERIENCE -->
<section>
    <h2>💼 Work Experience</h2>
    <div class="card">
        <strong>ML Developer</strong><br>
        Company Name | 2024–Present<br>
        Designed scalable ML pipelines and automated workflows.
    </div>
</section>

<!-- SKILLS -->
<section>
    <h2>🛠 Technical Skills</h2>

    <div class="skill">
        Python
        <div class="bar"><div class="progress"></div></div>
    </div>

    <div class="skill">
        Machine Learning
        <div class="bar"><div class="progress"></div></div>
    </div>

    <div class="skill">
        Deep Learning
        <div class="bar"><div class="progress"></div></div>
    </div>

</section>

<!-- GITHUB GRAPH -->
<section>
    <h2>📊 GitHub Activity</h2>
    <img src="https://github-readme-activity-graph.vercel.app/graph?username=yourusername&theme=react-dark" width="100%">
</section>

<!-- INTERESTS -->
<section>
    <h2>🌍 Research Interests</h2>
    <div class="card">
        Artificial Intelligence • Representation Learning • Generative AI • AI for Healthcare • Scalable Systems
    </div>
</section>

<!-- COLLABORATIONS -->
<section>
    <h2>🤝 Collaborations</h2>
    <div class="card">
        Open to international research internships, MS/MTech opportunities, and interdisciplinary AI collaborations.
    </div>
</section>

<footer>
    © 2026 Your Name | AI Research Portfolio
</footer>

</body>
</html>
