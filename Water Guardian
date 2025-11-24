<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Guardians - Protecting Our Water Resources</title>
    <style>
        /* Base Styles */
        :root {
            --primary: #1a73e8;
            --secondary: #34a853;
            --accent: #4285f4;
            --light: #f8f9fa;
            --dark: #202124;
            --text: #333333;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--text);
            background-color: #f5f7fa;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        section {
            padding: 80px 0;
        }
        
        h1, h2, h3 {
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        h1 {
            font-size: 3rem;
            font-weight: 700;
        }
        
        h2 {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        
        h2:after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background-color: var(--primary);
            border-radius: 2px;
        }
        
        p {
            margin-bottom: 20px;
            font-size: 1.1rem;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            background-color: var(--primary);
            color: white;
            text-decoration: none;
            border-radius: 30px;
            font-weight: 600;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            background-color: var(--accent);
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        /* Header Styles */
        header {
            background-color: white;
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
            padding: 20px 0;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: color 0.3s ease;
        }
        
        .nav-links a:hover {
            color: var(--primary);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), 
                        url('https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: white;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            color: white;
            font-size: 3.5rem;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 1.3rem;
            margin-bottom: 30px;
        }
        
        /* About Section */
        .about {
            background-color: white;
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        .about-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        /* Issues Section */
        .issues {
            background-color: #f0f7ff;
        }
        
        .issues-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .issue-card {
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }
        
        .issue-card:hover {
            transform: translateY(-10px);
        }
        
        .issue-card h3 {
            color: var(--primary);
            margin-bottom: 15px;
        }
        
        .issue-icon {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        /* Solutions Section */
        .solutions {
            background-color: white;
        }
        
        .solution-item {
            display: flex;
            align-items: center;
            margin-bottom: 50px;
            gap: 30px;
        }
        
        .solution-item:nth-child(even) {
            flex-direction: row-reverse;
        }
        
        .solution-text {
            flex: 1;
        }
        
        .solution-image {
            flex: 1;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }
        
        .solution-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        /* Action Section */
        .action {
            background-color: var(--primary);
            color: white;
            text-align: center;
        }
        
        .action h2 {
            color: white;
        }
        
        .action h2:after {
            background-color: white;
        }
        
        .action p {
            max-width: 800px;
            margin: 0 auto 30px;
        }
        
        .action .btn {
            background-color: white;
            color: var(--primary);
        }
        
        .action .btn:hover {
            background-color: #f0f0f0;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-between;
            margin-bottom: 40px;
        }
        
        .footer-column {
            flex: 1;
            margin-right: 30px;
        }
        
        .footer-column:last-child {
            margin-right: 0;
        }
        
        .footer-column h3 {
            color: white;
            margin-bottom: 20px;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: #ddd;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-links a:hover {
            color: white;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 0.9rem;
            color: #aaa;
        }
        
        /* Page Content Styles */
        .page-content {
            padding-top: 100px;
            min-height: calc(100vh - 200px);
        }
        
        .page-hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), 
                        var(--hero-image);
            background-size: cover;
            background-position: center;
            height: 50vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: white;
            margin-bottom: 50px;
        }
        
        .page-hero h1 {
            color: white;
            font-size: 3rem;
        }
        
        .content-section {
            margin-bottom: 60px;
        }
        
        .content-section h2 {
            text-align: left;
        }
        
        .content-section h2:after {
            left: 0;
            transform: none;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            h2 {
                font-size: 2rem;
            }
            
            .about-content,
            .solution-item {
                flex-direction: column;
            }
            
            .solution-item:nth-child(even) {
                flex-direction: column;
            }
            
            .footer-content {
                flex-direction: column;
            }
            
            .footer-column {
                margin-right: 0;
                margin-bottom: 30px;
            }
            
            .nav-links {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <a href="index.html" class="logo">Water Guardians</a>
                <ul class="nav-links">
                    <li><a href="index.html">Home</a></li>
                    <li><a href="about.html">About</a></li>
                    <li><a href="issues.html">Issues</a></li>
                    <li><a href="solutions.html">Solutions</a></li>
                    <li><a href="action.html">Take Action</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>Protecting Our Precious Water Resources</h1>
                <p>Join the movement to safeguard our rivers, lakes, and oceans for future generations. Together, we can ensure clean, accessible water for all.</p>
                <a href="action.html" class="btn">Become a Water Guardian</a>
            </div>
        </div>
    </section>

    <!-- About Preview Section -->
    <section id="about" class="about">
        <div class="container">
            <h2>About Water Guardians</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>Water Guardians is a global initiative dedicated to protecting and preserving our planet's most vital resource: water. Founded in 2020, our organization brings together scientists, activists, and concerned citizens to address the growing threats to our water systems.</p>
                    <p>Our mission is to ensure that every person has access to clean, safe drinking water while protecting aquatic ecosystems from pollution, overuse, and climate change impacts.</p>
                    <a href="about.html" class="btn">Learn More About Us</a>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1559827260-dc66d52bef19?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Clean water source">
                </div>
            </div>
        </div>
    </section>

    <!-- Issues Preview Section -->
    <section id="issues" class="issues">
        <div class="container">
            <h2>Water Challenges We Face</h2>
            <div class="issues-grid">
                <div class="issue-card">
                    <div class="issue-icon">💧</div>
                    <h3>Water Scarcity</h3>
                    <p>More than 2 billion people live in countries experiencing high water stress. Climate change, population growth, and inefficient water use are exacerbating this crisis.</p>
                    <a href="issues.html#scarcity" class="btn" style="margin-top: 15px; padding: 8px 20px; font-size: 0.9rem;">Read More</a>
                </div>
                <div class="issue-card">
                    <div class="issue-icon">🏭</div>
                    <h3>Pollution</h3>
                    <p>Industrial waste, agricultural runoff, and plastic pollution are contaminating our water sources at an alarming rate, harming marine life and entering our food chain.</p>
                    <a href="issues.html#pollution" class="btn" style="margin-top: 15px; padding: 8px 20px; font-size: 0.9rem;">Read More</a>
                </div>
                <div class="issue-card">
                    <div class="issue-icon">🌡️</div>
                    <h3>Climate Impact</h3>
                    <p>Climate change is disrupting water cycles worldwide, causing more frequent and severe droughts, floods, and storms that threaten freshwater sources.</p>
                    <a href="issues.html#climate" class="btn" style="margin-top: 15px; padding: 8px 20px; font-size: 0.9rem;">Read More</a>
                </div>
            </div>
            <div style="text-align: center; margin-top: 40px;">
                <a href="issues.html" class="btn">View All Water Issues</a>
            </div>
        </div>
    </section>

    <!-- Solutions Preview Section -->
    <section id="solutions" class="solutions">
        <div class="container">
            <h2>Our Solutions</h2>
            <div class="solution-item">
                <div class="solution-text">
                    <h3>Community Water Monitoring</h3>
                    <p>We empower local communities to monitor their water sources through our citizen science programs. Volunteers are trained to test water quality, identify pollution sources, and report issues to authorities.</p>
                    <a href="solutions.html#monitoring" class="btn">Learn About This Solution</a>
                </div>
                <div class="solution-image">
                    <img src="https://images.unsplash.com/photo-1586773860418-d37222d8fce3?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Water testing">
                </div>
            </div>
            <div style="text-align: center; margin-top: 20px;">
                <a href="solutions.html" class="btn">Explore All Solutions</a>
            </div>
        </div>
    </section>

    <!-- Action Section -->
    <section id="action" class="action">
        <div class="container">
            <h2>Join the Movement</h2>
            <p>Your actions matter. Whether you're an individual, community group, or business, there are many ways to contribute to water conservation and protection efforts.</p>
            <div style="margin-top: 40px;">
                <a href="action.html" class="btn">See How You Can Help</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Water Guardians</h3>
                    <p>Protecting water resources for current and future generations through education, advocacy, and community action.</p>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul class="footer-links">
                        <li><a href="index.html">Home</a></li>
                        <li><a href="about.html">About Us</a></li>
                        <li><a href="issues.html">Water Issues</a></li>
                        <li><a href="solutions.html">Our Solutions</a></li>
                        <li><a href="action.html">Get Involved</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Contact Us</h3>
                    <ul class="footer-links">
                        <li>Email: info@waterguardians.org</li>
                        <li>Phone: +1 (555) 123-4567</li>
                        <li>Address: 123 Conservation Way, Eco City</li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Water Guardians. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
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
