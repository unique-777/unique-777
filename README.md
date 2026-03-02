<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Your Name | AI Research Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  scroll-behavior:smooth;
}

body{
  font-family:'Poppins',sans-serif;
  background:#050816;
  color:#e6f1ff;
  overflow-x:hidden;
}

/* Animated Neural Background */
canvas{
  position:fixed;
  top:0;
  left:0;
  z-index:-1;
}

/* Layout */
section{
  padding:80px 10%;
}

h1,h2{
  font-family:'Orbitron',sans-serif;
  color:#00f2ff;
  margin-bottom:20px;
}

.card{
  background:#0f172a;
  padding:25px;
  margin:20px 0;
  border-radius:12px;
  border:1px solid #00f2ff33;
  transition:0.3s;
}

.card:hover{
  transform:translateY(-6px);
  box-shadow:0 0 25px #00f2ff55;
}

/* Skills */
.skill{
  margin:20px 0;
}

.bar{
  background:#1e293b;
  height:8px;
  border-radius:20px;
  overflow:hidden;
}

.progress{
  height:8px;
  width:0;
  background:#00f2ff;
  border-radius:20px;
}

/* Footer */
footer{
  text-align:center;
  padding:40px;
  background:#0f172a;
}

a{
  color:#00f2ff;
  text-decoration:none;
}

/* Responsive */
@media(max-width:768px){
  section{padding:60px 5%;}
}
</style>
</head>

<body>

<canvas id="bg"></canvas>

<section>
  <h1>🤖 Your Name</h1>
  <p>AI / ML Researcher | Deep Learning | Computer Vision | NLP</p>
  <p>
    <i class="fas fa-location-dot"></i> Location |
    <i class="fas fa-envelope"></i> yourmail@gmail.com |
    <a href="#"><i class="fab fa-linkedin"></i> LinkedIn</a> |
    <a href="#"><i class="fab fa-github"></i> GitHub</a>
  </p>
</section>

<section>
<h2><i class="fas fa-brain"></i> About</h2>
<div class="card">
Research-driven AI engineer focused on intelligent systems, scalable ML pipelines, and impactful real-world applications. Seeking international internships, MS/MTech, and research collaborations.
</div>
</section>

<section>
<h2><i class="fas fa-graduation-cap"></i> Education</h2>
<div class="card">
B.Tech in Computer Science — University Name (2022–2026)<br>
CGPA: 9.1/10
</div>
</section>

<section>
<h2><i class="fas fa-microchip"></i> Projects</h2>

<div class="card">
<strong>AI Medical Diagnosis System</strong><br>
CNN-based classification using PyTorch • 94% accuracy • Deployment ready
</div>

<div class="card">
<strong>Autonomous Vision System</strong><br>
YOLO object detection • OpenCV tracking • Real-time inference
</div>

</section>

<section>
<h2><i class="fas fa-building"></i> Internships</h2>
<div class="card">
AI Research Intern — Organization Name (2025)<br>
NLP modeling, evaluation, and deployment.
</div>
</section>

<section>
<h2><i class="fas fa-briefcase"></i> Work Experience</h2>
<div class="card">
Machine Learning Developer — Company Name (2024–Present)<br>
Built scalable ML systems and automated pipelines.
</div>
</section>

<section>
<h2><i class="fas fa-code"></i> Technical Skills</h2>

<div class="skill">Python
<div class="bar"><div class="progress" style="width:90%"></div></div>
</div>

<div class="skill">Machine Learning
<div class="bar"><div class="progress" style="width:85%"></div></div>
</div>

<div class="skill">Deep Learning
<div class="bar"><div class="progress" style="width:80%"></div></div>
</div>

</section>

<section>
<h2><i class="fas fa-chart-line"></i> GitHub Activity</h2>
<img src="https://github-readme-activity-graph.vercel.app/graph?username=yourusername&theme=react-dark" width="100%">
</section>

<section>
<h2><i class="fas fa-globe"></i> Research Interests</h2>
<div class="card">
Artificial Intelligence • Representation Learning • Generative AI • AI for Healthcare • Scalable Systems
</div>
</section>

<section>
<h2><i class="fas fa-handshake"></i> Collaborations</h2>
<div class="card">
Open to international internships, MS/MTech programs, research roles, and AI collaborations.
</div>
</section>

<footer>
© 2026 Your Name | AI Research Portfolio
</footer>

<script>
/* Neural Network Background */
const canvas = document.getElementById('bg');
const ctx = canvas.getContext('2d');

canvas.width = window.innerWidth;
canvas.height = window.innerHeight;

let particles = [];

for(let i=0;i<100;i++){
  particles.push({
    x:Math.random()*canvas.width,
    y:Math.random()*canvas.height,
    vx:(Math.random()-0.5),
    vy:(Math.random()-0.5)
  });
}

function animate(){
  ctx.clearRect(0,0,canvas.width,canvas.height);
  ctx.fillStyle="#00f2ff";
  particles.forEach(p=>{
    p.x+=p.vx;
    p.y+=p.vy;
    if(p.x<0||p.x>canvas.width)p.vx*=-1;
    if(p.y<0||p.y>canvas.height)p.vy*=-1;
    ctx.beginPath();
    ctx.arc(p.x,p.y,2,0,Math.PI*2);
    ctx.fill();
  });
  requestAnimationFrame(animate);
}
animate();
</script>

</body>
</html>
