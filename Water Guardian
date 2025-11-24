<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Guardians - Home</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800&family=Open+Sans:wght@400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #0066cc;
            --primary-dark: #004d99;
            --primary-light: #4da6ff;
            --secondary: #00cc99;
            --accent: #ff6600;
            --light: #f8fcff;
            --dark: #1a2b3c;
            --text: #2d3748;
            --gray: #718096;
            --blue-light: #e6f2ff;
            --shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            line-height: 1.7;
            color: var(--text);
            background-color: var(--light);
            overflow-x: hidden;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            line-height: 1.3;
            margin-bottom: 1rem;
        }

        h1 {
            font-size: 3.5rem;
            font-weight: 800;
        }

        h2 {
            font-size: 2.8rem;
            position: relative;
            display: inline-block;
        }

        h2:after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 80px;
            height: 4px;
            background: var(--secondary);
            border-radius: 2px;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .section-padding {
            padding: 100px 0;
        }

        .text-center {
            text-align: center;
        }

        .text-center h2:after {
            left: 50%;
            transform: translateX(-50%);
        }

        /* Page Styles */
        .page {
            display: none;
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.5s ease;
        }

        .page.active {
            display: block;
            opacity: 1;
            transform: translateY(0);
        }

        /* Header Styles */
        header {
            background-color: rgba(255, 255, 255, 0.95);
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
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
            display: flex;
            align-items: center;
            text-decoration: none;
            cursor: pointer;
        }

        .logo-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-right: 10px;
        }

        .logo-text {
            font-size: 1.8rem;
            font-weight: 800;
            color: var(--dark);
        }

        .logo-text span {
            color: var(--primary);
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
            font-weight: 600;
            font-size: 1rem;
            transition: var(--transition);
            padding: 8px 0;
            position: relative;
            cursor: pointer;
        }

        .nav-links a:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary);
            transition: var(--transition);
        }

        .nav-links a:hover, .nav-links a.active {
            color: var(--primary);
        }

        .nav-links a:hover:after, .nav-links a.active:after {
            width: 100%;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, rgba(0, 102, 204, 0.85) 0%, rgba(0, 153, 204, 0.8) 100%), 
                        url('https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?ixlib=rb-1.2.1&auto=format&fit=crop&w=1600&q=80');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            color: white;
            margin-top: 80px;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
        }

        .hero p {
            font-size: 1.4rem;
            margin-bottom: 2.5rem;
        }

        .btn {
            display: inline-block;
            padding: 15px 35px;
            background-color: var(--primary);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            font-size: 1.1rem;
            transition: var(--transition);
            border: none;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        .btn-outline {
            background-color: transparent;
            border: 2px solid white;
            margin-left: 15px;
        }

        .btn-outline:hover {
            background-color: white;
            color: var(--primary);
        }

        /* Stats Section */
        .stats {
            background-color: white;
            padding: 80px 0;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .stat-card {
            text-align: center;
            padding: 40px 20px;
            border-radius: 10px;
            background: white;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        .stat-card:hover {
            transform: translateY(-10px);
        }

        .stat-icon {
            font-size: 3rem;
            color: var(--primary);
            margin-bottom: 20px;
        }

        .stat-number {
            font-size: 3.5rem;
            font-weight: 800;
            color: var(--primary);
            margin-bottom: 10px;
        }

        /* About Preview Section */
        .about-preview {
            background-color: var(--blue-light);
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
        }

        .about-image img {
            width: 100%;
            border-radius: 15px;
            box-shadow: var(--shadow);
        }

        /* Issues Preview Section */
        .issues-preview {
            background-color: white;
        }

        .issues-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .issue-card {
            background: white;
            border-radius: 15px;
            padding: 40px 30px;
            box-shadow: var(--shadow);
            transition: var(--transition);
            text-align: center;
        }

        .issue-card:hover {
            transform: translateY(-10px);
        }

        .issue-icon {
            font-size: 3.5rem;
            margin-bottom: 25px;
            color: var(--primary);
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 80px 0 30px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 50px;
        }

        .footer-column h3 {
            color: white;
            margin-bottom: 25px;
            font-size: 1.4rem;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 12px;
        }

        .footer-links a {
            color: #b0b7c3;
            text-decoration: none;
            transition: var(--transition);
            cursor: pointer;
        }

        .footer-links a:hover {
            color: white;
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #b0b7c3;
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 1001;
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            background: white;
            padding: 40px;
            border-radius: 15px;
            max-width: 500px;
            width: 90%;
            text-align: center;
            position: relative;
        }

        .close-modal {
            position: absolute;
            top: 15px;
            right: 20px;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--gray);
        }

        .close-modal:hover {
            color: var(--dark);
        }

        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
        }

        .form-group input, .form-group select, .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }

        .form-group textarea {
            height: 100px;
            resize: vertical;
        }

        /* Alert Styles */
        .alert {
            position: fixed;
            top: 100px;
            right: 20px;
            padding: 15px 25px;
            background: var(--secondary);
            color: white;
            border-radius: 5px;
            box-shadow: var(--shadow);
            z-index: 1002;
            transform: translateX(400px);
            transition: transform 0.3s ease;
        }

        .alert.show {
            transform: translateX(0);
        }

        /* Donation Meter */
        .donation-meter {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: var(--shadow);
            margin: 30px 0;
        }

        .meter-bar {
            height: 20px;
            background: #e0e0e0;
            border-radius: 10px;
            overflow: hidden;
            margin: 15px 0;
        }

        .meter-progress {
            height: 100%;
            background: var(--secondary);
            width: 0%;
            transition: width 1s ease;
        }

        .meter-text {
            display: flex;
            justify-content: space-between;
            font-weight: 600;
        }
    </style>
</head>
<body>
    <!-- Alert Container -->
    <div id="alert" class="alert"></div>

    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <div class="logo" onclick="showPage('home')">
                    <div class="logo-icon">
                        <i class="fas fa-tint"></i>
                    </div>
                    <div class="logo-text">Water<span>Guardians</span></div>
                </div>
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
        <!-- Hero Section -->
        <section class="hero">
            <div class="container">
                <div class="hero-content">
                    <h1>Protecting Our Precious Water Resources</h1>
                    <p>Join the global movement to safeguard our rivers, lakes, and oceans for future generations. Together, we can ensure clean, accessible water for all.</p>
                    <div>
                        <button class="btn" onclick="showPage('action')">Become a Water Guardian</button>
                        <button class="btn btn-outline" onclick="showPage('about')">Learn More</button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Stats Section -->
        <section class="stats">
            <div class="container">
                <div class="stats-grid">
                    <div class="stat-card">
                        <div class="stat-icon">
                            <i class="fas fa-tint"></i>
                        </div>
                        <div class="stat-number">2.2B</div>
                        <div class="stat-text">People Lack Safe Drinking Water</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-icon">
                            <i class="fas fa-recycle"></i>
                        </div>
                        <div class="stat-number">80%</div>
                        <div class="stat-text">Of Wastewater is Untreated</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-icon">
                            <i class="fas fa-water"></i>
                        </div>
                        <div class="stat-number">40%</div>
                        <div class="stat-text">Of Water Bodies Are Polluted</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-icon">
                            <i class="fas fa-wind"></i>
                        </div>
                        <div class="stat-number">90%</div>
                        <div class="stat-text">Of Disasters Are Water-Related</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- About Preview Section -->
        <section class="about-preview section-padding">
            <div class="container">
                <div class="about-content">
                    <div class="about-text">
                        <h2>About Water Guardians</h2>
                        <p>Water Guardians is a global initiative dedicated to protecting and preserving our planet's most vital resource: water. Founded in 2020, our organization brings together scientists, activists, and concerned citizens to address the growing threats to our water systems.</p>
                        <p>Our mission is to ensure that every person has access to clean, safe drinking water while protecting aquatic ecosystems from pollution, overuse, and climate change impacts.</p>
                        <button class="btn" onclick="showPage('about')">Learn More About Us</button>
                    </div>
                    <div class="about-image">
                        <img src="https://images.unsplash.com/photo-1559827260-dc66d52bef19?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Clean water source">
                    </div>
                </div>
            </div>
        </section>

        <!-- Issues Preview Section -->
        <section class="issues-preview section-padding">
            <div class="container">
                <h2 class="text-center">Water Challenges We Face</h2>
                <p class="text-center">Our planet's water resources are under unprecedented threat from multiple fronts.</p>
                
                <div class="issues-grid">
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-tint"></i>
                        </div>
                        <h3>Water Scarcity</h3>
                        <p>More than 2 billion people live in countries experiencing high water stress due to climate change and population growth.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showPage('issues')">Learn More</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-industry"></i>
                        </div>
                        <h3>Pollution</h3>
                        <p>Industrial waste and plastic pollution are contaminating our water sources at an alarming rate.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showPage('issues')">Learn More</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-temperature-high"></i>
                        </div>
                        <h3>Climate Impact</h3>
                        <p>Climate change is disrupting water cycles worldwide, causing more frequent droughts and floods.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showPage('issues')">Learn More</button>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- About Page -->
    <div id="about" class="page">
        <section class="hero" style="background: linear-gradient(135deg, rgba(0, 102, 204, 0.85) 0%, rgba(0, 153, 204, 0.8) 100%); height: 40vh;">
            <div class="container">
                <div class="hero-content">
                    <h1>About Water Guardians</h1>
                    <p>Learn about our mission, vision, and impact</p>
                </div>
            </div>
        </section>

        <section class="section-padding">
            <div class="container">
                <div class="about-content">
                    <div class="about-text">
                        <h2>Our Mission & Vision</h2>
                        <p>Water Guardians was founded in 2020 with a simple but powerful mission: to protect and preserve our planet's most vital resource - water. We believe that access to clean, safe water is a fundamental human right.</p>
                        <p>Our vision is a world where every person has access to clean drinking water, where aquatic ecosystems thrive, and where water resources are managed sustainably for future generations.</p>
                        
                        <h3>Our Impact</h3>
                        <ul style="margin: 20px 0 20px 20px;">
                            <li>Established 150+ community water monitoring programs</li>
                            <li>Trained over 5,000 volunteers in water quality testing</li>
                            <li>Helped identify and address 200+ pollution sources</li>
                            <li>Influenced water protection policies in 20+ countries</li>
                        </ul>
                        
                        <button class="btn" onclick="showContactModal()">Contact Us</button>
                    </div>
                    <div class="about-image">
                        <img src="https://images.unsplash.com/photo-1586773860418-d37222d8fce3?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Team working">
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Issues Page -->
    <div id="issues" class="page">
        <section class="hero" style="background: linear-gradient(135deg, rgba(0, 102, 204, 0.85) 0%, rgba(0, 153, 204, 0.8) 100%); height: 40vh;">
            <div class="container">
                <div class="hero-content">
                    <h1>Water Challenges</h1>
                    <p>Understanding the critical issues facing our water resources</p>
                </div>
            </div>
        </section>

        <section class="section-padding">
            <div class="container">
                <h2 class="text-center">Major Water Issues</h2>
                
                <div class="issues-grid">
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-tint"></i>
                        </div>
                        <h3>Water Scarcity</h3>
                        <p>More than 2 billion people live in countries experiencing high water stress. Climate change, population growth, and inefficient water use are exacerbating this crisis.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showAlert('Learn more about water scarcity solutions')">Solutions</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-industry"></i>
                        </div>
                        <h3>Pollution</h3>
                        <p>Industrial waste, agricultural runoff, and plastic pollution contaminate water sources. Every year, 8 million tons of plastic enter our oceans.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showAlert('Discover pollution prevention methods')">Solutions</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-temperature-high"></i>
                        </div>
                        <h3>Climate Impact</h3>
                        <p>Climate change disrupts water cycles, causing severe droughts and floods. Rising sea levels threaten coastal freshwater sources.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showAlert('Explore climate adaptation strategies')">Solutions</button>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Solutions Page -->
    <div id="solutions" class="page">
        <section class="hero" style="background: linear-gradient(135deg, rgba(0, 102, 204, 0.85) 0%, rgba(0, 153, 204, 0.8) 100%); height: 40vh;">
            <div class="container">
                <div class="hero-content">
                    <h1>Our Solutions</h1>
                    <p>Innovative approaches to water conservation and protection</p>
                </div>
            </div>
        </section>

        <section class="section-padding">
            <div class="container">
                <h2 class="text-center">How We're Making a Difference</h2>
                
                <div class="issues-grid">
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-hand-holding-water"></i>
                        </div>
                        <h3>Community Monitoring</h3>
                        <p>Empowering local communities to test water quality and report pollution issues through our citizen science programs.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showAlert('Join our community monitoring program')">Get Involved</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-seedling"></i>
                        </div>
                        <h3>Conservation Programs</h3>
                        <p>Implementing water-saving technologies and practices in communities, agriculture, and industries.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showAlert('Learn about water conservation techniques')">Learn More</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-gavel"></i>
                        </div>
                        <h3>Policy Advocacy</h3>
                        <p>Working with governments to strengthen water protection regulations and ensure sustainable water management.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showAlert('Support our policy advocacy efforts')">Take Action</button>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Action Page -->
    <div id="action" class="page">
        <section class="hero" style="background: linear-gradient(135deg, rgba(0, 102, 204, 0.85) 0%, rgba(0, 153, 204, 0.8) 100%); height: 40vh;">
            <div class="container">
                <div class="hero-content">
                    <h1>Take Action</h1>
                    <p>Join our movement and make a difference</p>
                </div>
            </div>
        </section>

        <section class="section-padding">
            <div class="container">
                <h2 class="text-center">Get Involved</h2>
                
                <div class="issues-grid">
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-hands-helping"></i>
                        </div>
                        <h3>Volunteer</h3>
                        <p>Join our community monitoring programs, participate in cleanup events, or help with educational outreach.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showVolunteerModal()">Sign Up</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-donate"></i>
                        </div>
                        <h3>Donate</h3>
                        <p>Support our work financially. Your donation helps fund water testing kits and educational materials.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showDonationModal()">Donate Now</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-bullhorn"></i>
                        </div>
                        <h3>Advocate</h3>
                        <p>Contact your representatives about water protection policies or start a local chapter.</p>
                        <button class="btn" style="margin-top: 20px;" onclick="showAlert('Thank you for your interest in advocacy! We will contact you with resources.')">Get Started</button>
                    </div>
                </div>

                <!-- Donation Meter -->
                <div class="donation-meter">
                    <h3 class="text-center">Our Impact Goal</h3>
                    <div class="meter-text">
                        <span>Raised: $<span id="raisedAmount">12,450</span></span>
                        <span>Goal: $25,000</span>
                    </div>
                    <div class="meter-bar">
                        <div class="meter-progress" id="donationProgress"></div>
                    </div>
                    <div class="text-center">
                        <button class="btn" onclick="showDonationModal()">Contribute to Our Goal</button>
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
                    <p>Protecting water resources for current and future generations through education, advocacy, and community action.</p>
                </div>
                
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul class="footer-links">
                        <li><a onclick="showPage('home')">Home</a></li>
                        <li><a onclick="showPage('about')">About Us</a></li>
                        <li><a onclick="showPage('issues')">Water Issues</a></li>
                        <li><a onclick="showPage('solutions')">Our Solutions</a></li>
                        <li><a onclick="showPage('action')">Get Involved</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Contact Us</h3>
                    <ul class="footer-links">
                        <li><a onclick="showContactModal()">info@waterguardians.org</a></li>
                        <li><a>+1 (555) 123-4567</a></li>
                        <li>123 Conservation Way, Eco City</li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2025 Water Guardians. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Modals -->
    <div id="contactModal" class="modal">
        <div class="modal-content">
            <span class="close-modal" onclick="closeModal('contactModal')">&times;</span>
            <h2>Contact Us</h2>
            <form id="contactForm">
                <div class="form-group">
                    <label for="name">Name</label>
                    <input type="text" id="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" required>
                </div>
                <div class="form-group">
                    <label for="message">Message</label>
                    <textarea id="message" required></textarea>
                </div>
                <button type="submit" class="btn">Send Message</button>
            </form>
        </div>
    </div>

    <div id="volunteerModal" class="modal">
        <div class="modal-content">
            <span class="close-modal" onclick="closeModal('volunteerModal')">&times;</span>
            <h2>Volunteer Sign Up</h2>
            <form id="volunteerForm">
                <div class="form-group">
                    <label for="volunteerName">Name</label>
                    <input type="text" id="volunteerName" required>
                </div>
                <div class="form-group">
                    <label for="volunteerEmail">Email</label>
                    <input type="email" id="volunteerEmail" required>
                </div>
                <div class="form-group">
                    <label for="interest">Area of Interest</label>
                    <select id="interest" required>
                        <option value="">Select an option</option>
                        <option value="monitoring">Water Monitoring</option>
                        <option value="cleanup">Cleanup Events</option>
                        <option value="education">Education & Outreach</option>
                        <option value="advocacy">Policy Advocacy</option>
                    </select>
                </div>
                <button type="submit" class="btn">Join as Volunteer</button>
            </form>
        </div>
    </div>

    <div id="donationModal" class="modal">
        <div class="modal-content">
            <span class="close-modal" onclick="closeModal('donationModal')">&times;</span>
            <h2>Make a Donation</h2>
            <form id="donationForm">
                <div class="form-group">
                    <label for="donorName">Name</label>
                    <input type="text" id="donorName" required>
                </div>
                <div class="form-group">
                    <label for="donorEmail">Email</label>
                    <input type="email" id="donorEmail" required>
                </div>
                <div class="form-group">
                    <label for="amount">Donation Amount ($)</label>
                    <input type="number" id="amount" min="1" required>
                </div>
                <button type="submit" class="btn">Donate Now</button>
            </form>
        </div>
    </div>

    <script>
        // Page Navigation System
        function showPage(pageId) {
            console.log('Showing page:', pageId);
            
            // Hide all pages
            document.querySelectorAll('.page').forEach(page => {
                page.classList.remove('active');
            });
            
            // Show selected page
            const targetPage = document.getElementById(pageId);
            if (targetPage) {
                targetPage.classList.add('active');
            }
            
            // Update active nav link
            document.querySelectorAll('.nav-link').forEach(link => {
                link.classList.remove('active');
            });
            
            // Find and activate corresponding nav link
            document.querySelectorAll('.nav-link').forEach(link => {
                if (link.textContent.trim().toLowerCase().includes(pageId) || 
                    (pageId === 'home' && link.textContent.trim().toLowerCase() === 'home')) {
                    link.classList.add('active');
                }
            });
            
            // Scroll to top
            window.scrollTo(0, 0);
            
            // Update donation progress when showing action page
            if (pageId === 'action') {
                updateDonationProgress();
            }
        }

        // Modal Functions
        function showContactModal() {
            document.getElementById('contactModal').style.display = 'flex';
        }

        function showVolunteerModal() {
            document.getElementById('volunteerModal').style.display = 'flex';
        }

        function showDonationModal() {
            document.getElementById('donationModal').style.display = 'flex';
        }

        function closeModal(modalId) {
            document.getElementById(modalId).style.display = 'none';
        }

        // Alert System
        function showAlert(message) {
            const alert = document.getElementById('alert');
            alert.textContent = message;
            alert.classList.add('show');
            
            setTimeout(() => {
                alert.classList.remove('show');
            }, 3000);
        }

        // Donation System
        function updateDonationProgress() {
            const raised = 12450;
            const goal = 25000;
            const progress = (raised / goal) * 100;
            
            document.getElementById('raisedAmount').textContent = raised.toLocaleString();
            document.getElementById('donationProgress').style.width = `${progress}%`;
        }

        // Form Submissions
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            showAlert('Thank you for your message! We will get back to you soon.');
            closeModal('contactModal');
            this.reset();
        });

        document.getElementById('volunteerForm').addEventListener('submit', function(e) {
            e.preventDefault();
            showAlert('Thank you for volunteering! We will contact you with opportunities.');
            closeModal('volunteerModal');
            this.reset();
        });

        document.getElementById('donationForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const amount = document.getElementById('amount').value;
            showAlert(`Thank you for your $${amount} donation!`);
            closeModal('donationModal');
            this.reset();
            
            // Simulate updating donation progress
            setTimeout(updateDonationProgress, 1000);
        });

        // Close modals when clicking outside
        window.addEventListener('click', function(e) {
            if (e.target.classList.contains('modal')) {
                e.target.style.display = 'none';
            }
        });

        // Initialize the page
        document.addEventListener('DOMContentLoaded', function() {
            // Initialize donation progress
            updateDonationProgress();
            
            // Make sure home page is active
            showPage('home');
            
            // Add click handlers to all buttons for debugging
            document.querySelectorAll('button').forEach(button => {
                button.addEventListener('click', function() {
                    console.log('Button clicked:', this.textContent);
                });
            });
        });
    </script>
</body>
</html>
