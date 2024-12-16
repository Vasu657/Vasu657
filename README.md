```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vasu Ghanta - GitHub Profile</title>
    <style>
        :root {
            --bg-light: #f9f9f9;
            --text-light: #333;
            --bg-dark: #121212;
            --text-dark: #f9f9f9;
        }

        body {
            margin: 0;
            font-family: Arial, sans-serif;
            transition: background-color 0.3s, color 0.3s;
        }

        .light-mode {
            background-color: var(--bg-light);
            color: var(--text-light);
        }

        .dark-mode {
            background-color: var(--bg-dark);
            color: var(--text-dark);
        }

        header {
            padding: 20px;
            text-align: center;
        }

        h1 {
            margin: 0;
            font-size: 2rem;
        }

        .theme-toggle {
            margin: 20px;
            cursor: pointer;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            background: #007bff;
            color: white;
            font-size: 1rem;
            transition: background-color 0.3s;
        }

        .theme-toggle:hover {
            background-color: #0056b3;
        }

        .content {
            max-width: 800px;
            margin: auto;
            padding: 20px;
            line-height: 1.6;
        }

        .section {
            margin-bottom: 20px;
        }

        .section h2 {
            border-bottom: 2px solid currentColor;
            padding-bottom: 5px;
        }

        footer {
            text-align: center;
            padding: 20px;
            margin-top: 20px;
            font-size: 0.9rem;
        }
    </style>
</head>
<body class="light-mode">
    <header>
        <h1>Hi, I'm Vasu Ghanta 👋</h1>
        <button class="theme-toggle" onclick="toggleTheme()">Switch to Dark Mode</button>
    </header>
    <div class="content">
        <div class="section">
            <h2>About Me 🌟</h2>
            <p>👨‍💻 <strong>Current Role</strong>: Data Analyst at Darien Software Systems (Bangalore)</p>
            <p>🌟 <strong>Professional Summary</strong>: Skilled in data cleansing, visualization, and automation workflows using tools like <strong>Excel</strong>, <strong>SQL</strong>, <strong>Power BI</strong>, and <strong>Python</strong>.</p>
            <p>🎓 <strong>Education</strong>: Bachelor of Engineering in Computer Science from Jain Institute of Technology (VTU)</p>
        </div>

        <div class="section">
            <h2>Tools and Technologies ⚒️</h2>
            <ul>
                <li><strong>Excel</strong>: Advanced Formulas, Pivot Tables, Power Query</li>
                <li><strong>SQL</strong>: Query Optimization, Joins, Subqueries</li>
                <li><strong>Power BI</strong>: DAX, Interactive Dashboards</li>
                <li><strong>Python</strong>: Data Analysis (Pandas, NumPy), Visualization (Matplotlib)</li>
                <li><strong>AWS</strong>: EC2, S3, IAM, and more</li>
                <li><strong>Linux</strong>: Server Administration, Scripting</li>
            </ul>
        </div>

        <div class="section">
            <h2>Interests and Hobbies 🎨</h2>
            <ul>
                <li>🌍 Exploring cloud-based solutions</li>
                <li>📊 Creating interactive dashboards and data visualizations</li>
                <li>🎮 Gaming and exploring new tech trends</li>
                <li>🖌️ Sketching and graphic design</li>
            </ul>
        </div>

        <div class="section">
            <h2>Web Presence 🌐</h2>
            <ul>
                <li>📧 <a href="mailto:vasughanta2k@gmail.com">Email</a></li>
                <li>🔗 <a href="https://www.linkedin.com/in/vasu-ghanta">LinkedIn</a></li>
                <li>🌐 <a href="https://vasu-ghanta.web.app/">Personal Website</a></li>
            </ul>
        </div>
    </div>
    <footer>
        &copy; 2024 Vasu Ghanta. Built with ❤️ for GitHub.
    </footer>

    <script>
        function toggleTheme() {
            const body = document.body;
            const button = document.querySelector('.theme-toggle');
            if (body.classList.contains('light-mode')) {
                body.classList.remove('light-mode');
                body.classList.add('dark-mode');
                button.textContent = 'Switch to Light Mode';
            } else {
                body.classList.remove('dark-mode');
                body.classList.add('light-mode');
                button.textContent = 'Switch to Dark Mode';
            }
        }
    </script>
</body>
</html>
```
