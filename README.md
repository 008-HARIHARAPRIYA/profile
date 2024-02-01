

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Portfolio</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            color: #fff;
            background: url('pro.jpg') no-repeat center center fixed;
            background-size: cover;
        }

        header {
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            text-align: center;
            padding: 1em 0;
            position: relative;
        }

        .profile-photo {
            position: absolute;
            top: 50%;
            left: 2%;
            transform: translateY(-50%);
            width: 80px; /* Adjust the width as needed */
            height: auto;
            border-radius: 50%;
            overflow: hidden;
        }

        .profile-photo img {
            width: 100%;
            height: auto;
            border-radius: 50%;
        }

        h1, p {
            margin: 0.5em 0;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
            padding: 0.5em 0;
        }

        nav a {
            color: white;
            text-decoration: none;
            padding: 0.5em 1em;
            margin: 0 1em;
            font-weight: bold;
            cursor: pointer;
        }

        footer {
            background-color: rgba(0, 0, 0, 0.8);
            color: white;
            text-align: center;
            padding: 1em 0;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        /* Add a class for the about-me section */
        .about-me-section {
            padding: 2em;
            text-align: center;
            color: white;
            max-width: 800px;
            margin: 0 auto;
            animation: fadeInOut 10s infinite; /* Animation properties */
        }

        .about-me-section p {
            line-height: 1.5;
        }

        @keyframes fadeInOut {
            0%, 100% {
                opacity: 0;
                transform: translateY(-10px);
            }
            50% {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="profile-photo">
            <img src="Hariharapriy.jpg" alt="Your Name">
        </div>
        <h1>R.S.HARIHARAPRIYA</h1>
        <p>Web Developer</p>
    </header>

    <nav>
        <a href="certifications.html">Certifications</a>
        <a href="#about-me-section" onclick="scrollToSection('about-me-section')">About Me</a>
        <a href="education.html">Education</a>
        <!-- Add more navigation links for other sections -->
    </nav>

    <div class="about-me-section" id="about-me-section">
        <h2>About Me</h2>
        <p>"As a dedicated B.E. Computer Science and Engineering student, I am passionate about web development and bring a strong academic background, consistently ranking as a top performer. Eager to leverage my skills and knowledge in pursuing opportunities that align with my enthusiasm for creating innovative and impactful web solutions."</p>
    </div>

    <footer>
        <p>Contact: hariharapriya6@gmail.com | Follow me on <a href="https://www.linkedin.com/public-profile/settings


" target="_blank">LinkedIn</a></p>
    </footer>

    <script>
                function scrollToSection(sectionId) {
            var section = document.getElementById(sectionId);
            window.scrollTo({
                top: section.offsetTop,
                behavior: 'smooth'
            });
        }

        // Code for the slideshow
        var currentSlide = 1;
        setInterval(function() {
            document.getElementById('slide' + currentSlide).classList.remove('active');
            currentSlide = (currentSlide % 3) + 1;
            document.getElementById('slide' + currentSlide).classList.add('active');
        }, 5000);
    </script>

</body>
</html>
