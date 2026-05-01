
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Prajakta Thete | Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;800&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #3b82f6;
            --dark: #0f172a;
            --glass: rgba(30, 41, 59, 0.75);
            --white: #f8fafc;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--dark);
            color: var(--white);
            line-height: 1.6;
        }

        /* --- BLURRED FIXED BACKGROUND --- */
        .bg-overlay {
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: linear-gradient(rgba(15, 23, 42, 0.7), rgba(15, 23, 42, 0.9)), 
                        url('prajakta.jpg'); /* Your image */
            background-size: cover;
            background-position: center 20%;
            filter: blur(8px); /* Professional blur */
            transform: scale(1.1); /* Prevents white edges from blur */
            z-index: -1;
        }

        /* --- NAVIGATION --- */
        nav {
            position: fixed;
            top: 0; width: 100%;
            display: flex; justify-content: space-between; align-items: center;
            padding: 20px 8%;
            background: rgba(15, 23, 42, 0.85);
            backdrop-filter: blur(15px);
            z-index: 1000;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .logo { font-family: 'Plus Jakarta Sans'; font-weight: 800; color: var(--primary); font-size: 1.2rem; }

        nav ul { display: flex; list-style: none; gap: 25px; }
        nav ul li a {
            color: #94a3b8;
            text-decoration: none;
            font-size: 0.8rem;
            font-weight: 600;
            text-transform: uppercase;
            transition: 0.3s;
        }
        nav ul li a:hover { color: var(--primary); }

        /* --- HERO SECTION --- */
        .hero {
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 10%;
        }

        .hero h1 {
            font-family: 'Plus Jakarta Sans';
            font-size: clamp(2.5rem, 8vw, 5rem);
            font-weight: 800;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1.1rem;
            letter-spacing: 4px;
            color: var(--primary);
            text-transform: uppercase;
            font-weight: 700;
        }

        /* --- ABOUT SECTION WITH RIGHT IMAGE --- */
        section {
            padding: 80px 10%;
            max-width: 1300px;
            margin: 0 auto;
        }

        .glass-card {
            background: var(--glass);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            padding: 50px;
            border-radius: 20px;
            display: flex;
            gap: 40px;
            align-items: center;
        }

        .about-text { flex: 2; }
        .about-image { flex: 1; text-align: center; }

        .about-image img {
            width: 100%;
            max-width: 280px;
            border-radius: 15px;
            border: 3px solid var(--primary);
            box-shadow: 0 20px 40px rgba(0,0,0,0.4);
        }

        h2 { font-family: 'Plus Jakarta Sans'; font-size: 2.2rem; color: var(--primary); margin-bottom: 20px; }

        /* --- RESUME/SKILLS GRID --- */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .info-box {
            background: rgba(255, 255, 255, 0.05);
            padding: 25px;
            border-radius: 12px;
            border-left: 4px solid var(--primary);
        }

        .btn {
            background: var(--primary);
            color: white;
            padding: 12px 30px;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 700;
            display: inline-block;
            margin-top: 20px;
            transition: 0.3s;
        }
        .btn:hover { background: white; color: var(--dark); transform: translateY(-3px); }

        footer { text-align: center; padding: 40px; color: #64748b; font-size: 0.9rem; }

        @media (max-width: 900px) {
            .glass-card { flex-direction: column; text-align: center; }
            nav ul { display: none; }
        }
    </style>
</head>
<body>

    <div class="bg-overlay"></div>

    <nav>
        <div class="logo">PRAJAKTA THETE</div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About Me</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <header class="hero" id="home">
        <p>Student of MCS 1</p>
        <h1>Prajakta Prakash Thete</h1>
        <a href="#contact" class="btn">Get In Touch</a>
    </header>

    <section id="about">
        <div class="glass-card">
            <div class="about-text">
                <h2>About Me</h2>
                <p>I am a highly motivated Computer Science student currently in my first year of <strong>Master of Computer Science (MCS)</strong>. I have a strong foundation in both backend and frontend development, along with database management. I am passionate about coding and building modern web applications that solve real-world problems.</p>
                <a href="prajakta resume.jpeg" download class="btn">Download Resume</a>
            </div>
            <div class="about-image">
                <img src="prajakta.jpg" alt="Prajakta Thete"> </div>
        </div>
    </section>

    <section id="education">
        <h2 style="text-align: center; margin-bottom: 40px;">Education & Skills</h2>
        <div class="grid">
            <div class="info-box">
                <h3>BSc Computer Science</h3>
                <p>K. K. Wagh College, SPPU University</p>
                <p><strong>3rd Year: 83%</strong> (2024-2025)</p>
            </div>
            <div class="info-box">
                <h3>Technical Skills</h3>
                <p>Python, Java, C Programming, SQL, HTML/CSS</p>
                <p>Digital Branding & Logo Design</p>
            </div>
            <div class="info-box">
                <h3>Projects</h3>
                <p><strong>Online Car Rental System</strong></p>
                <p>Digital Branding for Suman Hitech Nursery</p>
            </div>
        </div>
    </section>

    <section id="contact" style="text-align: center;">
        <div class="glass-card" style="display: block;">
            <h2>Contact Details</h2>
            <p><strong>Phone:</strong> 7775878209</p>
            <p><strong>Email:</strong> prajaktathete10@gmail.com</p>
            <p><strong>Location:</strong> Palkhed, Niphad, Nashik</p>
        </div>
    </section>

    <footer>
        &copy; 2026 Prajakta Thete | Developed with Professional CSS
    </footer>

</body>
</html>
