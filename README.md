<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Conservation Points | Water Guardians</title>
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
        
        /* Points Section */
        .points-section {
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
        
        .points-container {
            display: flex;
            flex-direction: column;
            gap: 40px;
        }
        
        .point-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            display: flex;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .point-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.15);
        }
        
        .point-number {
            background: var(--primary);
            color: white;
            width: 80px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2.5rem;
            font-weight: 700;
        }
        
        .point-content {
            padding: 30px;
            flex: 1;
        }
        
        .point-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .point-title {
            font-size: 1.8rem;
            color: var(--primary);
        }
        
        .point-icon {
            width: 60px;
            height: 60px;
            background: var(--secondary);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            font-size: 1.5rem;
        }
        
        .point-description {
            margin-bottom: 20px;
            font-size: 1.1rem;
        }
        
        .point-details {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-top: 25px;
        }
        
        .detail-item {
            display: flex;
            align-items: flex-start;
        }
        
        .detail-icon {
            width: 40px;
            height: 40px;
            background: rgba(38, 208, 206, 0.1);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            color: var(--secondary);
            margin-right: 15px;
            flex-shrink: 0;
        }
        
        .detail-content h4 {
            margin-bottom: 5px;
            color: var(--primary);
        }
        
        .stats-container {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin: 60px 0 40px;
        }
        
        .stat {
            text-align: center;
            margin: 20px;
            padding: 30px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            min-width: 200px;
            transition: transform 0.3s;
        }
        
        .stat:hover {
            transform: translateY(-5px);
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
            
            .point-card {
                flex-direction: column;
            }
            
            .point-number {
                width: 100%;
                height: 80px;
            }
            
            .point-details {
                grid-template-columns: 1fr;
            }
            
            .stats-container {
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
                <h1>Water Conservation Points</h1>
                <p class="subtitle">Key strategies and actions to protect our planet's most vital resource</p>
                <a href="#points" class="btn">Explore Points</a>
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
                    <li><a href="#">Home</a></li>
                    <li><a href="#points">Points</a></li>
                    <li><a href="#">Solutions</a></li>
                    <li><a href="#">Get Involved</a></li>
                </ul>
            </nav>
        </div>
    </div>
    
    <section class="points-section" id="points">
        <div class="container">
            <div class="section-title">
                <h2>Key Conservation Points</h2>
                <p>Explore the essential strategies and actions that can make a significant difference in water conservation efforts worldwide</p>
            </div>
            
            <div class="points-container">
                <!-- Point 1 -->
                <div class="point-card">
                    <div class="point-number">1</div>
                    <div class="point-content">
                        <div class="point-header">
                            <h3 class="point-title">Reduce Household Water Usage</h3>
                            <div class="point-icon">
                                <i class="fas fa-home"></i>
                            </div>
                        </div>
                        <p class="point-description">Households account for a significant portion of water consumption. Simple changes in daily habits and upgrades to water-efficient fixtures can dramatically reduce water waste.</p>
                        
                        <div class="point-details">
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-shower"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Shorter Showers</h4>
                                    <p>Reducing shower time by just 2 minutes can save up to 1,500 gallons per person annually.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-faucet"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Fix Leaks</h4>
                                    <p>A dripping faucet can waste over 3,000 gallons per year. Prompt repairs are essential.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-toilet"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Efficient Fixtures</h4>
                                    <p>Low-flow toilets and showerheads can reduce water usage by 20-60%.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-utensils"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Full Loads Only</h4>
                                    <p>Running dishwashers and washing machines only when full saves both water and energy.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Point 2 -->
                <div class="point-card">
                    <div class="point-number">2</div>
                    <div class="point-content">
                        <div class="point-header">
                            <h3 class="point-title">Implement Smart Agricultural Practices</h3>
                            <div class="point-icon">
                                <i class="fas fa-tractor"></i>
                            </div>
                        </div>
                        <p class="point-description">Agriculture is the largest consumer of freshwater globally. Adopting efficient irrigation methods and water-smart farming techniques can significantly reduce agricultural water usage.</p>
                        
                        <div class="point-details">
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-tint"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Drip Irrigation</h4>
                                    <p>Delivers water directly to plant roots, reducing evaporation and runoff by up to 60%.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-cloud-sun"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Soil Moisture Monitoring</h4>
                                    <p>Smart sensors ensure watering only when necessary, preventing over-irrigation.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-seedling"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Drought-Resistant Crops</h4>
                                    <p>Planting crops suited to local climate conditions reduces irrigation demands.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-recycle"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Water Recycling</h4>
                                    <p>Treating and reusing agricultural runoff conserves freshwater resources.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Point 3 -->
                <div class="point-card">
                    <div class="point-number">3</div>
                    <div class="point-content">
                        <div class="point-header">
                            <h3 class="point-title">Promote Industrial Water Efficiency</h3>
                            <div class="point-icon">
                                <i class="fas fa-industry"></i>
                            </div>
                        </div>
                        <p class="point-description">Industries can dramatically reduce their water footprint through process optimization, recycling systems, and innovative technologies that minimize water consumption.</p>
                        
                        <div class="point-details">
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-recycle"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Closed-Loop Systems</h4>
                                    <p>Recycling water within industrial processes reduces freshwater intake by up to 90%.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-cogs"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Process Optimization</h4>
                                    <p>Efficient manufacturing techniques can significantly reduce water requirements.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-chart-line"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Water Audits</h4>
                                    <p>Regular assessments identify areas for improvement and potential savings.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-hand-holding-water"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Alternative Sources</h4>
                                    <p>Using treated wastewater or harvested rainwater for non-potable applications.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Point 4 -->
                <div class="point-card">
                    <div class="point-number">4</div>
                    <div class="point-content">
                        <div class="point-header">
                            <h3 class="point-title">Protect and Restore Watersheds</h3>
                            <div class="point-icon">
                                <i class="fas fa-tree"></i>
                            </div>
                        </div>
                        <p class="point-description">Healthy watersheds are essential for maintaining water quality and regulating water flow. Conservation and restoration efforts protect these vital ecosystems.</p>
                        
                        <div class="point-details">
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-mountain"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Riparian Buffers</h4>
                                    <p>Vegetated areas along water bodies filter pollutants and prevent erosion.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-water"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Wetland Restoration</h4>
                                    <p>Wetlands act as natural water filters and flood control systems.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-ban"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Pollution Prevention</h4>
                                    <p>Reducing agricultural and urban runoff protects water quality.</p>
                                </div>
                            </div>
                            
                            <div class="detail-item">
                                <div class="detail-icon">
                                    <i class="fas fa-hands-helping"></i>
                                </div>
                                <div class="detail-content">
                                    <h4>Community Involvement</h4>
                                    <p>Local stewardship programs engage citizens in watershed protection.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="stats-container">
                <div class="stat">
                    <div class="stat-value">30%</div>
                    <div class="stat-label">Potential Reduction in Household Water Use</div>
                </div>
                
                <div class="stat">
                    <div class="stat-value">50%</div>
                    <div class="stat-label">Water Savings with Drip Irrigation</div>
                </div>
                
                <div class="stat">
                    <div class="stat-value">70%</div>
                    <div class="stat-label">Industrial Water Recycling Potential</div>
                </div>
                
                <div class="stat">
                    <div class="stat-value">2.5B</div>
                    <div class="stat-label">People Impacted by Water Scarcity</div>
                </div>
            </div>
        </div>
    </section>
    
    <section class="cta-section">
        <div class="container">
            <div class="cta-content">
                <h2>Join Our Water Conservation Movement</h2>
                <p>Every action counts. Start implementing these water conservation points today and become part of the solution for a sustainable water future.</p>
                <a href="#" class="btn">Take the Pledge</a>
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
                        <li><a href="#">Home</a></li>
                        <li><a href="#points">Conservation Points</a></li>
                        <li><a href="#">Solutions</a></li>
                        <li><a href="#">Get Involved</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Resources</h3>
                    <ul class="footer-links">
                        <li><a href="#">Water Saving Tips</a></li>
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
                const elements = document.querySelectorAll('.point-card, .stat');
                
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
            const animatedElements = document.querySelectorAll('.point-card, .stat');
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
