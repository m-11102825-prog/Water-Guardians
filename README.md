<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Guardians - Towards Clean Water Future</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --primary: #1a6aa2;
            --secondary: #26d0ce;
            --accent: #ff6b6b;
            --light: #f8f9fa;
            --dark: #343a40;
            --text: #495057;
        }
        
        body {
            background-color: var(--light);
            color: var(--text);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 80px 0 40px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .header-content {
            position: relative;
            z-index: 2;
        }
        
        h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            font-weight: 700;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }
        
        .subtitle {
            font-size: 1.3rem;
            max-width: 700px;
            margin: 0 auto 30px;
            opacity: 0.9;
        }
        
        .header-wave {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 100px;
            background: url('data:image/svg+xml;utf8,<svg viewBox="0 0 1200 120" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg"><path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" fill="white"></path></svg>');
            background-size: cover;
        }
        
        /* Navigation */
        .nav-container {
            background: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
            display: flex;
            align-items: center;
        }
        
        .logo i {
            margin-right: 10px;
            color: var(--secondary);
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
            transition: color 0.3s;
            position: relative;
        }
        
        .nav-links a:hover {
            color: var(--primary);
        }
        
        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--secondary);
            transition: width 0.3s;
        }
        
        .nav-links a:hover::after {
            width: 100%;
        }
        
        /* Section Styles */
        section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--secondary);
            border-radius: 2px;
        }
        
        .section-title p {
            max-width: 700px;
            margin: 0 auto;
            font-size: 1.1rem;
            color: var(--text);
        }
        
        /* Problems Section */
        .problems-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .problem-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .problem-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        
        .problem-img {
            height: 200px;
            background-color: var(--primary);
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            font-size: 3rem;
        }
        
        .problem-content {
            padding: 25px;
        }
        
        .problem-content h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: var(--primary);
        }
        
        /* Solutions Section */
        .solutions-container {
            background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
            padding: 80px 0;
        }
        
        .solutions-tabs {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin-bottom: 40px;
        }
        
        .tab {
            padding: 12px 25px;
            background: white;
            border: none;
            border-radius: 30px;
            margin: 0 10px 15px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
        }
        
        .tab.active {
            background: var(--primary);
            color: white;
        }
        
        .tab-content {
            display: none;
        }
        
        .tab-content.active {
            display: block;
            animation: fadeIn 0.5s;
        }
        
        .solution-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .solution-card {
            background: white;
            border-radius: 10px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }
        
        .solution-card:hover {
            transform: translateY(-5px);
        }
        
        .solution-icon {
            width: 80px;
            height: 80px;
            background: var(--secondary);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0 auto 20px;
            color: white;
            font-size: 2rem;
        }
        
        .solution-card h3 {
            margin-bottom: 15px;
            color: var(--primary);
        }
        
        /* Impact Section */
        .impact-stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin: 40px 0;
        }
        
        .stat {
            text-align: center;
            margin: 20px;
            padding: 30px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            min-width: 200px;
        }
        
        .stat-value {
            font-size: 3rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 10px;
        }
        
        .stat-label {
            font-size: 1.1rem;
            color: var(--text);
        }
        
        /* Call to Action */
        .cta-section {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            text-align: center;
            padding: 100px 0;
        }
        
        .cta-content {
            max-width: 700px;
            margin: 0 auto;
        }
        
        .cta-content h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        
        .cta-content p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0.9;
        }
        
        .btn {
            display: inline-block;
            padding: 15px 35px;
            background: white;
            color: var(--primary);
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            text-decoration: none;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
        }
        
        /* Footer */
        footer {
            background: var(--dark);
            color: white;
            padding: 60px 0 30px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-column h3 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            color: var(--secondary);
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: #adb5bd;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: white;
        }
        
        .social-links {
            display: flex;
            margin-top: 20px;
        }
        
        .social-links a {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            margin-right: 10px;
            color: white;
            transition: background 0.3s;
        }
        
        .social-links a:hover {
            background: var(--secondary);
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #adb5bd;
            font-size: 0.9rem;
        }
        
        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            .nav-links {
                display: none;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
            
            .impact-stats {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="header-content">
            <div class="container">
                <h1>Water Guardians</h1>
                <p class="subtitle">Join the movement to protect our planet's most vital resource and ensure clean water for future generations</p>
                <a href="#solutions" class="btn">Get Involved</a>
            </div>
        </div>
        <div class="header-wave"></div>
    </header>
    
    <div class="nav-container">
        <div class="container">
            <nav>
                <div class="logo">
                    <i class="fas fa-tint"></i>
                    WaterGuardians
                </div>
                <ul class="nav-links">
                    <li><a href="#problems">The Problem</a></li>
                    <li><a href="#solutions">Solutions</a></li>
                    <li><a href="#impact">Impact</a></li>
                    <li><a href="#action">Take Action</a></li>
                </ul>
            </nav>
        </div>
    </div>
    
    <section id="problems">
        <div class="container">
            <div class="section-title">
                <h2>The Water Crisis</h2>
                <p>Our planet faces unprecedented water challenges that threaten ecosystems, economies, and human health</p>
            </div>
            
            <div class="problems-grid">
                <div class="problem-card">
                    <div class="problem-img">
                        <i class="fas fa-tint-slash"></i>
                    </div>
                    <div class="problem-content">
                        <h3>Water Scarcity</h3>
                        <p>Over 2 billion people live in countries experiencing high water stress, and this number continues to grow due to climate change and population growth.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-img">
                        <i class="fas fa-industry"></i>
                    </div>
                    <div class="problem-content">
                        <h3>Pollution</h3>
                        <p>Industrial waste, agricultural runoff, and plastic pollution contaminate water sources, making them unsafe for consumption and harming aquatic life.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-img">
                        <i class="fas fa-hand-holding-water"></i>
                    </div>
                    <div class="problem-content">
                        <h3>Access Inequality</h3>
                        <p>While some regions have abundant water resources, millions of people lack access to clean drinking water and basic sanitation facilities.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <section class="solutions-container" id="solutions">
        <div class="container">
            <div class="section-title">
                <h2>Our Solutions</h2>
                <p>Practical approaches to address water challenges and create sustainable water management systems</p>
            </div>
            
            <div class="solutions-tabs">
                <button class="tab active" data-tab="conservation">Conservation</button>
                <button class="tab" data-tab="technology">Technology</button>
                <button class="tab" data-tab="policy">Policy</button>
                <button class="tab" data-tab="education">Education</button>
            </div>
            
            <div class="tab-content active" id="conservation">
                <div class="solution-grid">
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-home"></i>
                        </div>
                        <h3>Household Efficiency</h3>
                        <p>Promoting water-saving fixtures and behaviors to reduce domestic water consumption by up to 30%.</p>
                    </div>
                    
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-tractor"></i>
                        </div>
                        <h3>Agricultural Innovation</h3>
                        <p>Implementing precision irrigation and drought-resistant crops to optimize water use in farming.</p>
                    </div>
                    
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-recycle"></i>
                        </div>
                        <h3>Water Recycling</h3>
                        <p>Developing systems to treat and reuse wastewater for non-potable purposes, reducing freshwater demand.</p>
                    </div>
                </div>
            </div>
            
            <div class="tab-content" id="technology">
                <div class="solution-grid">
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-filter"></i>
                        </div>
                        <h3>Purification Systems</h3>
                        <p>Advanced filtration technologies that provide clean drinking water even from contaminated sources.</p>
                    </div>
                    
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-tint"></i>
                        </div>
                        <h3>Rainwater Harvesting</h3>
                        <p>Systems to collect and store rainwater for household and agricultural use during dry periods.</p>
                    </div>
                    
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-cloud-rain"></i>
                        </div>
                        <h3>Desalination</h3>
                        <p>Energy-efficient methods to convert seawater into freshwater for coastal communities.</p>
                    </div>
                </div>
            </div>
            
            <div class="tab-content" id="policy">
                <div class="solution-grid">
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-gavel"></i>
                        </div>
                        <h3>Water Governance</h3>
                        <p>Establishing fair and effective policies for water allocation and protection of water resources.</p>
                    </div>
                    
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-handshake"></i>
                        </div>
                        <h3>International Cooperation</h3>
                        <p>Promoting transboundary water agreements to manage shared water resources sustainably.</p>
                    </div>
                    
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-balance-scale"></i>
                        </div>
                        <h3>Economic Instruments</h3>
                        <p>Implementing water pricing and trading systems that reflect the true value of water.</p>
                    </div>
                </div>
            </div>
            
            <div class="tab-content" id="education">
                <div class="solution-grid">
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-graduation-cap"></i>
                        </div>
                        <h3>School Programs</h3>
                        <p>Integrating water conservation into school curricula to educate the next generation.</p>
                    </div>
                    
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-chalkboard-teacher"></i>
                        </div>
                        <h3>Community Workshops</h3>
                        <p>Training local communities in water management practices and conservation techniques.</p>
                    </div>
                    
                    <div class="solution-card">
                        <div class="solution-icon">
                            <i class="fas fa-bullhorn"></i>
                        </div>
                        <h3>Awareness Campaigns</h3>
                        <p>Public information initiatives to highlight the importance of water conservation.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <section id="impact">
        <div class="container">
            <div class="section-title">
                <h2>Our Impact</h2>
                <p>Measuring the difference we're making in communities around the world</p>
            </div>
            
            <div class="impact-stats">
                <div class="stat">
                    <div class="stat-value">2.5M</div>
                    <div class="stat-label">People with Clean Water Access</div>
                </div>
                
                <div class="stat">
                    <div class="stat-value">350+</div>
                    <div class="stat-label">Communities Engaged</div>
                </div>
                
                <div class="stat">
                    <div class="stat-value">45%</div>
                    <div class="stat-label">Reduction in Water Waste</div>
                </div>
                
                <div class="stat">
                    <div class="stat-value">120</div>
                    <div class="stat-label">Water Projects Completed</div>
                </div>
            </div>
        </div>
    </section>
    
    <section class="cta-section" id="action">
        <div class="container">
            <div class="cta-content">
                <h2>Join the Water Guardians Movement</h2>
                <p>Your actions today will determine the water security of tomorrow. Together, we can protect this precious resource for future generations.</p>
                <a href="#" class="btn">Take Action Now</a>
            </div>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Water Guardians</h3>
                    <p>Dedicated to protecting our planet's water resources through conservation, innovation, and education.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul class="footer-links">
                        <li><a href="#problems">The Problem</a></li>
                        <li><a href="#solutions">Solutions</a></li>
                        <li><a href="#impact">Our Impact</a></li>
                        <li><a href="#action">Get Involved</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Resources</h3>
                    <ul class="footer-links">
                        <li><a href="#">Water Conservation Tips</a></li>
                        <li><a href="#">Educational Materials</a></li>
                        <li><a href="#">Research & Reports</a></li>
                        <li><a href="#">Volunteer Opportunities</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Contact Us</h3>
                    <ul class="footer-links">
                        <li><i class="fas fa-envelope"></i> info@waterguardians.org</li>
                        <li><i class="fas fa-phone"></i> +1 (555) 123-4567</li>
                        <li><i class="fas fa-map-marker-alt"></i> 123 Conservation Way, Eco City</li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2025 Water Guardians. All rights reserved. | Together for a water-secure future</p>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Tab functionality
            const tabs = document.querySelectorAll('.tab');
            const tabContents = document.querySelectorAll('.tab-content');
            
            tabs.forEach(tab => {
                tab.addEventListener('click', () => {
                    const tabId = tab.getAttribute('data-tab');
                    
                    // Remove active class from all tabs and contents
                    tabs.forEach(t => t.classList.remove('active'));
                    tabContents.forEach(c => c.classList.remove('active'));
                    
                    // Add active class to current tab and content
                    tab.classList.add('active');
                    document.getElementById(tabId).classList.add('active');
                });
            });
            
            // Smooth scrolling for navigation links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    
                    const targetId = this.getAttribute('href');
                    if (targetId === '#') return;
                    
                    const targetElement = document.querySelector(targetId);
                    if (targetElement) {
                        window.scrollTo({
                            top: targetElement.offsetTop - 80,
                            behavior: 'smooth'
                        });
                    }
                });
            });
            
            // Add animation on scroll
            const animateOnScroll = function() {
                const elements = document.querySelectorAll('.problem-card, .solution-card, .stat');
                
                elements.forEach(element => {
                    const elementPosition = element.getBoundingClientRect().top;
                    const screenPosition = window.innerHeight / 1.2;
                    
                    if (elementPosition < screenPosition) {
                        element.style.opacity = '1';
                        element.style.transform = 'translateY(0)';
                    }
                });
            };
            
            // Set initial state for animation
            const animatedElements = document.querySelectorAll('.problem-card, .solution-card, .stat');
            animatedElements.forEach(element => {
                element.style.opacity = '0';
                element.style.transform = 'translateY(20px)';
                element.style.transition = 'opacity 0.5s, transform 0.5s';
            });
            
            window.addEventListener('scroll', animateOnScroll);
            // Trigger once on load in case elements are already in view
            animateOnScroll();
        });
    </script>
</body>
</html>
