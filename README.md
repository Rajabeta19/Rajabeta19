
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rajvardhan Photography</title>
    <style>
        /* General Styles */
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
        }

        /* Header Section */
        .cover-photo {
            width: 100%;
            height: 60vh;
            background-image: url('cover.jpg'); /* Replace with your cover photo filename */
            background-size: cover;
            background-position: center;
            position: relative;
        }

        .profile-photo {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 5px solid white;
            position: absolute;
            top: 40%;
            left: 50%;
            transform: translate(-50%, -50%);
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);
        }

        .profile-info {
            text-align: center;
            margin-top: 100px;
        }

        .profile-info h1 {
            font-size: 28px;
            margin: 10px 0 5px;
        }

        .profile-info p {
            font-size: 18px;
            color: gray;
        }

        /* Hamburger Menu */
        .menu {
            position: fixed;
            top: 10px;
            left: 10px;
            background-color: #333;
            color: white;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
        }

        .menu div {
            width: 30px;
            height: 4px;
            background-color: white;
            margin: 5px 0;
        }

        /* Sidebar Navigation */
        .sidebar {
            position: fixed;
            top: 0;
            left: -250px;
            width: 250px;
            height: 100%;
            background-color: #333;
            color: white;
            display: flex;
            flex-direction: column;
            padding: 20px;
            box-shadow: 2px 0px 5px rgba(0, 0, 0, 0.5);
            transition: 0.3s;
        }

        .sidebar a {
            text-decoration: none;
            color: white;
            margin: 10px 0;
            font-size: 18px;
        }

        .sidebar a:hover {
            text-decoration: underline;
        }

        .sidebar.open {
            left: 0;
        }

        /* Portfolio Section */
        .portfolio {
            padding: 20px;
            text-align: center;
        }

        .portfolio h2 {
            font-size: 24px;
            margin-bottom: 20px;
        }

        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 10px;
        }

        .portfolio-item {
            background-color: #fff;
            padding: 10px;
            border-radius: 5px;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
            cursor: pointer;
        }

        .portfolio-item:hover {
            box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.2);
        }

        /* Contact Section */
        .contact {
            text-align: center;
            margin-top: 50px;
            padding: 20px;
            background-color: #333;
            color: white;
        }

        .contact a {
            text-decoration: none;
            color: #1DA1F2; /* Instagram blue */
            font-size: 18px;
        }

        .contact a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <!-- Cover Photo Section -->
    <div class="cover-photo"></div>

    <!-- Profile Photo -->
    <img class="profile-photo" src="profile.jpg" alt="Rajvardhan Profile Photo">

    <!-- Profile Info -->
    <div class="profile-info">
        <h1>Rajvardhan Singh</h1>
        <p>Nature and Street Photographer</p>
    </div>

    <!-- Hamburger Menu -->
    <div class="menu" onclick="toggleMenu()">
        <div></div>
        <div></div>
        <div></div>
    </div>

    <!-- Sidebar Navigation -->
    <div class="sidebar" id="sidebar">
        <a href="#about">About</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#contact">Contact</a>
    </div>

    <!-- About Section -->
    <section id="about" class="portfolio">
        <h2>About Me</h2>
        <p>I’m a 27-year-old self-taught photographer from India. I explore different genres like nature, street, black-and-white, minimalism, macro, landscapes, and ancient architecture. My work reflects my journey of finding beauty in the unnoticed.</p>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="portfolio">
        <h2>Portfolio</h2>
        <div class="portfolio-grid">
            <div class="portfolio-item">Nature</div>
            <div class="portfolio-item">Street</div>
            <div class="portfolio-item">Ancient Architecture</div>
            <div class="portfolio-item">Black & White</div>
            <div class="portfolio-item">Minimalism</div>
            <div class="portfolio-item">Macro</div>
            <div class="portfolio-item">Landscapes</div>
            <div class="portfolio-item">More...</div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <p>Follow me on Instagram: <a href="https://www.instagram.com/yourprofile/" target="_blank">yourprofile</a></p>
        <p>Email me: <a href="mailto:yourname@gmail.com">yourname@gmail.com</a></p>
    </section>

    <!-- JavaScript -->
    <script>
        function toggleMenu() {
            const sidebar = document.getElementById('sidebar');
            sidebar.classList.toggle('open');
        }
    </script>
</body>
</html>
<!---
Rajabeta19/Rajabeta19 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
