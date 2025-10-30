<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Kushal Raj - Product Manager Portfolio</title>

    <style>

        * {

            margin: 0;

            padding: 0;

            box-sizing: border-box;

        }

        body {

            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Arial, sans-serif;

            line-height: 1.6;

            color: #333;

            background: #f5f5f5;

        }

        /* Header Section */

        header {

            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);

            color: white;

            padding: 60px 20px;

            text-align: center;

        }

        header h1 {

            font-size: 2.5em;

            margin-bottom: 10px;

            font-weight: 600;

        }

        header p {

            font-size: 1.2em;

            opacity: 0.9;

            margin-bottom: 30px;

        }

        .header-stats {

            display: flex;

            justify-content: center;

            gap: 40px;

            flex-wrap: wrap;

            margin-top: 30px;

        }

        .stat-item {

            text-align: center;

        }

        .stat-number {

            font-size: 2em;

            font-weight: bold;

            display: block;

        }

        .stat-label {

            font-size: 0.9em;

            opacity: 0.8;

        }

        /* Navigation */

        nav {

            background: white;

            padding: 15px 0;

            box-shadow: 0 2px 5px rgba(0,0,0,0.1);

            position: sticky;

            top: 0;

            z-index: 100;

        }

        nav ul {

            list-style: none;

            display: flex;

            justify-content: center;

            gap: 30px;

            flex-wrap: wrap;

        }

        nav a {

            text-decoration: none;

            color: #333;

            font-weight: 500;

            padding: 8px 15px;

            border-radius: 5px;

            transition: all 0.3s;

        }

        nav a:hover {

            background: #1e3c72;

            color: white;

        }

        /* Container */

        .container {

            max-width: 1200px;

            margin: 0 auto;

            padding: 40px 20px;

        }

        /* Section Styles */

        section {

            background: white;

            margin-bottom: 40px;

            padding: 40px;

            border-radius: 10px;

            box-shadow: 0 2px 10px rgba(0,0,0,0.1);

        }

        section h2 {

            font-size: 2em;

            margin-bottom: 10px;

            color: #1e3c72;

            border-bottom: 3px solid #1e3c72;

            padding-bottom: 10px;

            display: inline-block;

        }

        section p.intro {

            color: #666;

            margin: 20px 0 30px 0;

            font-size: 1.1em;

        }

        /* Portfolio Grid */

        .portfolio-grid {

            display: grid;

            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));

            gap: 25px;

            margin-top: 30px;

        }

        .portfolio-card {

            background: #fff;

            border: 2px solid #e0e0e0;

            border-radius: 10px;

            padding: 25px;

            transition: all 0.3s ease;

            cursor: pointer;

            position: relative;

        }

        .portfolio-card:hover {

            transform: translateY(-5px);

            box-shadow: 0 5px 20px rgba(30, 60, 114, 0.2);

            border-color: #1e3c72;

        }

        .portfolio-card .icon {

            font-size: 2.5em;

            margin-bottom: 15px;

        }

        .portfolio-card h3 {

            font-size: 1.3em;

            margin-bottom: 10px;

            color: #1e3c72;

        }

        .portfolio-card p {

            color: #666;

            margin-bottom: 20px;

            min-height: 60px;

        }

        .portfolio-card .tags {

            display: flex;

            flex-wrap: wrap;

            gap: 8px;

            margin-bottom: 15px;

        }

        .tag {

            background: #e8f0fe;

            color: #1e3c72;

            padding: 4px 12px;

            border-radius: 15px;

            font-size: 0.85em;

            font-weight: 500;

        }

        .download-btn {

            display: inline-block;

            background: #1e3c72;

            color: white;

            padding: 10px 20px;

            border-radius: 5px;

            text-decoration: none;

            font-weight: 500;

            transition: all 0.3s;

        }

        .download-btn:hover {

            background: #2a5298;

            transform: scale(1.05);

        }

        /* Experience Cards */

        .experience-grid {

            display: grid;

            gap: 25px;

            margin-top: 30px;

        }

        .experience-card {

            background: #f9f9f9;

            padding: 25px;

            border-radius: 10px;

            border-left: 4px solid #1e3c72;

        }

        .experience-card h3 {

            color: #1e3c72;

            font-size: 1.4em;

            margin-bottom: 5px;

        }

        .experience-card .company {

            color: #666;

            font-style: italic;

            margin-bottom: 15px;

        }

        .experience-card ul {

            margin-left: 20px;

            color: #555;

        }

        .experience-card li {

            margin-bottom: 8px;

        }

        /* Skills Section */

        .skills-container {

            display: flex;

            flex-wrap: wrap;

            gap: 15px;

            margin-top: 30px;

        }

        .skill-badge {

            background: #1e3c72;

            color: white;

            padding: 10px 20px;

            border-radius: 25px;

            font-weight: 500;

        }

        /* Contact Section */

        .contact-info {

            display: flex;

            justify-content: center;

            gap: 30px;

            flex-wrap: wrap;

            margin-top: 30px;

        }

        .contact-item {

            display: flex;

            align-items: center;

            gap: 10px;

            font-size: 1.1em;

        }

        .contact-item a {

            color: #1e3c72;

            text-decoration: none;

            font-weight: 500;

        }

        .contact-item a:hover {

            text-decoration: underline;

        }

        /* Footer */

        footer {

            background: #1e3c72;

            color: white;

            text-align: center;

            padding: 30px 20px;

        }

        /* Responsive */

        @media (max-width: 768px) {

            header h1 {

                font-size: 2em;

            }

            .header-stats {

                gap: 20px;

            }

            section {

                padding: 25px;

            }

            .portfolio-grid {

                grid-template-columns: 1fr;

            }

        }

        /* Highlight Box */

        .highlight-box {

            background: #e8f0fe;

            border-left: 4px solid #1e3c72;

            padding: 20px;

            margin: 20px 0;

            border-radius: 5px;

        }

        .highlight-box strong {

            color: #1e3c72;

        }

    </style>

</head>

<body>

    <!-- Header -->

    <header>

        <h1>Kushal Raj</h1>

        <p>Product Manager | Building Customer-Centric Solutions | 2+ Years B2B/B2C Experience</p>

        <div class="header-stats">

            <div class="stat-item">

                <span class="stat-number">50+</span>

                <span class="stat-label">Enterprise Clients</span>

            </div>

            <div class="stat-item">

                <span class="stat-number">$5M+</span>

                <span class="stat-label">ARR Managed</span>

            </div>

            <div class="stat-item">

                <span class="stat-number">3</span>

                <span class="stat-label">International Markets</span>

            </div>

            <div class="stat-item">

                <span class="stat-number">68%</span>

                <span class="stat-label">Adoption Rate</span>

            </div>

        </div>

    </header>

    <!-- Navigation -->

    <nav>

        <ul>

            <li><a href="#about">About</a></li>

            <li><a href="#portfolio">Strategic Portfolio</a></li>

            <li><a href="#experience">Experience</a></li>

            <li><a href="#skills">Skills</a></li>

            <li><a href="#contact">Contact</a></li>

        </ul>

    </nav>

    <!-- Main Content -->

    <div class="container">

        

        <!-- About Section -->

        <section id="about">

            <h2>About Me</h2>

            <p class="intro">

                I'm a Product Manager with a passion for solving real customer problems through data-driven 

                product strategy and cross-functional collaboration. My approach combines customer discovery, 

                agile execution, and technical understanding to build products that users love and businesses need.

            </p>

            <div class="highlight-box">

                <strong>What I Do Best:</strong> Transform complex technical innovations into clear business value, 

                lead customer engagements through product changes, develop go-to-market strategies with compelling 

                sales narratives, and manage multi-dimensional international projects with cross-functional teams.

            </div>

        </section>

        <!-- Strategic Portfolio Section -->

        <section id="portfolio">

            <h2>Strategic Product Portfolio</h2>

            <p class="intro">

                Comprehensive documents demonstrating GTM strategy, stakeholder management, international expansion, 

                and customer engagement capabilities.

            </p>

            <div class="portfolio-grid">

                <!-- GTM Strategy -->

                <div class="portfolio-card">

                    <div class="icon">🚀</div>

                    <h3>Go-to-Market Strategy & Sales Playbook</h3>

                    <p>Complete GTM strategy for AI-powered search product including sales narratives, objection handling, demo scripts, and team enablement plans.</p>

                    <div class="tags">

                        <span class="tag">Sales Enablement</span>

                        <span class="tag">GTM Strategy</span>

                        <span class="tag">Product Launch</span>

                    </div>

                    <a href="product-management-portfolio/GTM_Strategy_Sales_Playbook.docx" class="download-btn" download>Download Document</a>

                </div>

                <!-- Customer Engagement -->

                <div class="portfolio-card">

                    <div class="icon">🤝</div>

                    <h3>Customer Engagement Case Study</h3>

                    <p>Led 50+ enterprise customers through AI innovation adoption with 68% adoption rate. Shows translation of product features into business value.</p>

                    <div class="tags">

                        <span class="tag">Customer Success</span>

                        <span class="tag">Change Management</span>

                        <span class="tag">Enablement</span>

                    </div>

                    <a href="product-management-portfolio/Customer_Engagement_Case_Study.docx" class="download-btn" download>Download Document</a>

                </div>

                <!-- Product Roadmap -->

                <div class="portfolio-card">

                    <div class="icon">📊</div>

                    <h3>12-Month Product Roadmap</h3>

                    <p>Strategic roadmap for heavy machinery division with stakeholder input integration, quarterly milestones, and international expansion plans.</p>

                    <div class="tags">

                        <span class="tag">Product Strategy</span>

                        <span class="tag">Roadmapping</span>

                        <span class="tag">Stakeholders</span>

                    </div>

                    <a href="product-management-portfolio/Product_Roadmap_Ghanshyam_Engineering.docx" class="download-btn" download>Download Document</a>

                </div>

                <!-- International Market -->

                <div class="portfolio-card">

                    <div class="icon">🌏</div>

                    <h3>International Market Expansion</h3>

                    <p>Southeast Asia market entry strategy (Singapore, Malaysia, Indonesia) with cross-functional coordination and regional adaptations.</p>

                    <div class="tags">

                        <span class="tag">International</span>

                        <span class="tag">Market Entry</span>

                        <span class="tag">Cross-functional</span>

                    </div>

                    <a href="product-management-portfolio/International_Market_Case_Study_Foundit.docx" class="download-btn" download>Download Document</a>

                </div>

                <!-- Stakeholder Framework -->

                <div class="portfolio-card">

                    <div class="icon">⚖️</div>

                    <h3>Stakeholder Management Framework</h3>

                    <p>Systematic 4-step approach to gathering, prioritizing (using RICE), and acting on stakeholder input with real-world examples.</p>

                    <div class="tags">

                        <span class="tag">Prioritization</span>

                        <span class="tag">RICE Framework</span>

                        <span class="tag">Communication</span>

                    </div>

                    <a href="product-management-portfolio/Stakeholder_Management_Framework.docx" class="download-btn" download>Download Document</a>

                </div>

            </div>

        </section>

        <!-- Experience Section -->

        <section id="experience">

            <h2>Professional Experience</h2>

            

            <div class="experience-grid">

                <div class="experience-card">

                    <h3>Product Management - Enterprise Solutions</h3>

                    <p class="company">Foundit (Monster India)</p>

                    <ul>

                        <li>Conducted consultative discovery with 50+ enterprise clients to understand pain points and translate needs into product requirements</li>

                        <li>Identified product gaps and developed tailored solutions that increased customer satisfaction by 35%</li>

                        <li>Led customer engagements for AI innovation adoption, achieving 68% adoption rate (vs 50% target)</li>

                        <li>Created enablement materials and training programs for internal teams and customers</li>

                    </ul>

                </div>

                <div class="experience-card">

                    <h3>Product Discovery & Strategy</h3>

                    <p class="company">Ghanshyam Engineering Company</p>

                    <ul>

                        <li>Led comprehensive product discovery initiative with 10+ stakeholder interviews and cross-functional workshops</li>

                        <li>Reduced customer dissatisfaction from 35% to <10% through customer-centric discovery processes</li>

                        <li>Established product management processes and translated technical specs into user value propositions</li>

                        <li>Managed multi-dimensional B2B product development with engineering, sales, and operations teams</li>

                    </ul>

                </div>

                <div class="experience-card">

                    <h3>Product Strategy & Market Analysis</h3>

                    <p class="company">Academic & Self-Directed Projects</p>

                    <ul>

                        <li><strong>Task Management App:</strong> Designed intuitive app using Eisenhower Matrix framework for 20M+ addressable market</li>

                        <li><strong>Parking Solution:</strong> Created GPS-integrated mobile app addressing challenges for 115M travelers</li>

                        <li>Developed comprehensive product strategies from market research through launch planning</li>

                        <li>Created user personas, conducted competitive analysis, and developed technical specifications</li>

                    </ul>

                </div>

            </div>

        </section>

        <!-- Skills Section -->

        <section id="skills">

            <h2>Core Competencies</h2>

            <p class="intro">Technical and strategic skills developed through hands-on product management experience</p>

            

            <h3 style="margin-top: 30px; margin-bottom: 15px; color: #1e3c72;">Product Strategy & Execution</h3>

            <div class="skills-container">

                <span class="skill-badge">Product Roadmapping</span>

                <span class="skill-badge">Go-to-Market Strategy</span>

                <span class="skill-badge">Customer Discovery</span>

                <span class="skill-badge">Competitive Analysis</span>

                <span class="skill-badge">Feature Prioritization (RICE)</span>

                <span class="skill-badge">Business Strategy</span>

            </div>

            <h3 style="margin-top: 30px; margin-bottom: 15px; color: #1e3c72;">Stakeholder & Customer Management</h3>

            <div class="skills-container">

                <span class="skill-badge">Cross-functional Leadership</span>

                <span class="skill-badge">Stakeholder Management</span>

                <span class="skill-badge">Customer Engagement</span>

                <span class="skill-badge">Sales Enablement</span>

                <span class="skill-badge">Training & Upskilling</span>

                <span class="skill-badge">Change Management</span>

            </div>

            <h3 style="margin-top: 30px; margin-bottom: 15px; color: #1e3c72;">Technical & Analytical</h3>

            <div class="skills-container">

                <span class="skill-badge">Data Analysis</span>

                <span class="skill-badge">SQL</span>

                <span class="skill-badge">Product Analytics</span>

                <span class="skill-badge">A/B Testing</span>

                <span class="skill-badge">Technical Documentation</span>

                <span class="skill-badge">API Integration</span>

            </div>

            <h3 style="margin-top: 30px; margin-bottom: 15px; color: #1e3c72;">Market & International</h3>

            <div class="skills-container">

                <span class="skill-badge">International Expansion</span>

                <span class="skill-badge">Market Entry Strategy</span>

                <span class="skill-badge">Localization</span>

                <span class="skill-badge">Regional Adaptation</span>

                <span class="skill-badge">Competitive Positioning</span>

            </div>

        </section>

        <!-- Contact Section -->

        <section id="contact">

            <h2>Let's Connect</h2>

            <p class="intro">

                I'm always open to discussing product opportunities, collaborations, or just chatting about PM.

            </p>

            <div class="contact-info">

                <div class="contact-item">

                    <span>📧</span>

                    <a href="mailto:kushalraj310@gmail.com">kushalraj310@gmail.com</a>

                </div>

                <div class="contact-item">

                    <span>💼</span>

                    <a href="https://www.linkedin.com/in/kushalraj4/" target="_blank">LinkedIn Profile</a>

                </div>

                <div class="contact-item">

                    <span>🐙</span>

                    <a href="https://github.com/rajkushal01" target="_blank">GitHub Portfolio</a>

                </div>

            </div>

        </section>

    </div>

    <!-- Footer -->

    <footer>

        <p>&copy; 2024 Kushal Raj. All rights reserved.</p>

        <p style="margin-top: 10px; opacity: 0.8;">Building products that users love and businesses need.</p>

    </footer>

    <script>

        // Smooth scrolling for navigation

        document.querySelectorAll('nav a').forEach(anchor => {

            anchor.addEventListener('click', function (e) {

                e.preventDefault();

                const target = document.querySelector(this.getAttribute('href'));

                target.scrollIntoView({

                    behavior: 'smooth',

                    block: 'start'

                });

            });

        });

        // Add animation on scroll

        const observerOptions = {

            threshold: 0.1,

            rootMargin: '0px 0px -50px 0px'

        };

        const observer = new IntersectionObserver((entries) => {

            entries.forEach(entry => {

                if (entry.isIntersecting) {

                    entry.target.style.opacity = '1';

       c            entry.target.style.transform = 'translateY(0)';

                }

            });

        }, observerOptions);

        document.querySelectorAll('.portfolio-card, .experience-card').forEach(card => {

            card.style.opacity = '0';

            card.style.transform = 'translateY(20px)';

            card.style.transition = 'opacity 0.5s, transform 0.5s';

            observer.observe(card);

        });

    </script>

</body>

</html>
