<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nayanapalli Venkata Jahnavi | AI/ML Engineer</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:#0f2027;
color:white;
overflow-x:hidden;
}

/* Animated Background */
body::before{
content:"";
position:fixed;
width:200%;
height:200%;
background:radial-gradient(circle at 30% 30%,#00f5a0,transparent),
radial-gradient(circle at 70% 70%,#00c3ff,transparent);
animation:moveBg 15s linear infinite;
z-index:-1;
opacity:0.15;
}

@keyframes moveBg{
0%{transform:translate(0,0);}
50%{transform:translate(-25%, -25%);}
100%{transform:translate(0,0);}
}

.container{
display:flex;
min-height:100vh;
}

.sidebar{
width:35%;
background:rgba(0,0,0,0.6);
padding:40px;
text-align:center;
backdrop-filter:blur(15px);
}

.sidebar img{
width:180px;
height:180px;
border-radius:50%;
border:4px solid #00f5a0;
margin-bottom:20px;
}

.sidebar h1{
font-size:22px;
}

.sidebar h3{
color:#00f5a0;
margin:10px 0 20px 0;
font-weight:400;
}

.contact{
font-size:14px;
line-height:24px;
}

.main{
width:65%;
padding:50px;
}

.section{
margin-bottom:40px;
}

.section h2{
color:#00f5a0;
margin-bottom:15px;
border-bottom:1px solid #00f5a0;
padding-bottom:5px;
}

/* Animated Skill Bars */

.skill{
margin-bottom:15px;
}

.skill-name{
margin-bottom:5px;
}

.progress{
background:#1f1f1f;
border-radius:20px;
overflow:hidden;
}

.progress-bar{
height:10px;
background:#00f5a0;
width:0;
animation:load 2s forwards;
}

@keyframes load{
100%{width:85%;}
}

/* GitHub Graph */
.github{
margin-top:20px;
}

.footer{
text-align:center;
padding:15px;
opacity:0.6;
font-size:12px;
}
</style>
</head>

<body>

<div class="container">

<div class="sidebar">
<img src="your-photo.jpg">
<h1>Nayanapalli Venkata Jahnavi</h1>
<h3>AI/ML Engineering Aspirant</h3>

<div class="contact">
📍 Kadapa, Andhra Pradesh <br>
📧 jahnavi.venkata777@gmail.com <br>
🔗 <a href="#" style="color:#00f5a0;">LinkedIn</a> |
<a href="#" style="color:#00f5a0;">GitHub</a>
</div>
</div>

<div class="main">

<div class="section">
<h2>About Me</h2>
<p>Research-oriented AI/ML student focused on Computer Vision, Deep Learning and scalable intelligent systems.</p>
</div>

<div class="section">
<h2>Technical Skills</h2>

<div class="skill">
<div class="skill-name">Python</div>
<div class="progress"><div class="progress-bar"></div></div>
</div>

<div class="skill">
<div class="skill-name">Machine Learning</div>
<div class="progress"><div class="progress-bar" style="animation-delay:0.3s;"></div></div>
</div>

<div class="skill">
<div class="skill-name">Computer Vision</div>
<div class="progress"><div class="progress-bar" style="animation-delay:0.6s;"></div></div>
</div>

</div>

<div class="section github">
<h2>GitHub Contribution</h2>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=unique-777&theme=github-dark" width="100%">

</div>

</div>
</div>

<div class="footer">
© 2026 Nayanapalli Venkata Jahnavi | AI Portfolio
</div>

</body>
</html>
