# P<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>P.A Mwaura Analytics Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</head>
<body>
    <header>
        <h1>P.A Mwaura Analytics Ltd</h1>
        <p class="motto">"Transforming Data into Insights"</p>
    </header>
    <nav>
        <a href="#projects">Projects</a>
        <a href="#about">About Me</a>
        <a href="#vision">Vision & Motto</a>
        <a href="#contact">Contact</a>
    </nav>
    <main>
        <section id="vision">
            <h2>Vision & Motto</h2>
            <p id="vision-text">My vision is to empower businesses and individuals to harness the power of data for better decision-making.</p>
            <button id="change-vision">See More</button>
        </section>
        <section id="projects">
            <h2>Projects</h2>
            <canvas id="dashboard" width="400" height="200"></canvas>
        </section>
        <section id="about">
            <h2>About Me</h2>
            <p>
                Hi, I'm Andrew Mwaura, a data scientist with 3 years of experience in R, MySQL, Tableau, Python, web scraping, and predictive modeling.
                My expertise lies in building analytics solutions and delivering actionable insights.
            </p>
        </section>
        <section id="contact">
            <h2>Contact</h2>
            <p>Email: <a href="mailto:andrewpmwaura047@gmail.com">andrewpmwaura047@gmail.com</a></p>
            <p>Phone: 0791560500</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 P.A Mwaura Analytics Ltd. Built with passion for data.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>A.Mwaura-analytics-ltd  

/* styles.css */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    color: #333;
    background-color: #f4f4f9;
}

header {
    background: linear-gradient(90deg, #333, #555);
    color: #fff;
    padding: 20px 0;
    text-align: center;
}

header .motto {
    font-style: italic;
    font-size: 1.2em;
}

nav {
    display: flex;
    justify-content: center;
    background: #444;
    padding: 10px 0;
}

nav a {
    color: #fff;
    text-decoration: none;
    margin: 0 15px;
    padding: 5px 10px;
    border-radius: 5px;
}

nav a:hover {
    background: #555;
    color: #fff;
}

main {
    padding: 20px;
}

h2 {
    color: #444;
    margin-bottom: 10px;
}

button {
    padding: 10px 15px;
    background-color: #007bff;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}

footer {
    text-align: center;
    padding: 10px;
    background: #333;
    color: #fff;
    margin-top: 20px;
}
