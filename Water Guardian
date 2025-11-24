<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Guardians | Protecting Our Water Resources</title>
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

        html {
            scroll-behavior: smooth;
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

        h3 {
            font-size: 1.8rem;
        }

        p {
            margin-bottom: 1.5rem;
            font-size: 1.1rem;
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

        /* Header Styles */
        header {
            background-color: rgba(255, 255, 255, 0.95);
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            transition: var(--transition);
        }

        header.scrolled {
            background-color: rgba(255, 255, 255, 0.98);
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
            padding: 10px 0;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            transition: var(--transition);
        }

        .logo {
            display: flex;
            align-items: center;
            text-decoration: none;
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
            position: relative;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            font-size: 1rem;
            transition: var(--transition);
            padding: 8px 0;
            position: relative;
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

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--dark);
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, rgba(0, 102, 204, 0.85) 0%, rgba(0, 153, 204, 0.8) 100%), 
                        url('https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?ixlib=rb-1.2.1&auto=format&fit=crop&w=1600&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            height: 100vh;
            display: flex;
            align-items: center;
            color: white;
            position: relative;
            overflow: hidden;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
            position: relative;
            z-index: 2;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
            animation: fadeInUp 1s ease;
        }

        .hero p {
            font-size: 1.4rem;
            margin-bottom: 2.5rem;
            animation: fadeInUp 1s ease 0.2s both;
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
            position: relative;
            overflow: hidden;
            z-index: 1;
        }

        .btn:before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 0%;
            height: 100%;
            background: var(--primary-dark);
            transition: var(--transition);
            z-index: -1;
            border-radius: 50px;
        }

        .btn:hover:before {
            width: 100%;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        .btn-outline {
            background-color: transparent;
            border: 2px solid white;
            margin-left: 15px;
        }

        .btn-outline:before {
            background: white;
        }

        .btn-outline:hover {
            color: var(--primary);
        }

        /* Stats Section */
        .stats {
            background-color: white;
            padding: 80px 0;
            box-shadow: 0 5px 30px rgba(0, 0, 0, 0.05);
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
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
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
            line-height: 1;
        }

        .stat-text {
            font-size: 1.2rem;
            color: var(--dark);
            font-weight: 600;
        }

        /* About Section */
        .about {
            background-color: var(--blue-light);
            position: relative;
            overflow: hidden;
        }

        .about:before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 40%;
            height: 100%;
            background: url('https://images.unsplash.com/photo-1559827260-dc66d52bef19?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80') no-repeat center center;
            background-size: cover;
            border-radius: 20px 0 0 20px;
        }

        .about-content {
            display: flex;
            align-items: center;
            position: relative;
            z-index: 2;
        }

        .about-text {
            flex: 0 0 60%;
            padding-right: 50px;
        }

        .about-image {
            flex: 0 0 40%;
        }

        .about-image img {
            width: 100%;
            border-radius: 15px;
            box-shadow: var(--shadow);
        }

        .feature-list {
            list-style: none;
            margin: 30px 0;
        }

        .feature-list li {
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
        }

        .feature-list i {
            color: var(--secondary);
            margin-right: 15px;
            font-size: 1.2rem;
            margin-top: 5px;
        }

        /* Issues Section */
        .issues {
            background-color: white;
        }

        .issues-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
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
            position: relative;
            overflow: hidden;
            z-index: 1;
        }

        .issue-card:before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: var(--primary);
            transition: var(--transition);
        }

        .issue-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
        }

        .issue-card:hover:before {
            height: 100%;
            opacity: 0.05;
        }

        .issue-icon {
            font-size: 3.5rem;
            margin-bottom: 25px;
            color: var(--primary);
        }

        .issue-card h3 {
            margin-bottom: 20px;
            color: var(--dark);
        }

        /* Solutions Section */
        .solutions {
            background-color: var(--blue-light);
        }

        .solution-item {
            display: flex;
            align-items: center;
            margin-bottom: 80px;
            gap: 50px;
        }

        .solution-item:nth-child(even) {
            flex-direction: row-reverse;
        }

        .solution-text {
            flex: 1;
        }

        .solution-image {
            flex: 1;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: var(--shadow);
            position: relative;
        }

        .solution-image img {
            width: 100%;
            height: 400px;
            object-fit: cover;
            transition: var(--transition);
        }

        .solution-image:hover img {
            transform: scale(1.05);
        }

        .solution-number {
            position: absolute;
            top: -20px;
            left: -20px;
            width: 60px;
            height: 60px;
            background: var(--primary);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            font-weight: 700;
            box-shadow: var(--shadow);
        }

        .solution-item:nth-child(even) .solution-number {
            left: auto;
            right: -20px;
        }

        /* Action Section */
        .action {
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-dark) 100%);
            color: white;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .action:before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000" preserveAspectRatio="none"><path fill="rgba(255,255,255,0.05)" d="M0,0 L1000,0 L1000,1000 L0,1000 Z"></path></svg>');
            background-size: cover;
        }

        .action h2 {
            color: white;
        }

        .action h2:after {
            background: white;
        }

        .action p {
            max-width: 800px;
            margin: 0 auto 40px;
            font-size: 1.2rem;
        }

        .action-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .action .btn {
            background: white;
            color: var(--primary);
        }

        .action .btn:before {
            background: var(--blue-light);
        }

        .action .btn-outline {
            background: transparent;
            border: 2px solid white;
            color: white;
        }

        .action .btn-outline:before {
            background: white;
        }

        .action .btn-outline:hover {
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
            position: relative;
            padding-bottom: 15px;
        }

        .footer-column h3:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 3px;
            background: var(--secondary);
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
            display: flex;
            align-items: center;
        }

        .footer-links a i {
            margin-right: 10px;
            font-size: 0.9rem;
        }

        .footer-links a:hover {
            color: white;
            transform: translateX(5px);
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            text-decoration: none;
            transition: var(--transition);
        }

        .social-links a:hover {
            background-color: var(--primary);
            transform: translateY(-3px);
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
            color: #b0b7c3;
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.8s ease, transform 0.8s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            h1 {
                font-size: 3rem;
            }
            
            h2 {
                font-size: 2.5rem;
            }
            
            .about:before {
                display: none;
            }
            
            .about-content {
                flex-direction: column;
            }
            
            .about-text {
                padding-right: 0;
                margin-bottom: 50px;
            }
            
            .solution-item, .solution-item:nth-child(even) {
                flex-direction: column;
            }
        }

        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            h1 {
                font-size: 2.5rem;
            }
            
            h2 {
                font-size: 2rem;
            }
            
            .hero {
                height: 80vh;
                background-attachment: scroll;
            }
            
            .section-padding {
                padding: 70px 0;
            }
            
            .action-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .btn-outline {
                margin-left: 0;
                margin-top: 15px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header id="header">
        <div class="container">
            <nav>
                <a href="#" class="logo">
                    <div class="logo-icon">
                        <i class="fas fa-tint"></i>
                    </div>
                    <div class="logo-text">Water<span>Guardians</span></div>
                </a>
                <ul class="nav-links">
                    <li><a href="#home" class="nav-link active">Home</a></li>
                    <li><a href="#about" class="nav-link">About</a></li>
                    <li><a href="#issues" class="nav-link">Issues</a></li>
                    <li><a href="#solutions" class="nav-link">Solutions</a></li>
                    <li><a href="#action" class="nav-link">Take Action</a></li>
                </ul>
                <button class="mobile-menu-btn">
                    <i class="fas fa-bars"></i>
                </button>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>Protecting Our Precious Water Resources</h1>
                <p>Join the global movement to safeguard our rivers, lakes, and oceans for future generations. Together, we can ensure clean, accessible water for all.</p>
                <div>
                    <a href="#action" class="btn">Become a Water Guardian</a>
                    <a href="#about" class="btn btn-outline">Learn More</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="stats">
        <div class="container">
            <div class="stats-grid">
                <div class="stat-card fade-in">
                    <div class="stat-icon">
                        <i class="fas fa-tint"></i>
                    </div>
                    <div class="stat-number">2.2B</div>
                    <div class="stat-text">People Lack Safe Drinking Water</div>
                </div>
                <div class="stat-card fade-in">
                    <div class="stat-icon">
                        <i class="fas fa-recycle"></i>
                    </div>
                    <div class="stat-number">80%</div>
                    <div class="stat-text">Of Wastewater is Untreated</div>
                </div>
                <div class="stat-card fade-in">
                    <div class="stat-icon">
                        <i class="fas fa-water"></i>
                    </div>
                    <div class="stat-number">40%</div>
                    <div class="stat-text">Of Water Bodies Are Polluted</div>
                </div>
                <div class="stat-card fade-in">
                    <div class="stat-icon">
                        <i class="fas fa-wind"></i>
                    </div>
                    <div class="stat-number">90%</div>
                    <div class="stat-text">Of Disasters Are Water-Related</div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about section-padding" id="about">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2>About Water Guardians</h2>
                    <p>Water Guardians is a global initiative dedicated to protecting and preserving our planet's most vital resource: water. Founded in 2020, our organization brings together scientists, activists, and concerned citizens to address the growing threats to our water systems.</p>
                    
                    <p>Our mission is to ensure that every person has access to clean, safe drinking water while protecting aquatic ecosystems from pollution, overuse, and climate change impacts.</p>
                    
                    <ul class="feature-list">
                        <li>
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <strong>Community Empowerment</strong>
                                <p>Engaging local communities in water protection efforts</p>
                            </div>
                        </li>
                        <li>
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <strong>Scientific Research</strong>
                                <p>Conducting cutting-edge research on water quality and conservation</p>
                            </div>
                        </li>
                        <li>
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <strong>Policy Advocacy</strong>
                                <p>Influencing water protection policies at all levels of government</p>
                            </div>
                        </li>
                    </ul>
                    
                    <a href="#action" class="btn">Join Our Mission</a>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1559827260-dc66d52bef19?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Clean water source">
                </div>
            </div>
        </div>
    </section>

    <!-- Issues Section -->
    <section class="issues section-padding" id="issues">
        <div class="container">
            <h2 class="text-center">Water Challenges We Face</h2>
            <p class="text-center">Our planet's water resources are under unprecedented threat from multiple fronts. Understanding these challenges is the first step toward solving them.</p>
            
            <div class="issues-grid">
                <div class="issue-card fade-in">
                    <div class="issue-icon">
                        <i class="fas fa-tint"></i>
                    </div>
                    <h3>Water Scarcity</h3>
                    <p>More than 2 billion people live in countries experiencing high water stress. Climate change, population growth, and inefficient water use are exacerbating this crisis, threatening agriculture, industry, and basic human needs.</p>
                </div>
                
                <div class="issue-card fade-in">
                    <div class="issue-icon">
                        <i class="fas fa-industry"></i>
                    </div>
                    <h3>Pollution</h3>
                    <p>Industrial waste, agricultural runoff, and plastic pollution are contaminating our water sources at an alarming rate. Every year, 8 million tons of plastic enter our oceans, harming marine life and entering our food chain.</p>
                </div>
                
                <div class="issue-card fade-in">
                    <div class="issue-icon">
                        <i class="fas fa-temperature-high"></i>
                    </div>
                    <h3>Climate Impact</h3>
                    <p>Climate change is disrupting water cycles worldwide, causing more frequent and severe droughts, floods, and storms. Rising sea levels threaten coastal freshwater sources with saltwater intrusion.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Solutions Section -->
    <section class="solutions section-padding" id="solutions">
        <div class="container">
            <h2 class="text-center">Our Innovative Solutions</h2>
            <p class="text-center">We're implementing cutting-edge approaches to address water challenges through technology, community engagement, and policy reform.</p>
            
            <div class="solution-item">
                <div class="solution-text">
                    <div class="solution-number">01</div>
                    <h3>Community Water Monitoring</h3>
                    <p>We empower local communities to monitor their water sources through our citizen science programs. Volunteers are trained to test water quality, identify pollution sources, and report issues to authorities.</p>
                    <p>Our mobile app allows users to upload water quality data in real-time, creating a comprehensive map of water health across regions. This data helps identify pollution hotspots and track improvements over time.</p>
                    <a href="#action" class="btn">Get Involved</a>
                </div>
                <div class="solution-image">
                    <img src="https://images.unsplash.com/photo-1586773860418-d37222d8fce3?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Water testing">
                </div>
            </div>
            
            <div class="solution-item">
                <div class="solution-text">
                    <div class="solution-number">02</div>
                    <h3>Water Conservation Programs</h3>
                    <p>We work with municipalities, businesses, and households to implement water-saving technologies and practices. Our programs have helped reduce water consumption by an average of 30% in participating communities.</p>
                    <p>We promote rainwater harvesting, greywater recycling, and efficient irrigation systems. In agricultural areas, we've helped farmers adopt drip irrigation and soil moisture monitoring to reduce water waste.</p>
                    <a href="#action" class="btn">Learn Conservation Tips</a>
                </div>
                <div class="solution-image">
                    <img src="https://images.unsplash.com/photo-1551524164-6ca64fb04d0b?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Water conservation">
                </div>
            </div>
            
            <div class="solution-item">
                <div class="solution-text">
                    <div class="solution-number">03</div>
                    <h3>Policy Advocacy</h3>
                    <p>We advocate for stronger water protection policies at local, national, and international levels. Our team of policy experts works with governments to develop and implement regulations that safeguard water resources.</p>
                    <p>Recent successes include helping pass legislation to limit industrial discharge into rivers and securing funding for wastewater treatment infrastructure in underserved communities.</p>
                    <a href="#action" class="btn">Support Our Advocacy</a>
                </div>
                <div class="solution-image">
                    <img src="https://images.unsplash.com/photo-1551135049-8a33b5883817?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Policy meeting">
                </div>
            </div>
        </div>
    </section>

    <!-- Action Section -->
    <section class="action section-padding" id="action">
        <div class="container">
            <h2 class="text-center">Join the Movement</h2>
            <p>Your actions matter. Whether you're an individual, community group, or business, there are many ways to contribute to water conservation and protection efforts.</p>
            
            <div class="action-buttons">
                <a href="#" class="btn">Volunteer With Us</a>
                <a href="#" class="btn btn-outline">Make a Donation</a>
                <a href="#" class="btn btn-outline">Start a Local Chapter</a>
                <a href="#" class="btn btn-outline">Partner With Us</a>
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
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul class="footer-links">
                        <li><a href="#home"><i class="fas fa-chevron-right"></i> Home</a></li>
                        <li><a href="#about"><i class="fas fa-chevron-right"></i> About Us</a></li>
                        <li><a href="#issues"><i class="fas fa-chevron-right"></i> Water Issues</a></li>
                        <li><a href="#solutions"><i class="fas fa-chevron-right"></i> Our Solutions</a></li>
                        <li><a href="#action"><i class="fas fa-chevron-right"></i> Get Involved</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Contact Us</h3>
                    <ul class="footer-links">
                        <li><a href="#"><i class="fas fa-envelope"></i> info@waterguardians.org</a></li>
                        <li><a href="#"><i class="fas fa-phone"></i> +1 (555) 123-4567</a></li>
                        <li><a href="#"><i class="fas fa-map-marker-alt"></i> 123 Conservation Way, Eco City</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2025 Water Guardians. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // Header scroll effect
        window.addEventListener('scroll', function() {
            const header = document.getElementById('header');
            if (window.scrollY > 50) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    // Update active nav link
                    document.querySelectorAll('.nav-link').forEach(link => {
                        link.classList.remove('active');
                    });
                    this.classList.add('active');
                    
                    // Scroll to target
                    window.scrollTo({
                        top: targetElement.offsetTop - 100,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Fade in animation on scroll
        const fadeElements = document.querySelectorAll('.fade-in');
        
        const fadeInOnScroll = () => {
            fadeElements.forEach(element => {
                const elementTop = element.getBoundingClientRect().top;
                const elementVisible = 150;
                
                if (elementTop < window.innerHeight - elementVisible) {
                    element.classList.add('visible');
                }
            });
        };
        
        window.addEventListener('scroll', fadeInOnScroll);
        // Initial check in case elements are already in view
        fadeInOnScroll();

        // Mobile menu toggle
        const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
        const navLinks = document.querySelector('.nav-links');
        
        mobileMenuBtn.addEventListener('click', () => {
            navLinks.style.display = navLinks.style.display === 'flex' ? 'none' : 'flex';
        });

        // Update active nav link based on scroll position
        const sections = document.querySelectorAll('section');
        const navItems = document.querySelectorAll('.nav-link');
        
        window.addEventListener('scroll', () => {
            let current = '';
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                
                if (scrollY >= (sectionTop - 150)) {
                    current = section.getAttribute('id');
                }
            });
            
            navItems.forEach(item => {
                item.classList.remove('active');
                if (item.getAttribute('href') === `#${current}`) {
                    item.classList.add('active');
                }
            });
        });
    </script>
</body>
</html>
