<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Guardians - Protecting Our Water Resources</title>
    
    <!-- CSS STYLES -->
    <style>
        /* Reset and base styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        
        body {
            background-color: #f0f8ff;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header styles */
        header {
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }
        
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #1e90ff;
            text-decoration: none;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 2rem;
        }
        
        .nav-links a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            cursor: pointer;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            transition: all 0.3s ease;
        }
        
        .nav-links a:hover, .nav-links a.active {
            background: #e6f2ff;
            color: #1e90ff;
        }
        
        /* Page styles */
        .page {
            display: none;
        }
        
        .page.active {
            display: block;
        }
        
        /* Hero section */
        .hero {
            background: linear-gradient(rgba(30, 144, 255, 0.8), rgba(30, 144, 255, 0.9)), 
                        url('https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 70vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: white;
            margin-top: 70px;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            background: #1e90ff;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            background: #0077e6;
            transform: translateY(-2px);
        }
        
        /* Content sections */
        section {
            padding: 4rem 0;
        }
        
        h2 {
            text-align: center;
            margin-bottom: 2rem;
            color: #1e90ff;
            font-size: 2.5rem;
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 3rem;
        }
        
        .about-text, .about-image {
            flex: 1;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        /* Issues grid */
        .issues-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .issue-card {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            text-align: center;
        }
        
        .issue-card h3 {
            color: #1e90ff;
            margin: 1rem 0;
        }
        
        /* Footer */
        footer {
            background: #333;
            color: white;
            padding: 3rem 0 1rem;
            text-align: center;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-between;
            margin-bottom: 2rem;
        }
        
        .footer-column {
            flex: 1;
            text-align: left;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 0.5rem;
        }
        
        .footer-links a {
            color: #ccc;
            text-decoration: none;
            cursor: pointer;
        }
        
        .footer-links a:hover {
            color: white;
        }
        
        .copyright {
            border-top: 1px solid #555;
            padding-top: 1rem;
            color: #aaa;
        }
        
        /* Responsive design */
        @media (max-width: 768px) {
            .about-content {
                flex-direction: column;
            }
            
            .footer-content {
                flex-direction: column;
                gap: 2rem;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- HTML CONTENT -->
    <header>
        <div class="container">
            <nav>
                <a class="logo" onclick="showPage('home')">💧 Water Guardians</a>
                <ul class="nav-links">
                    <li><a class="nav-link active" onclick="showPage('home')">Home</a></li>
                    <li><a class="nav-link" onclick="showPage('about')">About</a></li>
                    <li><a class="nav-link" onclick="showPage('issues')">Issues</a></li>
                    <li><a class="nav-link" onclick="showPage('solutions')">Solutions</a></li>
                    <li><a class="nav-link" onclick="showPage('action')">Take Action</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Home Page -->
    <div id="home" class="page active">
        <section class="hero">
            <div class="container">
                <div class="hero-content">
                    <h1>Protecting Our Water Resources</h1>
                    <p>Join the movement to safeguard our rivers, lakes, and oceans for future generations</p>
                    <a class="btn" onclick="showPage('action')">Become a Water Guardian</a>
                </div>
            </div>
        </section>

        <section class="about">
            <div class="container">
                <h2>About Water Guardians</h2>
                <div class="about-content">
                    <div class="about-text">
                        <p>Water Guardians is a global initiative dedicated to protecting and preserving our planet's most vital resource: water.</p>
                        <p>Our mission is to ensure clean, accessible water for all while protecting aquatic ecosystems from pollution and climate change impacts.</p>
                        <a class="btn" onclick="showPage('about')">Learn More</a>
                    </div>
                    <div class="about-image">
                        <img src="https://images.unsplash.com/photo-1559827260-dc66d52bef19?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Clean water">
                    </div>
                </div>
            </div>
        </section>

        <section class="issues" style="background: #e6f2ff;">
            <div class="container">
                <h2>Water Challenges</h2>
                <div class="issues-grid">
                    <div class="issue-card">
                        <h3>💧 Water Scarcity</h3>
                        <p>2+ billion people face water stress globally due to climate change and population growth.</p>
                    </div>
                    <div class="issue-card">
                        <h3>🏭 Pollution</h3>
                        <p>Industrial waste and plastic pollution threaten marine life and water quality.</p>
                    </div>
                    <div class="issue-card">
                        <h3>🌡️ Climate Impact</h3>
                        <p>Changing weather patterns disrupt water cycles and threaten freshwater sources.</p>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- About Page -->
    <div id="about" class="page">
        <section class="hero" style="background: linear-gradient(rgba(30, 144, 255, 0.8), rgba(30, 144, 255, 0.9)); margin-top: 70px;">
            <div class="container">
                <h1>About Our Mission</h1>
            </div>
        </section>
        
        <section class="about">
            <div class="container">
                <div class="about-content">
                    <div class="about-text">
                        <h2>Our Story</h2>
                        <p>Founded in 2020, Water Guardians began as a community initiative to protect local water sources and has grown into a global movement.</p>
                        <p>We work through education, advocacy, and community action to create lasting change in water conservation and protection.</p>
                        <h2>Our Impact</h2>
                        <p>• 150+ community monitoring programs established</p>
                        <p>• 5,000+ volunteers trained in water quality testing</p>
                        <p>• 200+ pollution sources identified and addressed</p>
                    </div>
                    <div class="about-image">
                        <img src="https://images.unsplash.com/photo-1586773860418-d37222d8fce3?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Water testing">
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Issues Page -->
    <div id="issues" class="page">
        <section class="hero" style="background: linear-gradient(rgba(30, 144, 255, 0.8), rgba(30, 144, 255, 0.9)); margin-top: 70px;">
            <div class="container">
                <h1>Water Challenges</h1>
            </div>
        </section>
        
        <section class="about">
            <div class="container">
                <h2>Major Water Issues</h2>
                <div class="issues-grid">
                    <div class="issue-card">
                        <h3>Water Scarcity</h3>
                        <p>Climate change, population growth, and inefficient water use are creating water stress for billions of people worldwide.</p>
                    </div>
                    <div class="issue-card">
                        <h3>Pollution</h3>
                        <p>Industrial waste, agricultural runoff, and plastic pollution contaminate water sources and harm ecosystems.</p>
                    </div>
                    <div class="issue-card">
                        <h3>Climate Impact</h3>
                        <p>Rising temperatures and changing precipitation patterns threaten water availability and quality.</p>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Solutions Page -->
    <div id="solutions" class="page">
        <section class="hero" style="background: linear-gradient(rgba(30, 144, 255, 0.8), rgba(30, 144, 255, 0.9)); margin-top: 70px;">
            <div class="container">
                <h1>Our Solutions</h1>
            </div>
        </section>
        
        <section class="about">
            <div class="container">
                <h2>How We're Making a Difference</h2>
                <div class="issues-grid">
                    <div class="issue-card">
                        <h3>Community Monitoring</h3>
                        <p>Empowering local communities to test water quality and report pollution issues.</p>
                    </div>
                    <div class="issue-card">
                        <h3>Conservation Programs</h3>
                        <p>Implementing water-saving technologies and practices in communities and agriculture.</p>
                    </div>
                    <div class="issue-card">
                        <h3>Policy Advocacy</h3>
                        <p>Working with governments to strengthen water protection regulations and policies.</p>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Action Page -->
    <div id="action" class="page">
        <section class="hero" style="background: linear-gradient(rgba(30, 144, 255, 0.8), rgba(30, 144, 255, 0.9)); margin-top: 70px;">
            <div class="container">
                <h1>Take Action</h1>
            </div>
        </section>
        
        <section class="about">
            <div class="container">
                <h2>Join Our Movement</h2>
                <div class="issues-grid">
                    <div class="issue-card">
                        <h3>Volunteer</h3>
                        <p>Join community monitoring programs or participate in cleanup events.</p>
                        <a class="btn" style="margin-top: 1rem;">Sign Up</a>
                    </div>
                    <div class="issue-card">
                        <h3>Donate</h3>
                        <p>Support our work funding water testing kits and educational materials.</p>
                        <a class="btn" style="margin-top: 1rem;">Donate Now</a>
                    </div>
                    <div class="issue-card">
                        <h3>Advocate</h3>
                        <p>Contact representatives about water policies or start a local chapter.</p>
                        <a class="btn" style="margin-top: 1rem;">Take Action</a>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Water Guardians</h3>
                    <p>Protecting water resources through education, advocacy, and community action.</p>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul class="footer-links">
                        <li><a onclick="showPage('home')">Home</a></li>
                        <li><a onclick="showPage('about')">About</a></li>
                        <li><a onclick="showPage('issues')">Issues</a></li>
                        <li><a onclick="showPage('solutions')">Solutions</a></li>
                        <li><a onclick="showPage('action')">Take Action</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Contact</h3>
                    <p>info@waterguardians.org</p>
                    <p>+1 (555) 123-4567</p>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2025 Water Guardians. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- JAVASCRIPT -->
    <script>
        // Page navigation function
        function showPage(pageId) {
            // Hide all pages
            document.querySelectorAll('.page').forEach(page => {
                page.classList.remove('active');
            });
            
            // Show the selected page
            document.getElementById(pageId).classList.add('active');
            
            // Update active nav link
            document.querySelectorAll('.nav-link').forEach(link => {
                link.classList.remove('active');
            });
            
            // Find and activate the corresponding nav link
            document.querySelectorAll('.nav-link').forEach(link => {
                if (link.textContent.trim().toLowerCase().includes(pageId) || 
                    (pageId === 'home' && link.textContent.trim().toLowerCase() === 'home')) {
                    link.classList.add('active');
                }
            });
            
            // Scroll to top when changing pages
            window.scrollTo(0, 0);
        }
        
        // Header background change on scroll
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if(window.scrollY > 50) {
                header.style.backgroundColor = 'rgba(255, 255, 255, 0.95)';
            } else {
                header.style.backgroundColor = 'white';
            }
        });
    </script>
</body>
</html>
