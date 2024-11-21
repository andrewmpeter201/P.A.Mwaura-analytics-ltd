<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>P.A Mwaura Analytics Portfolio</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
            background: url('https://images.unsplash.com/photo-1504384308090-c894fdcc538d?fit=crop&w=1600&q=80') no-repeat center center fixed;
            background-size: cover;
        }

        header {
            background: rgba(0, 0, 0, 0.7);
            color: #fff;
            text-align: center;
            padding: 20px 0;
        }

        header h1 {
            font-size: 2.5em;
        }

        header .motto {
            font-style: italic;
            font-size: 1.2em;
        }

        nav {
            display: flex;
            justify-content: center;
            background: rgba(0, 0, 0, 0.8);
            padding: 10px;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 15px;
            padding: 10px 15px;
            border-radius: 5px;
            transition: background 0.3s ease;
        }

        nav a:hover {
            background: #007bff;
        }

        main {
            padding: 20px;
            background: rgba(255, 255, 255, 0.9);
            margin: 20px auto;
            max-width: 1000px;
            border-radius: 10px;
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
            transition: background 0.3s ease;
        }

        button:hover {
            background-color: #0056b3;
        }

        footer {
            text-align: center;
            padding: 10px;
            background: rgba(0, 0, 0, 0.8);
            color: #fff;
            margin-top: 20px;
        }

        .comment-box, .review-box, .question-box {
            margin-top: 20px;
        }

        .comment-box textarea,
        .question-box textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .reviews {
            background: #f9f9f9;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-bottom: 10px;
        }

        .reviews p {
            margin: 5px 0;
        }
    </style>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</head>
<body>
    <!-- Header Section -->
    <header>
        <h1>P.A Mwaura Analytics Ltd</h1>
        <p class="motto">"Transforming Data into Insights"</p>
    </header>

    <!-- Navigation Menu -->
    <nav>
        <a href="#projects">Projects</a>
        <a href="#about">About Me</a>
        <a href="#vision">Vision</a>
        <a href="#reviews">Reviews</a>
        <a href="#comments">Comments</a>
        <a href="#questions">Questions</a>
        <a href="#contact">Contact</a>
    </nav>

    <!-- Main Content -->
    <main>
        <!-- Vision Section -->
        <section id="vision">
            <h2>Vision</h2>
            <p id="vision-text">My vision is to empower businesses and individuals to harness the power of data for better decision-making.</p>
            <button id="change-vision">See More</button>
        </section>

        <!-- Projects Section -->
        <section id="projects">
            <h2>Projects</h2>
            <canvas id="dashboard" width="400" height="200"></canvas>
        </section>

        <!-- About Me Section -->
        <section id="about">
            <h2>About Me</h2>
            <p>
                Hi, I'm Andrew Mwaura, a data scientist with 3 years of experience in R, MySQL, Tableau, Python, web scraping, and predictive modeling.
                My expertise lies in building analytics solutions and delivering actionable insights.
            </p>
        </section>

        <!-- Reviews Section -->
        <section id="reviews">
            <h2>Reviews</h2>
            <div class="reviews">
                <p><strong>John Doe:</strong> "Fantastic work, highly recommend!"</p>
            </div>
            <div class="reviews">
                <p><strong>Jane Smith:</strong> "Delivered great insights for my business."</p>
            </div>
        </section>

        <!-- Comments Section -->
        <section id="comments">
            <h2>Leave a Comment</h2>
            <div class="comment-box">
                <textarea placeholder="Write your comment here..." rows="5"></textarea>
                <button>Submit Comment</button>
            </div>
        </section>

        <!-- Questions Section -->
        <section id="questions">
            <h2>Ask a Question</h2>
            <div class="question-box">
                <textarea placeholder="Write your question here..." rows="5"></textarea>
                <button>Submit Question</button>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact">
            <h2>Contact</h2>
            <p>Email: <a href="mailto:andrewpmwaura047@gmail.com">andrewpmwaura047@gmail.com</a></p>
            <p>Phone: 0791560500</p>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 P.A Mwaura Analytics Ltd. Built with passion for data.</p>
    </footer>

    <!-- JavaScript -->
    <script>
        // Chart for Projects
        const ctx = document.getElementById('dashboard').getContext('2d');
        const myChart = new Chart(ctx, {
            type: 'bar',
            data: {
                labels: ['Project 1', 'Project 2', 'Project 3', 'Project 4'],
                datasets: [{
                    label: 'Complexity Level',
                    data: [12, 19, 3, 5],
                    backgroundColor: [
                        'rgba(255, 99, 132, 0.2)',
                        'rgba(54, 162, 235, 0.2)',
                        'rgba(255, 206, 86, 0.2)',
                        'rgba(75, 192, 192, 0.2)'
                    ],
                    borderColor: [
                        'rgba(255, 99, 132, 1)',
                        'rgba(54, 162, 235, 1)',
                        'rgba(255, 206, 86, 1)',
                        'rgba(75, 192, 192, 1)'
                    ],
                    borderWidth: 1
                }]
            },
            options: {
                scales: {
                    y: {
                        beginAtZero: true
                    }
                }
            }
        });

        // Interactive Vision Section
        document.getElementById('change-vision').addEventListener('click', function() {
            const visionText = document.getElementById('vision-text');
            visionText.textContent = "To be the go-to analytics provider for turning complex data into meaningful solutions.";
        });
    </script>
</body>
</html>
