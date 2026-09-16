# Ex01 Portfolio
## Date:

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
HTML:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Udhaya Nandhini M | Portfolio</title>

    <link rel="stylesheet" href="pf.css">

    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
</head>

<body>

<header>

<nav>
    <h2 class="logo">Portfolio</h2>

    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

</header>

<!-- HERO -->

<section id="home" class="hero">

    <div class="hero-text">

        <h1>Hi, I'm <span>Udhaya Nandhini M</span></h1>

        <h3>AIML Student & Aspiring Developer</h3>

        <p>
            Passionate about Artificial Intelligence, Machine Learning,
            Web Development and exploring new technologies. I enjoy
            learning new skills and building useful digital projects.
        </p>

        <a href="#projects" class="btn">View My Work</a>

    </div>

    <div class="hero-image">

        <img src="udhaya.jpeg" alt="Udhaya Nandhini Profile Picture">

    </div>

</section>

<!-- ABOUT -->

<section id="about">

    <h2>About Me</h2>

    <p>
        I'm a B.Tech Artificial Intelligence & Machine Learning student
        with an interest in web development and emerging technologies.
        I enjoy learning programming, solving problems, working on projects,
        and continuously improving my technical skills.
    </p>

</section>

<!-- PROJECTS -->

<section id="projects">

    <h2>Projects</h2>

    <div class="project-container">

        <div class="card">

            <h3>Portfolio Website</h3>

            <p>
                A responsive personal portfolio website created to
                showcase my skills, projects and achievements.
            </p>

        </div>

        <div class="card">

            <h3>AI/ML Project</h3>

            <p>
                A beginner-friendly Artificial Intelligence and Machine
                Learning project developed as part of my learning journey.
            </p>

        </div>

        <div class="card">

            <h3>Web Development Project</h3>

            <p>
                A modern web project created using HTML, CSS and
                JavaScript to improve my frontend development skills.
            </p>

        </div>

    </div>

</section>

<!-- CONTACT -->

<section id="contact">

    <h2>Contact Me</h2>

    <p>Email : udhayanandhini@example.com</p>

    <p>
        LinkedIn :
        <a href="https://www.linkedin.com/in/udhaya-nandhini-138bb7406"
           target="_blank">
           https://www.linkedin.com/in/udhaya-nandhini-138bb7406
        </a>
    </p>

    <p>
        GitHub :
        <a href="https://github.com/" target="_blank">
            https://udhayanandhini/github.com
        </a>
    </p>

</section>

<footer>

    <p>© 2026 Udhaya Nandhini M | All Rights Reserved</p>

</footer>

</body>
</html>
```

CSS:

```
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Poppins',sans-serif;
    background:#F8F5FC;
    color:#2D2438;
}

/* NAVIGATION */

header{
    position:sticky;
    top:0;
    background:#FFFFFF;
    box-shadow:0 3px 10px rgba(80,50,100,.10);
    z-index:1000;
}

nav{
    width:90%;
    margin:auto;
    display:flex;
    justify-content:space-between;
    align-items:center;
    height:75px;
}

.logo{
    color:#6B4C8A;
    font-size:30px;
}

nav ul{
    display:flex;
    list-style:none;
}

nav ul li{
    margin-left:35px;
}

nav a{
    text-decoration:none;
    color:#3F3548;
    font-weight:500;
    transition:.3s;
}

nav a:hover{
    color:#8B5FBF;
}

/* HERO */

.hero{

    width:90%;
    margin:auto;

    min-height:90vh;

    display:flex;
    justify-content:space-between;
    align-items:center;

}

.hero-text{

    width:55%;

}

.hero-text h1{

    font-size:60px;
    margin-bottom:20px;

}

.hero-text span{

    color:#8B5FBF;

}

.hero-text h3{

    font-size:30px;
    color:#665A70;

}

.hero-text p{

    margin:30px 0;
    line-height:1.8;
    font-size:18px;

}

.btn{

    display:inline-block;
    text-decoration:none;

    background:#8B5FBF;
    color:white;

    padding:15px 35px;

    border-radius:40px;

    transition:.3s;

}

.btn:hover{

    background:#6B4C8A;

    transform:translateY(-3px);

}

.hero-image img{

    width:380px;
    height:380px;
    object-fit:cover;

    border-radius:50%;

    border:8px solid #E8DDF0;

    box-shadow:0 15px 30px rgba(80,50,100,.20);

}

/* ABOUT */

section{

    padding:90px 10%;

}

section h2{

    font-size:42px;
    margin-bottom:30px;
    text-align:center;

    color:#6B4C8A;

}

section p{

    font-size:18px;
    line-height:1.9;
    text-align:center;

}

/* PROJECTS */

#projects{

    background:#F0EAF6;

}

.project-container{

    display:flex;
    justify-content:center;
    gap:30px;
    flex-wrap:wrap;

}

.card{

    width:320px;

    background:white;

    border-radius:18px;

    overflow:hidden;

    box-shadow:0 10px 20px rgba(80,50,100,.08);

    transition:.4s;

    border-top:5px solid #B79ACF;

}

.card:hover{

    transform:translateY(-10px);

    box-shadow:0 18px 35px rgba(80,50,100,.15);

}

.card img{

    width:100%;
    height:200px;
    object-fit:cover;

}

.card h3{

    margin:20px;

    color:#6B4C8A;

}

.card p{

    text-align:left;
    margin:0 20px 20px;
    font-size:15px;

}

/* CONTACT */

#contact{

    background:#6B4C8A;
    color:white;
    text-align:center;

}

#contact h2{

    color:white;

}

#contact p{

    margin:12px;

}

#contact a{

    color:#E8DDF0;
    text-decoration:none;

}

#contact a:hover{

    text-decoration:underline;

}

/* FOOTER */

footer{

    text-align:center;
    padding:25px;
    background:#2D2438;
    color:white;

}

/* RESPONSIVE */

@media(max-width:900px){

.hero{

    flex-direction:column-reverse;
    text-align:center;
    padding-top:50px;

}

.hero-text{

    width:100%;

}

.hero-text h1{

    font-size:42px;

}

.hero-text h3{

    font-size:22px;

}

.hero-image img{

    width:260px;
    height:260px;
    margin-bottom:40px;

}

nav{

    flex-direction:column;
    height:auto;
    padding:20px;

}

nav ul{

    margin-top:20px;
    flex-wrap:wrap;
    justify-content:center;

}

nav ul li{

    margin:10px;

}

}
```

## OUTPUT
<img width="1915" height="862" alt="Screenshot 2026-09-16 101922" src="https://github.com/user-attachments/assets/e5605026-bee6-4a21-81d7-91cad77a8142" />
<img width="1897" height="911" alt="Screenshot 2026-09-16 101956" src="https://github.com/user-attachments/assets/65485bf7-902d-4ab0-b441-e729baddec1a" />
<img width="1897" height="603" alt="Screenshot 2026-09-16 102157" src="https://github.com/user-attachments/assets/ac8bf3de-176b-44a4-baf1-6503acce6466" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
