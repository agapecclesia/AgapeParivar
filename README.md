<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Your Church App</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- Link to CSS -->
    <link rel="stylesheet" href="style.css">
    <!-- Google Fonts (Optional) -->
    <link href="https://fonts.googleapis.com/css?family=Nunito:400,700&display=swap" rel="stylesheet">
</head>
<body>

    <!-- Header Section -->
    <header>
        <h1>Your Church Name</h1>
        <p>Welcome to our community!</p>
    </header>

    <!-- Navigation Menu -->
    <nav>
        <ul>
            <li onclick="showPage('home')">Home</li>
            <li onclick="showPage('about')">About Us</li>
            <li onclick="showPage('services')">Services</li>
            <li onclick="showPage('contact')">Contact</li>
            <li onclick="showPage('inspiration')">Daily Inspiration</li>
        </ul>
    </nav>

    <!-- Main Content -->
    <main id="content">
        <!-- Home Page -->
        <section id="home" class="page">
            <h2>Welcome Home</h2>
            <p>We're delighted to have you here. Join us in worship and fellowship.</p>
        </section>

        <!-- About Us Page -->
        <section id="about" class="page">
            <h2>About Us</h2>
            <p>Discover our mission, vision, and the history that shapes us.</p>
        </section>

        <!-- Services Page -->
        <section id="services" class="page">
            <h2>Our Services</h2>
            <ul>
                <li><strong>Sunday Worship:</strong> 10:00 AM</li>
                <li><strong>Bible Study:</strong> Wednesdays at 7:00 PM</li>
                <li><strong>Youth Group:</strong> Fridays at 6:00 PM</li>
                <li><strong>Community Outreach:</strong> Check our calendar for events</li>
            </ul>
        </section>

        <!-- Contact Page -->
        <section id="contact" class="page">
            <h2>Contact Us</h2>
            <form id="contactForm">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="5" required></textarea>

                <button type="submit">Send Message</button>
            </form>
            <p id="formResponse"></p>
        </section>

        <!-- Daily Inspiration Page -->
        <section id="inspiration" class="page">
            <h2>Daily Inspiration</h2>
            <blockquote id="bibleVerse"></blockquote>
            <button onclick="displayVerse()">Get Another Verse</button>
        </section>
    </main>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2023 Your Church Name. All rights reserved.</p>
    </footer>

    <!-- Link to JavaScript -->
    <script src="script.js"></script>
</body>
</html>
