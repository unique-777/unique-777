<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Research Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <script src="script.js" defer></script>
</head>
<body>
    <header>
        <h1>My Research Portfolio</h1>
        <nav>
            <ul>
                <li><a href="#aboutMe">About Me</a></li>
                <li><a href="#technicalSkills">Technical Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#internships">Internships</a></li>
                <li><a href="#workExperience">Work Experience</a></li>
                <li><a href="#workshops">Workshops</a></li>
                <li><a href="#researchInterests">Research Interests</a></li>
                <li><a href="#collaborationOpportunities">Collaboration Opportunities</a></li>
            </ul>
        </nav>
        <div class="social-icons">
            <a href="mailto:your-email@example.com" class="icon email">📧</a>
            <a href="https://www.linkedin.com/in/your-profile" class="icon linkedin">🔗</a>
            <a href="https://github.com/your-profile" class="icon github">🐱</a>
            <a href="tel:+1234567890" class="icon phone">📞</a>
        </div>
    </header>
    <section id="aboutMe" class="fade-in">
        <h2>About Me</h2>
        <p>Welcome to my portfolio! Here you'll find my research background and projects.</p>
    </section>
    <section id="technicalSkills" class="fade-in">
        <h2>Technical Skills</h2>
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
            <li>Python</li>
            <li>Data Analysis</li>
        </ul>
    </section>
    <section id="projects" class="fade-in">
        <h2>Projects</h2>
        <p>Details about my projects will be showcased here.</p>
    </section>
    <section id="internships" class="fade-in">
        <h2>Internships</h2>
        <p>Information about my internships will be detailed here.</p>
    </section>
    <section id="workExperience" class="fade-in">
        <h2>Work Experience</h2>
        <p>Details about my work experience will be provided here.</p>
    </section>
    <section id="workshops" class="fade-in">
        <h2>Workshops</h2>
        <p>Information about workshops I've conducted or attended.</p>
    </section>
    <section id="researchInterests" class="fade-in">
        <h2>Research Interests</h2>
        <p>A brief overview of my research interests.</p>
    </section>
    <section id="collaborationOpportunities" class="fade-in">
        <h2>Collaboration Opportunities</h2>
        <p>Information on how to collaborate with me.</p>
    </section>
    <footer>
        <p>© 2026 Unique 777. All Rights Reserved.</p>
    </footer>
</body>
</html>

/* styles.css */
body {
    font-family: Arial, sans-serif;
    background-color: #121212;
    color: #e0e0e0;
}
header {
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(10px);
    padding: 20px;
    text-align: center;
}
nav ul {
    list-style-type: none;
    padding: 0;
}
nav ul li {
    display: inline;
    margin: 0 15px;
}
.social-icons {
    margin-top: 10px;
}
.icon {
    margin: 0 10px;
    transition: transform 0.3s;
}
.icon:hover {
    transform: scale(1.2);
}
section {
    margin: 20px;
    padding: 20px;
    border-radius: 10px;
    background-color: rgba(255, 255, 255, 0.2);
}
.fade-in {
    opacity: 0;
    animation: fadeIn 1s forwards;
}
@keyframes fadeIn {
    to { opacity: 1; }
}