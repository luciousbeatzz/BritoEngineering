# BritoEngineering
BritoEngineering
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BRITO ENG PTY - Mining Safety & Rock Fall Prediction Systems</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #1a5276;
            --secondary: #7d6608;
            --accent: #e74c3c;
            --dark: #2c3e50;
            --light: #ecf0f1;
            --gray: #95a5a6;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: #f9f9f9;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, var(--primary), var(--dark));
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.2);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: white;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .logo span {
            color: var(--secondary);
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--secondary);
        }

        .mobile-menu {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            margin-top: 80px;
            background: linear-gradient(rgba(26, 82, 118, 0.85), rgba(44, 62, 80, 0.9)), url('https://images.unsplash.com/photo-1581091226033-d5c48150dbaa?ixlib=rb-4.0.3') center/cover;
            color: white;
            padding: 6rem 0;
            text-align: center;
        }

        .hero h1 {
            font-size: 3.2rem;
            margin-bottom: 1.5rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .btn {
            display: inline-block;
            background: var(--secondary);
            color: white;
            padding: 0.9rem 2.2rem;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
            cursor: pointer;
            font-size: 1.1rem;
        }

        .btn:hover {
            background: var(--accent);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .btn-outline {
            background: transparent;
            border: 2px solid white;
            margin-left: 1rem;
        }

        .btn-outline:hover {
            background: white;
            color: var(--primary);
        }

        /* Services Section */
        .section {
            padding: 5rem 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-title h2 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
            position: relative;
            display: inline-block;
        }

        .section-title h2:after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--secondary);
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .service-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
            border-top: 5px solid var(--primary);
        }

        .service-card:hover {
            transform: translateY(-10px);
        }

        .service-icon {
            background: var(--primary);
            color: white;
            font-size: 2.5rem;
            padding: 1.5rem;
            text-align: center;
        }

        .service-content {
            padding: 1.5rem;
        }

        .service-content h3 {
            font-size: 1.4rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }

        .service-content p {
            color: #666;
            margin-bottom: 1.5rem;
        }

        .service-features {
            list-style: none;
        }

        .service-features li {
            padding: 0.5rem 0;
            border-bottom: 1px solid #eee;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .service-features li:last-child {
            border-bottom: none;
        }

        .service-features i {
            color: var(--secondary);
        }

        /* Technology Section */
        .technology {
            background: linear-gradient(135deg, var(--dark), var(--primary));
            color: white;
        }

        .technology .section-title h2 {
            color: white;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .tech-card {
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(10px);
            border-radius: 10px;
            padding: 2rem;
            text-align: center;
            transition: transform 0.3s;
        }

        .tech-card:hover {
            transform: translateY(-5px);
            background: rgba(255,255,255,0.15);
        }

        .tech-icon {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            color: var(--secondary);
        }

        .tech-card h3 {
            font-size: 1.4rem;
            margin-bottom: 1rem;
        }

        /* Case Studies */
        .case-studies {
            background: var(--light);
        }

        .case-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .case-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .case-image {
            height: 200px;
            background: var(--gray);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.5rem;
        }

        .case-content {
            padding: 1.5rem;
        }

        .case-content h3 {
            font-size: 1.3rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }

        .case-stats {
            display: flex;
            justify-content: space-between;
            margin-top: 1.5rem;
            padding-top: 1rem;
            border-top: 1px solid #eee;
        }

        .stat {
            text-align: center;
        }

        .stat-value {
            font-size: 1.8rem;
            font-weight: bold;
            color: var(--primary);
        }

        .stat-label {
            font-size: 0.9rem;
            color: var(--gray);
        }

        /* Contact Section */
        .contact {
            background: white;
        }

        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
        }

        .contact-info h3 {
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
            color: var(--primary);
        }

        .contact-details {
            margin-bottom: 2rem;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1rem;
        }

        .contact-item i {
            width: 40px;
            height: 40px;
            background: var(--primary);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .contact-form .form-group {
            margin-bottom: 1.5rem;
        }

        .contact-form label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
        }

        .contact-form input,
        .contact-form textarea,
        .contact-form select {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }

        .contact-form textarea {
            height: 150px;
            resize: vertical;
        }

        /* Footer */
        footer {
            background: var(--dark);
            color: white;
            padding: 3rem 0 1rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-section h3 {
            margin-bottom: 1.5rem;
            color: var(--secondary);
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 0.8rem;
        }

        .footer-links a {
            color: #ddd;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-links a:hover {
            color: var(--secondary);
        }

        .social-links {
            display: flex;
            gap: 1rem;
        }

        .social-links a {
            color: white;
            font-size: 1.2rem;
            transition: color 0.3s;
        }

        .social-links a:hover {
            color: var(--secondary);
        }

        .copyright {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid #444;
            color: #aaa;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .mobile-menu {
                display: block;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .hero p {
                font-size: 1.1rem;
            }

            .btn-container {
                display: flex;
                flex-direction: column;
                gap: 1rem;
            }

            .btn-outline {
                margin-left: 0;
            }

            .contact-container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <div class="logo">
                    <i class="fas fa-mountain"></i>
                    BRITO <span>ENG</span> PTY
                </div>
                <ul class="nav-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#services">Solutions</a></li>
                    <li><a href="#technology">Technology</a></li>
                    <li><a href="#case-studies">Case Studies</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
                <div class="mobile-menu">
                    <i class="fas fa-bars"></i>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Advanced Rock Fall Prediction & Mining Safety Systems</h1>
            <p>Protecting mining operations with cutting-edge technology and predictive analytics to prevent accidents and improve safety underground.</p>
            <div class="btn-container">
                <a href="#contact" class="btn">Request Consultation</a>
                <a href="#technology" class="btn btn-outline">Our Technology</a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="section" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Our Safety Solutions</h2>
                <p>Comprehensive systems designed to address the most critical challenges in underground mining</p>
            </div>
            
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <div class="service-content">
                        <h3>Rock Fall Prediction System</h3>
                        <p>Advanced AI-powered system that analyzes geological data to predict potential rock falls before they happen.</p>
                        <ul class="service-features">
                            <li><i class="fas fa-check"></i> Real-time monitoring</li>
                            <li><i class="fas fa-check"></i> Predictive analytics</li>
                            <li><i class="fas fa-check"></i> Early warning alerts</li>
                            <li><i class="fas fa-check"></i> Geological risk assessment</li>
                        </ul>
                    </div>
                </div>

                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-hard-hat"></i>
                    </div>
                    <div class="service-content">
                        <h3>Worker Safety Monitoring</h3>
                        <p>Comprehensive system to track personnel location, vital signs, and environmental exposure in real-time.</p>
                        <ul class="service-features">
                            <li><i class="fas fa-check"></i> Personnel tracking</li>
                            <li><i class="fas fa-check"></i> Proximity detection</li>
                            <li><i class="fas fa-check"></i> Emergency response</li>
                            <li><i class="fas fa-check"></i> Health monitoring</li>
                        </ul>
                    </div>
                </div>

                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-wind"></i>
                    </div>
                    <div class="service-content">
                        <h3>Ventilation Control System</h3>
                        <p>Intelligent ventilation management that optimizes airflow while monitoring for hazardous gases.</p>
                        <ul class="service-features">
                            <li><i class="fas fa-check"></i> Air quality monitoring</li>
                            <li><i class="fas fa-check"></i> Automated ventilation</li>
                            <li><i class="fas fa-check"></i> Gas detection</li>
                            <li><i class="fas fa-check"></i> Energy optimization</li>
                        </ul>
                    </div>
                </div>

                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-tachometer-alt"></i>
                    </div>
                    <div class="service-content">
                        <h3>Equipment Monitoring</h3>
                        <p>Predictive maintenance and performance monitoring for mining equipment to prevent failures.</p>
                        <ul class="service-features">
                            <li><i class="fas fa-check"></i> Equipment health tracking</li>
                            <li><i class="fas fa-check"></i> Predictive maintenance</li>
                            <li><i class="fas fa-check"></i> Performance analytics</li>
                            <li><i class="fas fa-check"></i> Failure prevention</li>
                        </ul>
                    </div>
                </div>

                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-exclamation-triangle"></i>
                    </div>
                    <div class="service-content">
                        <h3>Emergency Response System</h3>
                        <p>Integrated emergency protocols and communication systems for rapid response to incidents.</p>
                        <ul class="service-features">
                            <li><i class="fas fa-check"></i> Emergency communication</li>
                            <li><i class="fas fa-check"></i> Evacuation guidance</li>
                            <li><i class="fas fa-check"></i> Rescue coordination</li>
                            <li><i class="fas fa-check"></i> Incident reporting</li>
                        </ul>
                    </div>
                </div>

                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-database"></i>
                    </div>
                    <div class="service-content">
                        <h3>Data Analytics Platform</h3>
                        <p>Centralized platform for collecting, analyzing, and visualizing all safety and operational data.</p>
                        <ul class="service-features">
                            <li><i class="fas fa-check"></i> Data integration</li>
                            <li><i class="fas fa-check"></i> Advanced analytics</li>
                            <li><i class="fas fa-check"></i> Custom reporting</li>
                            <li><i class="fas fa-check"></i> Performance insights</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Technology Section -->
    <section class="section technology" id="technology">
        <div class="container">
            <div class="section-title">
                <h2>Our Technology</h2>
                <p>Cutting-edge solutions powered by advanced algorithms and industry expertise</p>
            </div>
            
            <div class="tech-grid">
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fas fa-brain"></i>
                    </div>
                    <h3>AI & Machine Learning</h3>
                    <p>Our proprietary algorithms analyze geological data patterns to predict stability issues with over 94% accuracy.</p>
                </div>

                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fas fa-satellite-dish"></i>
                    </div>
                    <h3>IoT Sensors</h3>
                    <p>Network of wireless sensors continuously monitor ground movement, stress, and environmental conditions.</p>
                </div>

                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fas fa-broadcast-tower"></i>
                    </div>
                    <h3>Real-time Communication</h3>
                    <p>Underground communication systems that work even in the most challenging mining environments.</p>
                </div>

                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fas fa-vr-cardboard"></i>
                    </div>
                    <h3>3D Visualization</h3>
                    <p>Immersive visualization tools that help engineers understand complex geological structures and risks.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Case Studies Section -->
    <section class="section case-studies" id="case-studies">
        <div class="container">
            <div class="section-title">
                <h2>Case Studies</h2>
                <p>Real-world examples of how our systems have improved safety and efficiency</p>
            </div>
            
            <div class="case-grid">
                <div class="case-card">
                    <div class="case-image" style="background: linear-gradient(135deg, #1a5276, #7d6608);">
                        <i class="fas fa-mine"></i>
                    </div>
                    <div class="case-content">
                        <h3>Deep Gold Mine Implementation</h3>
                        <p>Implementation of our rock fall prediction system in a 2km deep gold mine resulted in a 76% reduction in rock fall incidents.</p>
                        <div class="case-stats">
                            <div class="stat">
                                <div class="stat-value">76%</div>
                                <div class="stat-label">Fewer Incidents</div>
                            </div>
                            <div class="stat">
                                <div class="stat-value">42</div>
                                <div class="stat-label">Lives Protected</div>
                            </div>
                            <div class="stat">
                                <div class="stat-value">18</div>
                                <div class="stat-label">Months</div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="case-card">
                    <div class="case-image" style="background: linear-gradient(135deg, #7d6608, #1a5276);">
                        <i class="fas fa-hard-hat"></i>
                    </div>
                    <div class="case-content">
                        <h3>Copper Mine Safety Upgrade</h3>
                        <p>Comprehensive safety system implementation including ventilation control and personnel tracking.</p>
                        <div class="case-stats">
                            <div class="stat">
                                <div class="stat-value">92%</div>
                                <div class="stat-label">Faster Response</div>
                            </div>
                            <div class="stat">
                                <div class="stat-value">15%</div>
                                <div class="stat-label">Productivity Increase</div>
                            </div>
                            <div class="stat">
                                <div class="stat-value">0</div>
                                <div class="stat-label">Major Incidents</div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="case-card">
                    <div class="case-image" style="background: linear-gradient(135deg, #1a5276, #e74c3c);">
                        <i class="fas fa-chart-bar"></i>
                    </div>
                    <div class="case-content">
                        <h3>Predictive Maintenance Success</h3>
                        <p>Equipment monitoring system prevented critical failures and reduced maintenance costs by 34%.</p>
                        <div class="case-stats">
                            <div class="stat">
                                <div class="stat-value">34%</div>
                                <div class="stat-label">Cost Reduction</div>
                            </div>
                            <div class="stat">
                                <div class="stat-value">62%</div>
                                <div class="stat-label">Fewer Downtimes</div>
                            </div>
                            <div class="stat">
                                <div class="stat-value">28</div>
                                <div class="stat-label">Failures Prevented</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="section contact" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Contact Us</h2>
                <p>Get in touch to discuss how we can improve safety at your mining operation</p>
            </div>
            
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Get In Touch</h3>
                    <div class="contact-details">
                        <div class="contact-item">
                            <i class="fas fa-map-marker-alt"></i>
                            <div>
                                <h4>Address</h4>
                                <p>E1124 Phase 1, Blossom tree, Freedom Park, Rustenburg, South Africa</p>
                            </div>
                        </div>
                        <div class="contact-item">
                            <i class="fas fa-phone"></i>
                            <div>
                                <h4>Phone</h4>
                                <p>+27 760 242 725</p>
                            </div>
                        </div>
                        <div class="contact-item">
                            <i class="fas fa-envelope"></i>
                            <div>
                                <h4>Email</h4>
                                <p>solutions@britoeng.co.za</p>
                            </div>
                        </div>
                    </div>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-linkedin"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-facebook"></i></a>
                        <a href="#"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
                
                <form class="contact-form" id="contact-form">
                    <div class="form-group">
                        <label for="name">Full Name</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="company">Company</label>
                        <input type="text" id="company" name="company" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div class="form-group">
                        <label for="phone">Phone</label>
                        <input type="tel" id="phone" name="phone">
                    </div>
                    <div class="form-group">
                        <label for="service">Service Interest</label>
                        <select id="service" name="service">
                            <option value="">Select a service</option>
                            <option value="rock-fall">Rock Fall Prediction</option>
                            <option value="safety-monitoring">Worker Safety Monitoring</option>
                            <option value="ventilation">Ventilation Control</option>
                            <option value="equipment">Equipment Monitoring</option>
                            <option value="emergency">Emergency Response</option>
                            <option value="analytics">Data Analytics</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" name="message" required></textarea>
                    </div>
                    <button type="submit" class="btn">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>BRITO ENG PTY</h3>
                    <p>Leading provider of advanced safety and monitoring solutions for the mining industry. Protecting workers and assets through innovation.</p>
                </div>
                <div class="footer-section">
                    <h3>Quick Links</h3>
                    <ul class="footer-links">
                        <li><a href="#home">Home</a></li>
                        <li><a href="#services">Solutions</a></li>
                        <li><a href="#technology">Technology</a></li>
                        <li><a href="#case-studies">Case Studies</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Services</h3>
                    <ul class="footer-links">
                        <li><a href="#services">Rock Fall Prediction</a></li>
                        <li><a href="#services">Worker Safety Monitoring</a></li>
                        <li><a href="#services">Ventilation Control</a></li>
                        <li><a href="#services">Equipment Monitoring</a></li>
                        <li><a href="#services">Emergency Response</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Connect With Us</h3>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-linkedin"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-facebook"></i></a>
                        <a href="#"><i class="fab fa-youtube"></i></a>
                    </div>
                    <p style="margin-top: 1rem;">Subscribe to our newsletter for updates</p>
                    <div style="display: flex; margin-top: 0.5rem;">
                        <input type="email" placeholder="Your email" style="flex: 1; padding: 0.5rem; border: none; border-radius: 3px 0 0 3px;">
                        <button style="background: var(--secondary); color: white; border: none; padding: 0 1rem; border-radius: 0 3px 3px 0; cursor: pointer;">→</button>
                    </div>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2025 BRITO ENG PTY. All rights reserved. | Mining Safety Solutions</p>
            </div>
        </div>
    </footer>

    <script>
        // Simple form submission handler
        document.getElementById('contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your inquiry! We will contact you shortly.');
            this.reset();
        });

        // Mobile menu toggle
        document.querySelector('.mobile-menu').addEventListener('click', function() {
            document.querySelector('.nav-links').classList.toggle('active');
        });

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
