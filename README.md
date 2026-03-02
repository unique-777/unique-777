<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <title>My Professional Portfolio</title>
    <style>
        body {
            background-color: #121212;
            color: #ffffff;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        a {
            color: #00ffcc;
            text-decoration: none;
        }
        .header, .section {
            padding: 20px;
            margin: 10px;
            border-radius: 10px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(5px);
        }
        .icons {
            display: flex;
            justify-content: space-around;
            margin: 20px 0;
        }
        .icon {
            font-size: 30px;
            transition: transform 0.3s;
        }
        .icon:hover {
            transform: scale(1.1);
        }
        h2 {
            border-bottom: 2px solid #00ffcc;
            padding-bottom: 10px;
        }
        .projects, .internships {
            margin-bottom: 40px;
        }
        .call-to-action {
            margin: 20px 0;
            text-align: center;
        }
        .button {
            background: #00ffcc;
            color: #121212;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background 0.3s;
        }
        .button:hover {
            background: #00cc99;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Welcome to My Professional Portfolio</h1>
        <div class="icons">
            <a href="https://www.linkedin.com/in/yourprofile" target="_blank" class="icon"><i class="fab fa-linkedin"></i></a>
            <a href="https://github.com/yourprofile" target="_blank" class="icon"><i class="fab fa-github"></i></a>
            <a href="mailto:youremail@example.com" target="_blank" class="icon"><i class="fas fa-envelope"></i></a>
            <a href="tel:+1234567890" class="icon"><i class="fas fa-phone"></i></a>
        </div>
    </div>

    <div class="section about">
        <h2>About Me</h2>
        <p>Your brief introduction goes here. Share your journey and passion!</p>
    </div>

    <div class="section skills">
        <h2>Technical Skills</h2>
        <p>Languages: HTML, CSS, JavaScript, Python, etc.</p>
        <p>Skills: Web Development, Data Analysis, etc.</p>
    </div>

    <div class="section projects">
        <h2>Projects</h2>
        <ul>
            <li><a href="https://github.com/project1">Project 1</a> - Description of project 1.</li>
            <li><a href="https://github.com/project2">Project 2</a> - Description of project 2.</li>
        </ul>
    </div>

    <div class="section internships">
        <h2>Internships & Work Experience</h2>
        <p>Timeline of experiences...</p>
    </div>

    <div class="section workshops">
        <h2>Workshops</h2>
        <p>Details about workshops attended or conducted.</p>
    </div>

    <div class="section research">
        <h2>Research Interests</h2>
        <p>Your research interests go here.</p>
    </div>

    <div class="call-to-action">
        <h2>Let’s Collaborate!</h2>
        <button class="button">Get in Touch</button>
    </div>

    <script>
        // Add smooth scrolling and any other interactive components here
    </script>
</body>
</html>
