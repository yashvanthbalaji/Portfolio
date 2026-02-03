# Ex01 Portfolio
## Date: 30.01.2026

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html).

### STEP 2
Create a CSS file (style.css).

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
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="keywords" content="Balaji A, portfolio, Balaji, full stack dev, personal portfolio, portfolio design, portfolio website, personal portfolio" />
    <meta name="description" content="Welcome to Balaji's Portfolio. Full-Stack Web Developer and Android App Developer" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" xintegrity="sha512-iBBXm8fW90+nuLcSKlbmrPcLa0OT92xO1BIsZ+ywDWZCvqsWgccV3gFoRBv0z+8dLJgyAHIhR35VZc2oM/gI1w==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <title>Portfolio | Balaji A</title>

    <style>
        @import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap");
        @import url('https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,300;0,400;0,600;0,700;1,300;1,400&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            text-decoration: none;
            outline: none; 
            border: none;
            text-transform: capitalize;
            transition: all .2s linear;
        }

        html {
            font-size: 62.5%;
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        body {
            background: #f7f7f7;
            font-family: 'Poppins', sans-serif;
        }

        *::selection {
            background: #2b3dda;
            color: #fff;
        }

        html::-webkit-scrollbar {
            width: .8rem;
        }

        html::-webkit-scrollbar-track {
            background: rgb(235, 202, 245);
        }

        html::-webkit-scrollbar-thumb {
            background: #420177;
        }

        /* Navbar */
        header {
            position: fixed;
            top: 0; left: 0; right: 0;
            z-index: 1000;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 1.7rem 10%;
            height: 6.5rem;
            background-color: #fff;
            box-shadow: 0 1px 4px rgba(146,161,176,.3);
        }

        section {
            min-height: 100vh;
            padding: 2rem 9%;
        }

        .heading {
            font-size: 3.5rem;
            color: rgb(20, 20, 20);
            font-weight: 800;
            text-align: center;
            margin-bottom: 2rem;
        }

        .heading span {
            color: rgb(115, 3, 167);
        }

        header .logo {
            font-size: 1.9rem;
            font-weight: 800;
            text-decoration: none;
            color: #0E2431;
        }

        header .navbar ul {
            list-style: none;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        header .navbar li {
            margin-left: 2.5rem;
        }

        header .navbar ul li a {
            font-size: 1.57rem;
            color: #0E2431;
            font-weight: 600;
        }

        header .navbar ul li a:hover {
            color: #011aff;
            border-bottom: .2rem solid #011aff;
            padding: .5rem 0;
        }

        /* Home Section */
        .home {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap: 1.5rem;
            background: #f7f7f7;
        }

        .home .content {
            flex: 1 1 40rem;
        }

        .home .content h2 {
            font-size: 5rem;
            color: #002057;
        }

        .home .content h2 span {
            color: #ff7b00;
        }

        .home .content p {
            font-size: 2.5rem;
            color: #000;
            padding: 1rem 0;
        }

        .home .image {
            flex: 1 1 40rem;
            text-align: center;
        }

        .home .image img {
            width: 80%;
            border-radius: 50%;
            box-shadow: 0 2px 8px rgba(0,0,0,0.3);
        }

        .btn {
            display: inline-block;
            margin-top: 1rem;
            padding: 1.6rem 3rem;
            border-radius: 4rem;
            background: #2506ad;
            color: #fff;
            font-size: 1.7rem;
            font-weight: 700;
            box-shadow: 0px 5px 18px rgba(48, 68, 247, 0.6);
        }

        .socials .social-icons {
            list-style: none;
            margin-top: 2rem;
        }

        .socials .social-icons li {
            display: inline-block;
            margin-right: 1rem;
        }

        .social-icons a {
            font-size: 2rem;
            display: block;
            line-height: 44px;
            color: #00d9ff;
            background: #09011b;
            width: 44px;
            height: 44px;
            text-align: center;
            border-radius: 50%;
        }

        /* About Section */
        .about {
            background: #fff;
        }

        .about .row {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap: 2rem;
        }

        .about .row .image {
            flex: 1 1 35rem;
            text-align: center;
        }

        .about .row .image img {
            width: 30rem;
            border-radius: 1rem;
            box-shadow: 0 5px 10px rgba(0,0,0,0.2);
        }

        .about .row .content {
            flex: 1 1 45rem;
        }

        .about .row .content h3 {
            font-size: 2.5rem;
            color: #333;
        }

        .about .row .content .tag {
            font-size: 1.6rem;
            color: #011aff;
            font-weight: 600;
        }

        .about .row .content p {
            font-size: 1.5rem;
            margin-top: 1.5rem;
            line-height: 1.6;
        }

        /* Skills Section */
        .skills {
            background: linear-gradient(to bottom, #57059e, #4a00e0);
            color: #fff;
        }

        .skills .container {
            background: rgba(0,0,0,0.2);
            padding: 2rem;
            border-radius: 1rem;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1.5rem;
        }

        .skills .bar {
            background: rgba(255,255,255,0.1);
            padding: 1rem 2rem;
            border-radius: .5rem;
            display: flex;
            align-items: center;
            gap: 1rem;
            min-width: 15rem;
        }

        .skills .bar img {
            height: 3rem;
        }

        .skills .bar span {
            font-size: 1.6rem;
            font-weight: 600;
        }

        /* Education */
        .education .box-container {
            display: flex;
            flex-wrap: wrap;
            gap: 1.5rem;
        }

        .education .box {
            flex: 1 1 33rem;
            background: #fff;
            padding: 2rem;
            border-radius: .5rem;
            box-shadow: 0 .5rem 1rem rgba(0,0,0,0.1);
            text-align: center;
        }

        .education .box h3 {
            font-size: 2rem;
            color: #011aff;
        }

        /* Experience Timeline */
        .experience .timeline {
            position: relative;
            max-width: 1200px;
            margin: 2rem auto;
            padding: 1rem;
        }

        .experience .timeline::after {
            content: '';
            position: absolute;
            width: 6px;
            background: #020133;
            top: 0; bottom: 0; left: 50%;
            margin-left: -3px;
        }

        .experience .container {
            padding: 1rem 4rem;
            position: relative;
            width: 50%;
        }

        .experience .container.left { left: 0; }
        .experience .container.right { left: 50%; }

        .experience .content {
            padding: 2rem;
            background: #f68c09;
            color: #fff;
            border-radius: .5rem;
        }

        /* Contact Section (Non-input version) */
        .contact .container {
            max-width: 60rem;
            margin: 0 auto;
            background: #fff;
            padding: 4rem;
            border-radius: 1rem;
            box-shadow: 0 .5rem 1rem rgba(0,0,0,0.1);
            text-align: center;
        }

        .contact .info-card {
            display: flex;
            flex-direction: column;
            gap: 2rem;
            font-size: 1.8rem;
        }

        .contact .info-item {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 1.5rem;
            color: #333;
        }

        .contact .info-item i {
            color: #2506ad;
            font-size: 2.2rem;
        }

        /* Footer */
        .footer {
            background: rgb(0, 1, 43);
            color: #fff;
            padding: 3rem 9%;
            text-align: center;
        }

        .footer .box-container {
            display: flex;
            flex-wrap: wrap;
            gap: 2rem;
            text-align: left;
            margin-bottom: 2rem;
        }

        .footer .box {
            flex: 1 1 25rem;
        }

        .footer h3 { font-size: 2rem; margin-bottom: 1rem; }
        .footer p { font-size: 1.4rem; color: #ccc; }

        .footer .credit {
            border-top: .1rem solid #fff3;
            padding-top: 2rem;
            font-size: 1.6rem;
        }

        /* Responsive Settings */
        @media (max-width: 768px) {
            header .navbar { display: none; }
            .experience .timeline::after { left: 31px; }
            .experience .container { width: 100%; padding-left: 70px; left: 0 !important; }
        }
    </style>
</head>
<body>

<header>
    <a href="#" class="logo"><i class="fab fa-node-js"></i> Balaji</a>
    <nav class="navbar">
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<section class="home" id="home">
    <div class="content">
        <h2>Hi There,<br/> I'm Balaji <span>A</span></h2>
        <p>I am a Passionate Developer</p>
        <div class="socials">
            <ul class="social-icons">
                <li><a class="linkedin" href="https://linkedin.com/in/yashvanthbalaji-undefined-5073932a8" target="_blank"><i class="fab fa-linkedin"></i></a></li>
                <li><a class="github" href="https://github.com/yashvanthbalaji" target="_blank"><i class="fab fa-github"></i></a></li>
                <li><a class="instagram" href="#" target="_blank"><i class="fab fa-instagram"></i></a></li>
            </ul>
        </div>
    </div>
    <div class="image">
        <img src="https://via.placeholder.com/400x400/002057/FFFFFF?text=Balaji+A" alt="Balaji Profile">
    </div>
</section>

<section class="about" id="about">
    <h2 class="heading"><i class="fas fa-user-alt"></i> About <span>Me</span></h2>
    <div class="row">
        <div class="image">
            <img src="https://via.placeholder.com/300x400" alt="About Image">
        </div>
        <div class="content">
            <h3>I'm Balaji</h3>
            <span class="tag">Computer Science Undergraduate</span>
            <p>I am a Computer Science and Engineering student at Saveetha Engineering College, Chennai. I am passionate about coding, problem-solving, and building innovative applications. I enjoy working on projects that combine creativity and technology, from mobile apps to smart hardware ideas. Currently, I’m improving my skills in C, Python, Java, and Web Development.</p>
            
            <div class="box-container">
                <div class="box" style="margin-top:10px; font-size:1.4rem;">
                    <p><span> Email : </span> 333yashvanthbalaji@gmail.com</p>
                    <p><span> Place : </span> Chennai, India - 602105</p>
                </div>
            </div>
        </div>
    </div>
</section>

<section class="skills" id="skills">
    <h2 class="heading"><i class="fas fa-laptop-code"></i> Skills & <span>Abilities</span></h2>
    <div class="container">
        <div class="bar"><img src="https://img.icons8.com/color/48/000000/python.png" /><span>Python</span></div>
        <div class="bar"><img src="https://img.icons8.com/color/48/000000/java-coffee-cup-logo.png" /><span>Java</span></div>
        <div class="bar"><img src="https://img.icons8.com/color/48/000000/c-programming.png" /><span>C</span></div>
        <div class="bar"><img src="https://img.icons8.com/color/48/000000/html-5.png" /><span>HTML5</span></div>
        <div class="bar"><img src="https://img.icons8.com/color/48/000000/css3.png" /><span>CSS3</span></div>
        <div class="bar"><img src="https://img.icons8.com/color/48/000000/javascript.png" /><span>JavaScript</span></div>
        <div class="bar"><img src="https://img.icons8.com/color/48/000000/sql.png" /><span>SQL</span></div>
        <div class="bar"><img src="https://img.icons8.com/color/48/000000/git.png" /><span>Git & GitHub</span></div>
    </div>
</section>

<section class="education" id="education">
    <h1 class="heading"><i class="fas fa-graduation-cap"></i> My <span>Education</span></h1>
    <div class="box-container">
        <div class="box">
            <h3>Bachelor of Engineering in CSE</h3>
            <p>Saveetha Engineering College</p>
            <h4>2023-2027 | Pursuing</h4>
        </div>
        <div class="box">
            <h3>Bio Maths</h3>
            <p>Krishnasamy Memorial Matriculation Higher Secondary School</p>
            <h4>2021-2023 | Completed</h4>
        </div>
    </div>
</section>

<section class="experience" id="experience">
    <h2 class="heading"><i class="fas fa-briefcase"></i> Experience </h2>
    <div class="timeline">
        <div class="container right">
            <div class="content">
                <h3>Connect InfoSystem</h3>
                <p>WEB Application Development | Internship (2025)</p>
            </div>
        </div>
        <div class="container left">
            <div class="content">
                <h3>RETECH Solutions Private Limited</h3>
                <p>Ui / Ux design | Implant (2025)</p>
            </div>
        </div>
    </div>
</section>

<section class="contact" id="contact">
    <h2 class="heading"><i class="fas fa-headset"></i> Contact <span>Details</span></h2>
    <div class="container">
        <div class="info-card">
            <div class="info-item">
                <i class="fas fa-envelope"></i>
                <span>333yashvanthbalaji@gmail.com</span>
            </div>
            <div class="info-item">
                <i class="fas fa-phone-alt"></i>
                <span>+91 6380684400</span>
            </div>
            <div class="info-item">
                <i class="fas fa-map-marker-alt"></i>
                <span>Chennai, India</span>
            </div>
        </div>
    </div>
</section>

<section class="footer">
    <div class="box-container">
        <div class="box">
            <h3>Balaji's Portfolio</h3>
            <p>Thank you for visiting my personal portfolio website. Connect with me over socials.</p>
        </div>
        <div class="box">
            <h3>Quick Links</h3>
            <p>• Home<br>• About<br>• Skills<br>• Experience</p>
        </div>
        <div class="box">
            <h3>Contact Info</h3>
            <p><i class="fas fa-phone"></i> +91 6380684400</p>
            <p><i class="fas fa-envelope"></i> 333yashvanthbalaji@gmail.com</p>
        </div>
    </div>
    <h1 class="credit">Designed with <i class="fa fa-heart" style="color:red"></i> by Balaji A</h1>
</section>

</body>
</html>
```


## OUTPUT
<img width="1917" height="970" alt="image" src="https://github.com/user-attachments/assets/54396340-8545-42d8-9781-6c93f9841678" />
<img width="1886" height="911" alt="image" src="https://github.com/user-attachments/assets/72573b68-e708-4347-880b-20402cec61ba" />
<img width="1903" height="880" alt="image" src="https://github.com/user-attachments/assets/a1060e70-5939-4543-b6e9-ed5026b922ab" />
<img width="1875" height="949" alt="image" src="https://github.com/user-attachments/assets/09d748b8-6348-485b-8711-c0bc3cc0b623" />
<img width="1836" height="959" alt="image" src="https://github.com/user-attachments/assets/a8b69f1d-c17a-4b38-9732-fc80e3c39b7b" />



## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
