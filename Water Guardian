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
            cursor: pointer;
        }
        
        .nav-links a:hover, .nav-links a.active {
            color: var(--primary);
        }
        
        /* Page Styles */
        .page {
            display: none;
            animation: fadeIn 0.5s ease;
        }
        
        .page.active {
            display: block;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
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
        
        /* Team Section */
        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .team-member {
            text-align: center;
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .team-member img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 20px;
        }
        
        /* Form Styles */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }
        
        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: inherit;
            font-size: 1rem;
        }
        
        .form-group textarea {
            height: 150px;
            resize: vertical;
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
            cursor: pointer;
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
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <a class="logo" onclick="showPage('home')">Water Guardians</a>
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
                    <p>Join the movement to safeguard our rivers, lakes, and oceans for future generations. Together, we can ensure clean, accessible water for all.</p>
                    <a class="btn" onclick="showPage('action')">Become a Water Guardian</a>
                </div>
            </div>
        </section>

        <!-- About Preview Section -->
        <section class="about">
            <div class="container">
                <h2>About Water Guardians</h2>
                <div class="about-content">
                    <div class="about-text">
                        <p>Water Guardians is a global initiative dedicated to protecting and preserving our planet's most vital resource: water. Founded in 2020, our organization brings together scientists, activists, and concerned citizens to address the growing threats to our water systems.</p>
                        <p>Our mission is to ensure that every person has access to clean, safe drinking water while protecting aquatic ecosystems from pollution, overuse, and climate change impacts.</p>
                        <a class="btn" onclick="showPage('about')">Learn More About Us</a>
                    </div>
                    <div class="about-image">
                        <img src="https://images.unsplash.com/photo-1559827260-dc66d52bef19?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Clean water source">
                    </div>
                </div>
            </div>
        </section>

        <!-- Issues Preview Section -->
        <section class="issues">
            <div class="container">
                <h2>Water Challenges We Face</h2>
                <div class="issues-grid">
                    <div class="issue-card">
                        <div class="issue-icon">💧</div>
                        <h3>Water Scarcity</h3>
                        <p>More than 2 billion people live in countries experiencing high water stress. Climate change, population growth, and inefficient water use are exacerbating this crisis.</p>
                        <a class="btn" onclick="showPage('issues')" style="margin-top: 15px; padding: 8px 20px; font-size: 0.9rem;">Read More</a>
                    </div>
                    <div class="issue-card">
                        <div class="issue-icon">🏭</div>
                        <h3>Pollution</h3>
                        <p>Industrial waste, agricultural runoff, and plastic pollution are contaminating our water sources at an alarming rate, harming marine life and entering our food chain.</p>
                        <a class="btn" onclick="showPage('issues')" style="margin-top: 15px; padding: 8px 20px; font-size: 0.9rem;">Read More</a>
                    </div>
                    <div class="issue-card">
                        <div class="issue-icon">🌡️</div>
                        <h3>Climate Impact</h3>
                        <p>Climate change is disrupting water cycles worldwide, causing more frequent and severe droughts, floods, and storms that threaten freshwater sources.</p>
                        <a class="btn" onclick="showPage('issues')" style="margin-top: 15px; padding: 8px 20px; font-size: 0.9rem;">Read More</a>
                    </div>
                </div>
                <div style="text-align: center; margin-top: 40px;">
                    <a class="btn" onclick="showPage('issues')">View All Water Issues</a>
                </div>
            </div>
        </section>

        <!-- Solutions Preview Section -->
        <section class="solutions">
            <div class="container">
                <h2>Our Solutions</h2>
                <div class="solution-item">
                    <div class="solution-text">
                        <h3>Community Water Monitoring</h3>
                        <p>We empower local communities to monitor their water sources through our citizen science programs. Volunteers are trained to test water quality, identify pollution sources, and report issues to authorities.</p>
                        <a class="btn" onclick="showPage('solutions')">Learn About This Solution</a>
                    </div>
                    <div class="solution-image">
                        <img src="https://images.unsplash.com/photo-1586773860418-d37222d8fce3?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Water testing">
                    </div>
                </div>
                <div style="text-align: center; margin-top: 20px;">
                    <a class="btn" onclick="showPage('solutions')">Explore All Solutions</a>
                </div>
            </div>
        </section>

        <!-- Action Section -->
        <section class="action">
            <div class="container">
                <h2>Join the Movement</h2>
                <p>Your actions matter. Whether you're an individual, community group, or business, there are many ways to contribute to water conservation and protection efforts.</p>
                <div style="margin-top: 40px;">
                    <a class="btn" onclick="showPage('action')">See How You Can Help</a>
                </div>
            </div>
        </section>
    </div>

    <!-- About Page -->
    <div id="about" class="page">
        <div class="page-content">
            <div class="page-hero" style="--hero-image: url('https://images.unsplash.com/photo-1559827260-dc66d52bef19?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80')">
                <div class="container">
                    <h1>About Water Guardians</h1>
                </div>
            </div>
            
            <div class="container">
                <section class="content-section">
                    <h2>Our Mission</h2>
                    <p>Water Guardians is a global initiative dedicated to protecting and preserving our planet's most vital resource: water. Founded in 2020, our organization brings together scientists, activists, and concerned citizens to address the growing threats to our water systems.</p>
                    <p>Our mission is to ensure that every person has access to clean, safe drinking water while protecting aquatic ecosystems from pollution, overuse, and climate change impacts. We work through education, advocacy, and community action to create lasting change.</p>
                    <p>With water scarcity affecting more than 40% of the global population and pollution threatening marine life, the need for water guardians has never been greater. We believe that by working together, we can reverse the damage and create a sustainable water future.</p>
                </section>
                
                <section class="content-section">
                    <h2>Our Story</h2>
                    <p>Water Guardians began as a small community initiative in 2020 when a group of environmental scientists and local activists noticed the deteriorating quality of their local river. What started as weekly water testing and cleanup events quickly grew into a regional movement.</p>
                    <p>By 2022, we had expanded to over 50 communities across three countries, with thousands of volunteers participating in our programs. Our data collection efforts have helped identify and address over 200 pollution sources, leading to improved water quality in numerous watersheds.</p>
                    <p>Today, Water Guardians operates in over 15 countries with a dedicated team of staff and volunteers working to protect water resources through monitoring, education, and policy advocacy.</p>
                </section>
                
                <section class="content-section">
                    <h2>Our Team</h2>
                    <div class="team-grid">
                        <div class="team-member">
                            <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Dr. Sarah Johnson">
                            <h3>Dr. Sarah Johnson</h3>
                            <p>Executive Director</p>
                            <p>Environmental scientist with 15 years of experience in water resource management.</p>
                        </div>
                        <div class="team-member">
                            <img src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Michael Chen">
                            <h3>Michael Chen</h3>
                            <p>Director of Programs</p>
                            <p>Community organizer specializing in citizen science and volunteer engagement.</p>
                        </div>
                        <div class="team-member">
                            <img src="https://images.unsplash.com/photo-1534751516642-a1af1ef26a56?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=80" alt="Dr. Elena Rodriguez">
                            <h3>Dr. Elena Rodriguez</h3>
                            <p>Research Director</p>
                            <p>Marine biologist focused on pollution impacts on aquatic ecosystems.</p>
                        </div>
                    </div>
                </section>
            </div>
        </div>
    </div>

    <!-- Issues Page -->
    <div id="issues" class="page">
        <div class="page-content">
            <div class="page-hero" style="--hero-image: url('https://images.unsplash.com/photo-1569163139394-de44cb54d0ce?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80')">
                <div class="container">
                    <h1>Water Challenges</h1>
                </div>
            </div>
            
            <div class="container">
                <section class="content-section">
                    <h2>Water Scarcity</h2>
                    <div class="about-content">
                        <div class="about-text">
                            <p>More than 2 billion people live in countries experiencing high water stress. Climate change, population growth, and inefficient water use are exacerbating this crisis, threatening agriculture, industry, and basic human needs.</p>
                            <p>By 2025, half of the world's population will be living in water-stressed areas. This scarcity disproportionately affects vulnerable communities, contributing to poverty and conflict.</p>
                            <p>Agriculture accounts for approximately 70% of global freshwater withdrawals, with much of it being used inefficiently. Improving irrigation techniques and promoting water-saving crops could significantly reduce this pressure on water resources.</p>
                        </div>
                        <div class="about-image">
                            <img src="https://images.unsplash.com/photo-1569163139394-de44cb54d0ce?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Dry riverbed">
                        </div>
                    </div>
                </section>
                
                <section class="content-section">
                    <h2>Water Pollution</h2>
                    <div class="about-content">
                        <div class="about-image">
                            <img src="https://images.unsplash.com/photo-1559827260-dc66d52bef19?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Polluted water">
                        </div>
                        <div class="about-text">
                            <p>Industrial waste, agricultural runoff, and plastic pollution are contaminating our water sources at an alarming rate. Every year, 8 million tons of plastic enter our oceans, harming marine life and entering our food chain.</p>
                            <p>Chemical pollutants from factories and farms create dead zones in water bodies where no life can survive. These toxins also make their way into drinking water, posing serious health risks to communities.</p>
                            <p>Nutrient pollution from agricultural fertilizers causes algal blooms that deplete oxygen in water bodies, creating "dead zones" where aquatic life cannot survive. The Gulf of Mexico dead zone, for example, can cover an area larger than Connecticut.</p>
                        </div>
                    </div>
                </section>
                
                <section class="content-section">
                    <h2>Climate Impact on Water</h2>
                    <div class="about-content">
                        <div class="about-text">
                            <p>Climate change is disrupting water cycles worldwide, causing more frequent and severe droughts, floods, and storms. Rising sea levels threaten coastal freshwater sources with saltwater intrusion.</p>
                            <p>Warmer water temperatures affect aquatic ecosystems, causing coral bleaching and disrupting fish migration patterns. These changes have cascading effects on biodiversity and food security.</p>
                            <p>Glacial melt, a critical water source for millions of people, is accelerating due to climate change. In the Himalayas, glacial retreat threatens the water security of nearly 2 billion people who depend on rivers fed by these glaciers.</p>
                        </div>
                        <div class="about-image">
                            <img src="https://images.unsplash.com/photo-1615876234660-9a6c1fb6b4b6?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Melting glacier">
                        </div>
                    </div>
                </section>
            </div>
        </div>
    </div>

    <!-- Solutions Page -->
    <div id="solutions" class="page">
        <div class="page-content">
            <div class="page-hero" style="--hero-image: url('https://images.unsplash.com/photo-1586773860418-d37222d8fce3?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80')">
                <div class="container">
                    <h1>Our Solutions</h1>
                </div>
            </div>
            
            <div class="container">
                <section class="content-section">
                    <h2>Community Water Monitoring</h2>
                    <div class="solution-item">
                        <div class="solution-text">
                            <p>We empower local communities to monitor their water sources through our citizen science programs. Volunteers are trained to test water quality, identify pollution sources, and report issues to authorities.</p>
                            <p>Our mobile app allows users to upload water quality data in real-time, creating a comprehensive map of water health across regions. This data helps identify pollution hotspots and track improvements over time.</p>
                            <p>Through these efforts, we've helped communities identify and address 150+ pollution incidents in the past two years alone. Our monitoring network now includes over 5,000 volunteers across three continents.</p>
                            <a class="btn" onclick="showPage('action')">Get Involved</a>
                        </div>
                        <div class="solution-image">
                            <img src="https://images.unsplash.com/photo-1586773860418-d37222d8fce3?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Water testing">
                        </div>
                    </div>
                </section>
                
                <section class="content-section">
                    <h2>Water Conservation Programs</h2>
                    <div class="solution-item">
                        <div class="solution-image">
                            <img src="https://images.unsplash.com/photo-1551524164-6ca64fb04d0b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Water conservation">
                        </div>
                        <div class="solution-text">
                            <p>We work with municipalities, businesses, and households to implement water-saving technologies and practices. Our programs have helped reduce water consumption by an average of 30% in participating communities.</p>
                            <p>We promote rainwater harvesting, greywater recycling, and efficient irrigation systems. In agricultural areas, we've helped farmers adopt drip irrigation and soil moisture monitoring to reduce water waste.</p>
                            <p>Our educational campaigns reach over 1 million people annually, teaching simple conservation techniques that make a big difference when adopted widely. We've distributed over 50,000 water-saving devices to low-income households.</p>
                            <a class="btn" onclick="showPage('action')">Learn Conservation Tips</a>
                        </div>
                    </div>
                </section>
                
                <section class="content-section">
                    <h2>Policy Advocacy</h2>
                    <div class="solution-item">
                        <div class="solution-text">
                            <p>We advocate for stronger water protection policies at local, national, and international levels. Our team of policy experts works with governments to develop and implement regulations that safeguard water resources.</p>
                            <p>Recent successes include helping pass legislation to limit industrial discharge into rivers and securing funding for wastewater treatment infrastructure in underserved communities.</p>
                            <p>We also participate in international forums to promote transboundary water cooperation and the recognition of water as a human right. Our advocacy has influenced water policy in over 20 countries.</p>
                            <a class="btn" onclick="showPage('action')">Support Our Advocacy</a>
                        </div>
                        <div class="solution-image">
                            <img src="https://images.unsplash.com/photo-1551135049-8a33b5883817?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Policy meeting">
                        </div>
                    </div>
                </section>
            </div>
        </div>
    </div>

    <!-- Action Page -->
    <div id="action" class="page">
        <div class="page-content">
            <div class="page-hero" style="--hero-image: url('https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80')">
                <div class="container">
                    <h1>Take Action</h1>
                </div>
            </div>
            
            <div class="container">
                <section class="content-section">
                    <h2>Join Our Movement</h2>
                    <p>Your actions matter. Whether you're an individual, community group, or business, there are many ways to contribute to water conservation and protection efforts.</p>
                    
                    <div class="issues-grid">
                        <div class="issue-card">
                            <div class="issue-icon">👥</div>
                            <h3>Volunteer</h3>
                            <p>Join our community monitoring programs, participate in cleanup events, or help with educational outreach in your area.</p>
                            <a class="btn" style="margin-top: 15px; padding: 8px 20px; font-size: 0.9rem;">Sign Up</a>
                        </div>
                        <div class="issue-card">
                            <div class="issue-icon">💙</div>
                            <h3>Donate</h3>
                            <p>Support our work financially. Your donation helps fund water testing kits, educational materials, and advocacy efforts.</p>
                            <a class="btn" style="margin-top: 15px; padding: 8px 20px; font-size: 0.9rem;">Donate Now</a>
                        </div>
                        <div class="issue-card">
                            <div class="issue-icon">📢</div>
                            <h3>Advocate</h3>
                            <p>Contact your representatives about water protection policies or start a Water Guardians chapter in your community.</p>
                            <a class="btn" style="margin-top: 15px; padding: 8px 20px; font-size: 0.9rem;">Take Action</a>
                        </div>
                    </div>
                </section>
                
                <section class="content-section">
                    <h2>Contact Us</h2>
                    <div class="about-content">
                        <div class="about-text">
                            <p>Ready to make a difference? Get in touch with us to learn more about how you can contribute to protecting our water resources.</p>
                            <p>We're always looking for passionate individuals, community partners, and corporate sponsors to join our mission.</p>
                            <p><strong>Email:</strong> info@waterguardians.org</p>
                            <p><strong>Phone:</strong> +1 (555) 123-4567</p>
                            <p><strong>Address:</strong> 123 Conservation Way, Eco City</p>
                        </div>
                        <div class="about-image">
                            <div class="contact-form">
                                <div class="form-group">
                                    <label for="name">Name</label>
                                    <input type="text" id="name" placeholder="Your name">
                                </div>
                                <div class="form-group">
                                    <label for="email">Email</label>
                                    <input type="email" id="email" placeholder="Your email">
                                </div>
                                <div class="form-group">
                                    <label for="interest">I'm interested in</label>
                                    <select id="interest">
                                        <option>Volunteering</option>
                                        <option>Donating</option>
                                        <option>Starting a chapter</option>
                                        <option>Partnership</option>
                                        <option>Other</option>
                                    </select>
                                </div>
                                <div class="form-group">
                                    <label for="message">Message</label>
                                    <textarea id="message" placeholder="Your message"></textarea>
                                </div>
                                <button class="btn">Send Message</button>
                            </div>
                        </div>
                    </div>
                </section>
            </div>
        </div>
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
                        <li>Email: info@waterguardians.org</li>
                        <li>Phone: +1 (555) 123-4567</li>
                        <li>Address: 123 Conservation Way, Eco City</li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2025 Water Guardians. All rights reserved.</p>
            </div>
        </div>
    </footer>

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
