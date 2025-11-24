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

        html, body {
            width: 100%;
            height: 100%;
            overflow-x: hidden;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            line-height: 1.6;
            color: var(--text);
            background-color: var(--light);
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            line-height: 1.3;
            margin-bottom: 1rem;
        }

        h1 {
            font-size: clamp(2.5rem, 5vw, 3.5rem);
            font-weight: 800;
        }

        h2 {
            font-size: clamp(2rem, 4vw, 2.8rem);
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
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .section-padding {
            padding: 60px 0;
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
            flex: 1;
            width: 100%;
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
            padding: 0;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
            max-width: 1200px;
            margin: 0 auto;
            width: 100%;
        }

        .logo {
            display: flex;
            align-items: center;
            text-decoration: none;
            cursor: pointer;
        }

        .logo-icon {
            font-size: 2rem;
            color: var(--primary);
            margin-right: 10px;
        }

        .logo-text {
            font-size: 1.5rem;
            font-weight: 800;
            color: var(--dark);
        }

        .logo-text span {
            color: var(--primary);
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 20px;
        }

        .nav-links li {
            margin: 0;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            font-size: 0.9rem;
            transition: var(--transition);
            padding: 8px 0;
            position: relative;
            cursor: pointer;
            white-space: nowrap;
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
            min-height: 100vh;
            display: flex;
            align-items: center;
            color: white;
            padding: 80px 0 40px;
            width: 100%;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
            padding: 20px;
        }

        .hero h1 {
            margin-bottom: 1rem;
            text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
        }

        .hero p {
            font-size: clamp(1.1rem, 2.5vw, 1.4rem);
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            padding: 12px 25px;
            background-color: var(--primary);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            font-size: 1rem;
            transition: var(--transition);
            border: none;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            margin: 5px;
        }

        .btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        .btn-outline {
            background-color: transparent;
            border: 2px solid white;
        }

        .btn-outline:hover {
            background-color: white;
            color: var(--primary);
        }

        /* Stats Section */
        .stats {
            background-color: white;
            padding: 50px 0;
            width: 100%;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            width: 100%;
        }

        .stat-card {
            text-align: center;
            padding: 30px 15px;
            border-radius: 10px;
            background: white;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        .stat-card:hover {
            transform: translateY(-5px);
        }

        .stat-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 15px;
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 800;
            color: var(--primary);
            margin-bottom: 10px;
            line-height: 1;
        }

        .stat-text {
            font-size: 1rem;
            color: var(--dark);
            font-weight: 600;
        }

        /* About Preview Section */
        .about-preview {
            background-color: var(--blue-light);
            width: 100%;
        }

        .about-content {
            display: flex;
            align-items: center;
            gap: 30px;
            flex-wrap: wrap;
        }

        .about-text, .about-image {
            flex: 1;
            min-width: 300px;
        }

        .about-image img {
            width: 100%;
            border-radius: 15px;
            box-shadow: var(--shadow);
            height: auto;
        }

        /* Issues Preview Section */
        .issues-preview {
            background-color: white;
            width: 100%;
        }

        .issues-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 30px;
            width: 100%;
        }

        .issue-card {
            background: white;
            border-radius: 15px;
            padding: 30px 20px;
            box-shadow: var(--shadow);
            transition: var(--transition);
            text-align: center;
            display: flex;
            flex-direction: column;
            height: 100%;
        }

        .issue-card:hover {
            transform: translateY(-5px);
        }

        .issue-icon {
            font-size: 3rem;
            margin-bottom: 20px;
            color: var(--primary);
        }

        .issue-card h3 {
            margin-bottom: 15px;
        }

        .issue-card p {
            flex: 1;
            margin-bottom: 20px;
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
            width: 100%;
            margin-top: auto;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }

        .footer-column h3 {
            color: white;
            margin-bottom: 20px;
            font-size: 1.2rem;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 10px;
        }

        .footer-links a {
            color: #b0b7c3;
            text-decoration: none;
            transition: var(--transition);
            cursor: pointer;
            font-size: 0.9rem;
        }

        .footer-links a:hover {
            color: white;
        }

        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #b0b7c3;
            font-size: 0.9rem;
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
            padding: 20px;
        }

        .modal-content {
            background: white;
            padding: 30px;
            border-radius: 15px;
            max-width: 500px;
            width: 100%;
            text-align: center;
            position: relative;
            max-height: 90vh;
            overflow-y: auto;
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
            margin-bottom: 15px;
            text-align: left;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            font-size: 0.9rem;
        }

        .form-group input, .form-group select, .form-group textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 0.9rem;
        }

        .form-group textarea {
            height: 80px;
            resize: vertical;
        }

        /* Alert Styles */
        .alert {
            position: fixed;
            top: 80px;
            right: 20px;
            padding: 12px 20px;
            background: var(--secondary);
            color: white;
            border-radius: 5px;
            box-shadow: var(--shadow);
            z-index: 1002;
            transform: translateX(400px);
            transition: transform 0.3s ease;
            max-width: 300px;
            font-size: 0.9rem;
        }

        .alert.show {
            transform: translateX(0);
        }

        /* Donation Meter */
        .donation-meter {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: var(--shadow);
            margin: 20px 0;
        }

        .meter-bar {
            height: 15px;
            background: #e0e0e0;
            border-radius: 10px;
            overflow: hidden;
            margin: 10px 0;
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
            font-size: 0.9rem;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .container {
                padding: 0 15px;
            }

            nav {
                padding: 10px 0;
            }

            .logo-text {
                font-size: 1.3rem;
            }

            .logo-icon {
                font-size: 1.7rem;
            }

            .nav-links {
                gap: 15px;
            }

            .nav-links a {
                font-size: 0.8rem;
            }

            .hero {
                min-height: 70vh;
                padding: 70px 0 30px;
            }

            .hero-content {
                padding: 10px;
            }

            .section-padding {
                padding: 40px 0;
            }

            .stats-grid,
            .issues-grid {
                grid-template-columns: 1fr;
                gap: 15px;
            }

            .about-content {
                flex-direction: column;
                gap: 20px;
            }

            .about-text, .about-image {
                min-width: 100%;
            }

            .btn {
                display: block;
                width: 100%;
                margin: 5px 0;
            }

            .footer-content {
                grid-template-columns: 1fr;
                gap: 20px;
            }

            .modal-content {
                padding: 20px;
                margin: 10px;
            }
        }

        @media (max-width: 480px) {
            .hero {
                min-height: 60vh;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .stat-card {
                padding: 20px 10px;
            }

            .stat-number {
                font-size: 2rem;
            }

            .issue-card {
                padding: 20px 15px;
            }

            .nav-links {
                flex-wrap: wrap;
                justify-content: center;
            }
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
                        <button class="btn" onclick="showPage('issues')">Learn More</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-industry"></i>
                        </div>
                        <h3>Pollution</h3>
                        <p>Industrial waste and plastic pollution are contaminating our water sources at an alarming rate.</p>
                        <button class="btn" onclick="showPage('issues')">Learn More</button>
                    </div>
                    
                    <div class="issue-card">
                        <div class="issue-icon">
                            <i class="fas fa-temperature-high"></i>
                        </div>
                        <h3>Climate Impact</h3>
                        <p>Climate change is disrupting water cycles worldwide, causing more frequent droughts and floods.</p>
                        <button class="btn" onclick="showPage('issues')">Learn More</button>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Other pages would go here (About, Issues, Solutions, Action) -->

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

    <script>
        // Page Navigation System
        function showPage(pageId) {
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
        }

        // Modal Functions
        function showContactModal() {
            document.getElementById('contactModal').style.display = 'flex';
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

        // Form Submissions
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            showAlert('Thank you for your message! We will get back to you soon.');
            closeModal('contactModal');
            this.reset();
        });

        // Close modals when clicking outside
        window.addEventListener('click', function(e) {
            if (e.target.classList.contains('modal')) {
                e.target.style.display = 'none';
            }
        });

        // Initialize the page
        document.addEventListener('DOMContentLoaded', function() {
            // Make sure home page is active
            showPage('home');
        });
    </script>
</body>
</html>
