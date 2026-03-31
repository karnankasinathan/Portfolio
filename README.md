# Ex01 Portfolio


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
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            background-color: #f9f9f9;
            color: #333;
            margin: 0;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background-color: #fff;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }

        header {
            text-align: center;
            border-bottom: 1px solid #eee;
            padding-bottom: 20px;
            margin-bottom: 30px;
        }

        header img.profile-pic {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 15px;
            border: 3px solid #eee;
        }

        header h1 {
            margin: 0;
            font-size: 2.5rem;
            color: #2c3e50;
        }

        header p {
            margin: 5px 0 0;
            font-size: 1.2rem;
            color: #7f8c8d;
        }

        section {
            margin-bottom: 40px;
        }

        h2 {
            font-size: 1.8rem;
            color: #34495e;
            border-bottom: 2px solid #3498db;
            padding-bottom: 10px;
            margin-bottom: 20px;
        }

        .content-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .content-item {
            background-color: #fdfdfd;
            border: 1px solid #eee;
            border-radius: 5px;
            padding: 20px;
            flex: 1 1 45%;
            min-width: 280px;
            transition: box-shadow 0.3s ease;
        }

        .content-item:hover {
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
        }

        .content-item h3 {
            margin-top: 0;
            color: #3498db;
        }

        .contact-info a {
            color: #3498db;
            text-decoration: none;
            font-weight: 500;
        }

        .contact-info a:hover {
            text-decoration: underline;
        }

        footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #eee;
            font-size: 0.9rem;
            color: #95a5a6;
        }

        /* Navigation Styles */
        nav {
            text-align: center;
            margin-bottom: 30px;
        }
        nav button {
            background: none;
            border: none;
            font-size: 1.1rem;
            margin: 0 15px;
            cursor: pointer;
            color: #7f8c8d;
            padding-bottom: 5px;
            transition: color 0.3s;
        }
        nav button:hover, nav button.active {
            color: #3498db;
            border-bottom: 2px solid #3498db;
        }
        .page-section {
            display: none;
            animation: fadeIn 0.5s;
        }
        .page-section.active {
            display: block;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    </style>
</head>
<body>

    <div class="container">

        <header>
            <img src="212222230062.jpeg" alt="Profile Picture" class="profile-pic">
            <h1>KARNAN K</h1>
            <p>B.Tech | AI & DS</p>
        </header>
        
        <nav>
            <button class="active" onclick="showPage('home', this)">Home</button>
            <button onclick="showPage('about', this)">About Me</button>
            <button onclick="showPage('contact', this)">Contact Me</button>
        </nav>

        <section id="home" class="page-section active">
            <h2>Welcome</h2>
            <p>
                I am a B.Tech student in <strong>Artificial Intelligence & Data Science</strong>
                <p>This portfolio shows my skills, interests, and learning journey.</p>
            </p>
        </section>

        <section id="about" class="page-section">
            <h2>About Me</h2>
            <div class="content-grid">
                <div class="content-item">
                    <p>
        I am a passionate AI & DS student with a strong
        interest in technology and development.<br><br>

        ✔ Learning Web Development<br>
        ✔ Learning Game Development<br>
    </p>
                </div>
            </div>
        </section>

        <section id="contact" class="page-section">
            <h2>Contact Me</h2>
            <p class="contact-info">
                <b>Email:</b> vishwa4513@gmail.com</p>
    <p><b>LinkedIn:</b> linkedin.com/in/Karnankasi
            </p>
        </section>

        <footer>
            <p>&copy; 2026 ៚ karnan. All rights reserved.</p>
        </footer>

    </div>

    <script>
        function showPage(pageId, btn) {
            
            document.querySelectorAll('.page-section').forEach(section => section.classList.remove('active'));
            document.querySelectorAll('nav button').forEach(button => button.classList.remove('active'));

            document.getElementById(pageId).classList.add('active');
            btn.classList.add('active');
        }
    </script>
</body>
</html>

```

## OUTPUT

<img width="1141" height="768" alt="Screenshot 2026-03-14 194226" src="https://github.com/user-attachments/assets/19f38286-0a30-453b-adf4-b039473da740" />


<img width="1156" height="793" alt="Screenshot 2026-03-14 194249" src="https://github.com/user-attachments/assets/df6cdf0e-98f0-4f70-b8ad-809fb8210321" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
