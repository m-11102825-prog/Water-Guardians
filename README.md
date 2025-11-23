<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Guardians - Conservation Points</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a2980, #26d0ce);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        header {
            text-align: center;
            padding: 30px 0;
            color: white;
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
        }
        
        .content-wrapper {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin-top: 30px;
        }
        
        .points-container {
            flex: 1;
            min-width: 300px;
            background: white;
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }
        
        .point {
            margin-bottom: 25px;
            padding-bottom: 25px;
            border-bottom: 1px solid #eee;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .point:last-child {
            border-bottom: none;
            margin-bottom: 0;
        }
        
        .point:hover {
            transform: translateX(5px);
        }
        
        .point.active {
            background: #f0f9ff;
            padding: 15px;
            border-radius: 10px;
            border-left: 5px solid #26d0ce;
        }
        
        .point-header {
            display: flex;
            align-items: center;
        }
        
        .point-number {
            display: inline-block;
            width: 35px;
            height: 35px;
            background: #26d0ce;
            color: white;
            border-radius: 50%;
            text-align: center;
            line-height: 35px;
            margin-right: 15px;
            font-weight: bold;
        }
        
        .point-title {
            display: inline-block;
            font-size: 1.3rem;
            font-weight: 600;
            color: #1a2980;
        }
        
        .point-description {
            margin-top: 15px;
            padding-left: 50px;
            color: #555;
            display: none;
        }
        
        .point-image {
            width: 100%;
            height: 200px;
            border-radius: 10px;
            margin-top: 15px;
            object-fit: cover;
            display: none;
        }
        
        .point.active .point-description,
        .point.active .point-image {
            display: block;
            animation: fadeIn 0.5s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .visual-container {
            flex: 1;
            min-width: 300px;
            background: white;
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        
        .water-icon {
            width: 150px;
            height: 150px;
            background: #e6f7ff;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 20px;
            border: 3px solid #26d0ce;
        }
        
        .water-icon i {
            font-size: 70px;
            color: #1a2980;
        }
        
        .visual-title {
            font-size: 1.5rem;
            color: #1a2980;
            margin-bottom: 15px;
            text-align: center;
        }
        
        .visual-description {
            text-align: center;
            color: #555;
            margin-bottom: 20px;
        }
        
        .stats-container {
            display: flex;
            justify-content: space-around;
            width: 100%;
            margin-top: 20px;
        }
        
        .stat {
            text-align: center;
        }
        
        .stat-value {
            font-size: 2rem;
            font-weight: bold;
            color: #1a2980;
        }
        
        .stat-label {
            font-size: 0.9rem;
            color: #777;
        }
        
        .image-gallery {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            margin-top: 25px;
            width: 100%;
        }
        
        .gallery-item {
            border-radius: 10px;
            overflow: hidden;
            height: 120px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        
        .gallery-item:hover {
            transform: scale(1.05);
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .call-to-action {
            text-align: center;
            margin-top: 40px;
            padding: 25px;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            background: #1a2980;
            color: white;
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            margin-top: 15px;
        }
        
        .btn:hover {
            background: #26d0ce;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        footer {
            text-align: center;
            margin-top: 40px;
            color: white;
            opacity: 0.8;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .content-wrapper {
                flex-direction: column;
            }
            
            h1 {
                font-size: 2.2rem;
            }
            
            .image-gallery {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Water Conservation Points</h1>
            <p class="subtitle">Explore key information about water preservation and learn how you can contribute to protecting our planet's most vital resource</p>
        </header>
        
        <div class="content-wrapper">
            <div class="points-container">
                <div class="point active">
                    <div class="point-header">
                        <span class="point-number">1</span>
                        <span class="point-title">Water Scarcity</span>
                    </div>
                    <div class="point-description">
                        <p>Over 2 billion people live in countries experiencing high water stress. Climate change, population growth, and inefficient usage are exacerbating this global crisis.</p>
                        <p>By 2025, half of the world's population will be living in water-stressed areas. Conservation efforts today can prevent severe shortages tomorrow.</p>
                    </div>
                    <img src="https://images.unsplash.com/photo-1548013146-72479768bada?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Dry riverbed showing water scarcity" class="point-image">
                </div>
                
                <div class="point">
                    <div class="point-header">
                        <span class="point-number">2</span>
                        <span class="point-title">Household Conservation</span>
                    </div>
                    <div class="point-description">
                        <p>The average household can reduce water usage by 30% through simple changes like fixing leaks, installing water-efficient fixtures, and changing daily habits.</p>
                        <p>Taking shorter showers, turning off taps when not in use, and only running full loads in dishwashers and washing machines can save thousands of gallons annually.</p>
                    </div>
                    <img src="https://images.unsplash.com/photo-1581578731548-c64695cc6952?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Water saving faucet" class="point-image">
                </div>
                
                <div class="point">
                    <div class="point-header">
                        <span class="point-number">3</span>
                        <span class="point-title">Agricultural Efficiency</span>
                    </div>
                    <div class="point-description">
                        <p>Agriculture accounts for approximately 70% of global freshwater withdrawals. Improving irrigation techniques could save enormous amounts of water.</p>
                        <p>Drip irrigation, soil moisture monitoring, and growing appropriate crops for local climates can significantly reduce agricultural water waste.</p>
                    </div>
                    <img src="https://images.unsplash.com/photo-1622737133809-d95047b9e673?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Modern irrigation system" class="point-image">
                </div>
                
                <div class="point">
                    <div class="point-header">
                        <span class="point-number">4</span>
                        <span class="point-title">Industrial Innovation</span>
                    </div>
                    <div class="point-description">
                        <p>Industries can implement water recycling systems, use dry cooling technologies, and optimize processes to minimize water consumption.</p>
                        <p>Water footprint assessments help companies identify areas for improvement, leading to both environmental benefits and cost savings.</p>
                    </div>
                    <img src="https://images.unsplash.com/photo-1562077980-73cb0d5ae57c?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Water treatment facility" class="point-image">
                </div>
                
                <div class="point">
                    <div class="point-header">
                        <span class="point-number">5</span>
                        <span class="point-title">Community Action</span>
                    </div>
                    <div class="point-description">
                        <p>Local initiatives like rainwater harvesting, watershed protection, and educational programs create resilient communities.</p>
                        <p>Community gardens using native plants, school water conservation programs, and local policy advocacy all contribute to sustainable water management.</p>
                    </div>
                    <img src="https://images.unsplash.com/photo-1559027615-c7c535a81f4f?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Community water conservation project" class="point-image">
                </div>
            </div>
            
            <div class="visual-container">
                <div class="water-icon">
                    <i class="fas fa-tint"></i>
                </div>
                <h2 class="visual-title">The Value of Every Drop</h2>
                <p class="visual-description">Water is essential for all life on Earth. Protecting this precious resource ensures a sustainable future for generations to come.</p>
                
                <div class="stats-container">
                    <div class="stat">
                        <div class="stat-value">97%</div>
                        <div class="stat-label">Salt Water</div>
                    </div>
                    <div class="stat">
                        <div class="stat-value">2.5%</div>
                        <div class="stat-label">Fresh Water</div>
                    </div>
                    <div class="stat">
                        <div class="stat-value">0.5%</div>
                        <div class="stat-label">Accessible</div>
                    </div>
                </div>
                
                <div class="image-gallery">
                    <div class="gallery-item">
                        <img src="https://images.unsplash.com/photo-1439066615861-d1af74d74000?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Clean water source">
                    </div>
                    <div class="gallery-item">
                        <img src="https://images.unsplash.com/photo-1544531585-9847b16c1f1a?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Water testing">
                    </div>
                    <div class="gallery-item">
                        <img src="https://images.unsplash.com/photo-1551085254-e96b210db58a?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Water conservation education">
                    </div>
                    <div class="gallery-item">
                        <img src="https://images.unsplash.com/photo-1570804439979-801c8ac1d1b4?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Rainwater harvesting">
                    </div>
                </div>
            </div>
        </div>
        
        <div class="call-to-action">
            <h2>Join the Water Guardians Movement</h2>
            <p>Your actions matter. Start implementing water conservation practices today and inspire others to do the same.</p>
            <a href="#" class="btn">Learn More</a>
        </div>
        
        <footer>
            <p>Water Guardians Initiative &copy; 2023 | Together we can protect our water resources</p>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const points = document.querySelectorAll('.point');
            
            points.forEach(point => {
                point.addEventListener('click', function() {
                    // Remove active class from all points
                    points.forEach(p => p.classList.remove('active'));
                    
                    // Add active class to clicked point
                    this.classList.add('active');
                });
            });
        });
    </script>
</body>
</html>
