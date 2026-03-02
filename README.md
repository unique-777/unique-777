<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Your Name | AI Research Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:'Inter',sans-serif;
background:#0b1120;
color:#e2e8f0;
overflow-x:hidden;
scroll-behavior:smooth;
}

/* Canvas Background */
canvas{
position:fixed;
top:0;
left:0;
z-index:-1;
}

/* Navbar */
nav{
position:fixed;
top:0;
width:100%;
display:flex;
justify-content:space-between;
align-items:center;
padding:20px 10%;
background:rgba(15,23,42,0.7);
backdrop-filter:blur(10px);
z-index:1000;
}

nav h2{
font-weight:700;
color:#38bdf8;
}

nav ul{
display:flex;
list-style:none;
gap:30px;
}

nav a{
text-decoration:none;
color:#cbd5e1;
transition:0.3s;
font-weight:500;
}

nav a:hover{
color:#38bdf8;
}

/* Hero */
.hero{
min-height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:0 20px;
}

.hero h1{
font-size:60px;
font-weight:800;
margin-bottom:20px;
}

.hero p{
font-size:20px;
color:#94a3b8;
max-width:700px;
margin-bottom:30px;
}

.metrics{
display:flex;
gap:50px;
margin-top:20px;
flex-wrap:wrap;
justify-content:center;
}

.metric{
text-align:center;
}

.metric h3{
font-size:30px;
color:#38bdf8;
}

section{
padding:100px 10%;
max-width:1300px;
margin:auto;
}

h2{
font-size:32px;
margin-bottom:40px;
position:relative;
}

h2::after{
content:"";
position:absolute;
left:0;
bottom:-10px;
width:60px;
height:3px;
background:#38bdf8;
}

/* Cards */
.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
gap:30px;
}

.card{
background:#111827;
padding:30px;
border-radius:15px;
transition:0.4s;
border:1px solid rgba(255,255,255,0.05);
}

.card:hover{
transform:translateY(-8px);
box-shadow:0 20px 40px rgba(0,0,0,0.4);
border:1px solid #38bdf8;
}

.card h3{
margin-bottom:15px;
color:#38bdf8;
}

/* Timeline */
.timeline{
border-left:2px solid #334155;
padding-left:30px;
}

.timeline-item{
margin-bottom:40px;
position:relative;
}

.timeline-item::before{
content:"";
position:absolute;
left:-41px;
top:5px;
width:15px;
height:15px;
background:#38bdf8;
border-radius:50%;
}

/* Skills */
.skills{
display:flex;
flex-wrap:wrap;
gap:15px;
}

.skill{
background:#1e293b;
padding:10px 18px;
border-radius:30px;
font-size:14px;
transition:0.3s;
}

.skill:hover{
background:#38bdf8;
color:#0b1120;
}

/* Footer */
footer{
text-align:center;
padding:50px 20px;
color:#64748b;
}

/* Responsive */
@media(max-width:768px){
.hero h1{
font-size:40px;
}
nav{
padding:20px;
}
section{
padding:80px 20px;
}
}
</style>
</head>
<body>

<canvas id="network"></canvas>

<nav>
<h2>YourName</h2>
<ul>
<li><a href="#about">About</a></li>
<li><a href="#projects">Projects</a></li>
<li><a href="#experience">Experience</a></li>
<li><a href="#skills">Skills</a></li>
<li><a href="#contact">Contact</a></li>
</ul>
</nav>

<div class="hero">
<h1>Your Name</h1>
<p>AI Researcher specializing in Machine Learning, Computer Vision, and scalable intelligent systems for real-world impact.</p>

<div class="metrics">
<div class="metric">
<h3>5+</h3>
<p>Research Projects</p>
</div>
<div class="metric">
<h3>3+</h3>
<p>AI Systems Built</p>
</div>
<div class="metric">
<h3>2026</h3>
<p>Research Active</p>
</div>
</div>
</div>

<section id="about">
<h2>About Me</h2>
<div class="card">
I am a research-driven AI engineer focused on deep learning architectures, representation learning, and scalable computer vision systems. My work bridges theory and real-world deployment, emphasizing robust embeddings, clustering pipelines, and AutoML optimization.
</div>
</section>

<section id="projects">
<h2>Selected Projects</h2>
<div class="grid">
<div class="card">
<h3>Face Clustering System</h3>
Designed an embedding-based clustering pipeline using RetinaFace, FaceNet, and HDBSCAN for automated identity grouping.
</div>
<div class="card">
<h3>AutoML Optimization Framework</h3>
Implemented automated hyperparameter tuning using AutoKeras and scalable training pipelines.
</div>
<div class="card">
<h3>Deep Image Restoration</h3>
Developed deep neural networks for denoising and super-resolution in biomedical imaging.
</div>
</div>
</section>

<section id="experience">
<h2>Research Experience</h2>
<div class="timeline">
<div class="timeline-item">
<strong>Computer Vision Intern</strong><br>
SPCV Lab – IIT Tirupati<br>
Jan 2026 – Present<br>
Working on advanced face recognition and object detection pipelines.
</div>
</div>
</section>

<section id="skills">
<h2>Technical Skills</h2>
<div class="skills">
<div class="skill">Python</div>
<div class="skill">PyTorch</div>
<div class="skill">TensorFlow</div>
<div class="skill">OpenCV</div>
<div class="skill">Scikit-Learn</div>
<div class="skill">AutoML</div>
<div class="skill">HDBSCAN</div>
<div class="skill">Linux</div>
<div class="skill">Git</div>
</div>
</section>

<section id="contact">
<h2>Contact</h2>
<div class="card">
Email: yourmail@example.com <br><br>
GitHub: github.com/yourprofile <br><br>
LinkedIn: linkedin.com/in/yourprofile
</div>
</section>

<footer>
© 2026 Your Name | AI Research Portfolio
</footer>

<script>
/* Neural Network Background */
const canvas = document.getElementById("network");
const ctx = canvas.getContext("2d");
canvas.width = window.innerWidth;
canvas.height = window.innerHeight;

let particlesArray = [];
const numberOfParticles = 80;

class Particle{
constructor(){
this.x = Math.random()*canvas.width;
this.y = Math.random()*canvas.height;
this.size = 2;
this.speedX = Math.random()*1 -0.5;
this.speedY = Math.random()*1 -0.5;
}
update(){
this.x += this.speedX;
this.y += this.speedY;
if(this.x<0||this.x>canvas.width) this.speedX*=-1;
if(this.y<0||this.y>canvas.height) this.speedY*=-1;
}
draw(){
ctx.fillStyle="#38bdf8";
ctx.beginPath();
ctx.arc(this.x,this.y,this.size,0,Math.PI*2);
ctx.fill();
}
}

function init(){
for(let i=0;i<numberOfParticles;i++){
particlesArray.push(new Particle());
}
}

function connect(){
for(let a=0;a<particlesArray.length;a++){
for(let b=a;b<particlesArray.length;b++){
let dx=particlesArray[a].x-particlesArray[b].x;
let dy=particlesArray[a].y-particlesArray[b].y;
let distance=dx*dx+dy*dy;
if(distance<10000){
ctx.strokeStyle="rgba(56,189,248,0.1)";
ctx.lineWidth=1;
ctx.beginPath();
ctx.moveTo(particlesArray[a].x,particlesArray[a].y);
ctx.lineTo(particlesArray[b].x,particlesArray[b].y);
ctx.stroke();
}
}
}
}

function animate(){
ctx.clearRect(0,0,canvas.width,canvas.height);
for(let i=0;i<particlesArray.length;i++){
particlesArray[i].update();
particlesArray[i].draw();
}
connect();
requestAnimationFrame(animate);
}

init();
animate();

window.addEventListener("resize",()=>{
canvas.width=window.innerWidth;
canvas.height=window.innerHeight;
});
</script>

</body>
</html>
