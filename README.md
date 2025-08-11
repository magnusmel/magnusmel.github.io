
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Magnus Melwin Dsouza - Technology & Delivery Manager</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            margin-bottom: 30px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #667eea, #764ba2, #f093fb);
        }

        .profile-section {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
        }

        .profile-info h1 {
            font-size: 3rem;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .profile-info .title {
            font-size: 1.3rem;
            color: #666;
            margin-bottom: 20px;
            font-weight: 300;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
            color: #555;
            text-decoration: none;
            transition: all 0.3s ease;
            padding: 8px 16px;
            border-radius: 25px;
            background: rgba(102, 126, 234, 0.1);
        }

        .contact-item:hover {
            background: rgba(102, 126, 234, 0.2);
            transform: translateY(-2px);
        }

        .section {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            margin-bottom: 30px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }

        .section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: linear-gradient(90deg, #667eea, #764ba2);
        }

        .section h2 {
            font-size: 2.2rem;
            margin-bottom: 30px;
            color: #333;
            position: relative;
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .section h2 i {
            color: #667eea;
        }

        .summary {
            font-size: 1.1rem;
            line-height: 1.8;
            color: #555;
            text-align: justify;
        }

        .experience-item {
            margin-bottom: 40px;
            padding: 30px;
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.05), rgba(118, 75, 162, 0.05));
            border-radius: 15px;
            border-left: 4px solid #667eea;
            transition: all 0.3s ease;
        }

        .experience-item:hover {
            transform: translateX(10px);
            box-shadow: 0 10px 30px rgba(102, 126, 234, 0.15);
        }

        .job-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 15px;
            flex-wrap: wrap;
            gap: 10px;
        }

        .job-title {
            font-size: 1.4rem;
            font-weight: 600;
            color: #333;
        }

        .company {
            font-size: 1.2rem;
            color: #667eea;
            font-weight: 500;
        }

        .duration {
            color: #888;
            font-weight: 500;
            background: rgba(102, 126, 234, 0.1);
            padding: 5px 15px;
            border-radius: 20px;
        }

        .responsibilities {
            list-style: none;
            margin-top: 15px;
        }

        .responsibilities li {
            margin-bottom: 8px;
            padding-left: 25px;
            position: relative;
            color: #555;
        }

        .responsibilities li::before {
            content: '▶';
            position: absolute;
            left: 0;
            color: #667eea;
            font-size: 0.8rem;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .skill-category {
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.1), rgba(118, 75, 162, 0.1));
            padding: 25px;
            border-radius: 15px;
            border-top: 3px solid #667eea;
        }

        .skill-category h3 {
            color: #333;
            margin-bottom: 15px;
            font-size: 1.2rem;
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .skill-tag {
            background: rgba(102, 126, 234, 0.2);
            color: #333;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 25px;
        }

        .project-card {
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.05), rgba(118, 75, 162, 0.05));
            border-radius: 15px;
            padding: 25px;
            border-top: 3px solid #667eea;
            transition: all 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(102, 126, 234, 0.15);
        }

        .project-card h3 {
            color: #333;
            margin-bottom: 10px;
            font-size: 1.3rem;
        }

        .project-meta {
            display: flex;
            justify-content: space-between;
            margin-bottom: 15px;
            flex-wrap: wrap;
            gap: 10px;
        }

        .project-role {
            color: #667eea;
            font-weight: 500;
        }

        .team-size {
            background: rgba(102, 126, 234, 0.1);
            padding: 3px 10px;
            border-radius: 15px;
            font-size: 0.9rem;
        }

        .education-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.05), rgba(118, 75, 162, 0.05));
            border-radius: 10px;
            margin-bottom: 15px;
            border-left: 4px solid #667eea;
        }

        .certifications {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 15px;
        }

        .cert-item {
            background: rgba(102, 126, 234, 0.1);
            padding: 15px 20px;
            border-radius: 10px;
            border-left: 3px solid #667eea;
        }

        .languages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
        }

        .language-item {
            text-align: center;
            padding: 15px;
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.1), rgba(118, 75, 162, 0.1));
            border-radius: 10px;
        }

        .availability {
            text-align: center;
            padding: 30px;
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            border-radius: 15px;
            margin-top: 20px;
        }

        .availability h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }

        .locations {
            font-size: 1.1rem;
            font-weight: 300;
        }

        @media (max-width: 768px) {
            .profile-info h1 {
                font-size: 2.5rem;
            }
            
            .contact-info {
                flex-direction: column;
                align-items: center;
            }
            
            .job-header {
                flex-direction: column;
                align-items: flex-start;
            }
            
            .experience-item:hover {
                transform: none;
            }
        }

        .fade-in {
            animation: fadeIn 0.8s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header Section -->
        <header class="header fade-in">
            <div class="profile-section">
                <div class="profile-info">
                    <h1>Magnus Melwin Dsouza</h1>
                    <p class="title">Technology & Delivery Manager | DevSecOps Leader | Cloud Architect</p>
                    <div class="contact-info">
                        <a href="tel:+96898854173" class="contact-item">
                            <i class="fas fa-phone"></i>
                            <span>(+968) 9885 4173</span>
                        </a>
                        <a href="mailto:magnus.melwin@gmail.com" class="contact-item">
                            <i class="fas fa-envelope"></i>
                            <span>magnus.melwin@gmail.com</span>
                        </a>
                        <a href="https://linkedin.com/in/magnus-melwin-dsouza-bb16534b/" class="contact-item" target="_blank">
                            <i class="fab fa-linkedin"></i>
                            <span>LinkedIn Profile</span>
                        </a>
                    </div>
                </div>
            </div>
        </header>

        <!-- Professional Summary -->
        <section class="section fade-in">
            <h2><i class="fas fa-user-tie"></i>Professional Summary</h2>
            <p class="summary">
                Results-oriented Technology & Delivery Manager with 15+ years of experience in scaling tech teams, 
                driving DevSecOps adoption, and delivering secure enterprise solutions. Proven leadership in hiring, 
                mentoring, and managing global teams. Adept at implementing cyber defense programs and achieving 
                CMMI L3 process maturity. Passionate about innovation, automation, and organizational transformation.
            </p>
        </section>

        <!-- Work Experience -->
        <section class="section fade-in">
            <h2><i class="fas fa-briefcase"></i>Work Experience</h2>
            
            <div class="experience-item">
                <div class="job-header">
                    <div>
                        <div class="job-title">IT Head</div>
                        <div class="company">GlobalMinds</div>
                    </div>
                    <div class="duration">May 2019 - Present</div>
                </div>
                <ul class="responsibilities">
                    <li>Developed end-to-end software solutions optimized for the Insurance industry for the UK and EU</li>
                    <li>Involved in building solutions for the migration of Oracle EBS Systems to Oracle Cloud ERP Fusion for ADIA (Abu Dhabi Investment Authority)</li>
                    <li>Architected Cloud-based platforms for Finance, human capital & Insurance domains</li>
                    <li>Designed and implemented scalable software solutions</li>
                    <li>Architected, Developed and built multiple products using Mendix, Oracle Apex and Oracle Cloud</li>
                    <li>Implemented Zoho ERP systems across departments</li>
                    <li>Trained & Implemented a cyber defense team for the organization</li>
                    <li>SIEM systems implementation</li>
                    <li>Managing recruitment, training and certifications programmes across the organization</li>
                    <li>Helped transform the organization to CMMI level 3 by adopting best practices as per industry standards</li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="job-header">
                    <div>
                        <div class="job-title">DevSecOps Head</div>
                        <div class="company">Entersoft Information Systems Pvt Ltd</div>
                    </div>
                    <div class="duration">Oct 2017 - Mar 2019</div>
                </div>
                <ul class="responsibilities">
                    <li>Led a global security team across Australia, Singapore, and India</li>
                    <li>Integrated security automation into DevOps pipelines</li>
                    <li>Designed security solutions to enhance pre-sales and client trust</li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="job-header">
                    <div>
                        <div class="job-title">Tech Head</div>
                        <div class="company">Roadbang Pvt Ltd</div>
                    </div>
                    <div class="duration">Jun 2016 - Sep 2017</div>
                </div>
                <ul class="responsibilities">
                    <li>Led a team to develop smart transport solutions</li>
                    <li>Designed big data solutions using Spark and Hadoop</li>
                    <li>Implemented IBM Watson-powered recommendation engine</li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="job-header">
                    <div>
                        <div class="job-title">Software Consultant</div>
                        <div class="company">Imboss Consulting</div>
                    </div>
                    <div class="duration">Jun 2013 - Apr 2016</div>
                </div>
                <ul class="responsibilities">
                    <li>Developed blockchain solutions for the agriculture industry</li>
                    <li>Managed full software lifecycle, from requirements to deployment</li>
                    <li>Led rapid application development for various enterprise clients</li>
                </ul>
            </div>

            <div class="experience-item">
                <div class="job-header">
                    <div>
                        <div class="job-title">Software Engineer</div>
                        <div class="company">Globalminds</div>
                    </div>
                    <div class="duration">Apr 2006 - May 2013</div>
                </div>
                <ul class="responsibilities">
                    <li>Developed Python & PL/SQL-based applications using MVC architecture</li>
                    <li>Worked extensively on ETL tasks, database tuning, and automation scripts</li>
                    <li>Built robust Oracle-based solutions for enterprise clients</li>
                </ul>
            </div>
        </section>

        <!-- Technical Skills -->
        <section class="section fade-in">
            <h2><i class="fas fa-code"></i>Technical Skills</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>Programming</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Python 2.x/3.x</span>
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">Shell Script</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Cloud Platforms</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">AWS</span>
                        <span class="skill-tag">Azure</span>
                        <span class="skill-tag">Oracle Cloud</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>DevSecOps & Automation</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Kubernetes</span>
                        <span class="skill-tag">Docker</span>
                        <span class="skill-tag">Jenkins</span>
                        <span class="skill-tag">Git</span>
                        <span class="skill-tag">CI/CD Pipelines</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Databases</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Oracle</span>
                        <span class="skill-tag">MySQL</span>
                        <span class="skill-tag">DynamoDB</span>
                        <span class="skill-tag">MongoDB</span>
                        <span class="skill-tag">RDS</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>Serverless Technologies</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">AWS Lambda</span>
                        <span class="skill-tag">Azure Functions</span>
                    </div>
                </div>
                <div class="skill-category">
                    <h3>AI & Cybersecurity</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Langchain</span>
                        <span class="skill-tag">Wireshark</span>
                        <span class="skill-tag">Burpsuite</span>
                        <span class="skill-tag">Linux</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Notable Projects -->
        <section class="section fade-in">
            <h2><i class="fas fa-project-diagram"></i>Notable Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3>Abu Dhabi Investment Authority (ADIA)</h3>
                    <div class="project-meta">
                        <span class="project-role">Tech Lead</span>
                        <span class="team-size">Team Size: 8</span>
                    </div>
                    <p>Implementation of Oracle Fusion Cloud and migration from E-Business suite (EBS) to fusion cloud. Implemented various extensions via Oracle Apex and Oracle VBCS to support existing business requirements.</p>
                </div>

                <div class="project-card">
                    <h3>Reassure Insurance, UK</h3>
                    <div class="project-meta">
                        <span class="project-role">Lead Developer, Architect</span>
                        <span class="team-size">Team Size: 9</span>
                    </div>
                    <p>Developed application using Mendix Platform to manage insurance products across the UK and 3 European countries. The solution provides high-level interactivity with various parts of the Reassure estate.</p>
                </div>

                <div class="project-card">
                    <h3>Vetkart</h3>
                    <div class="project-meta">
                        <span class="project-role">Full Stack Developer, Architect</span>
                        <span class="team-size">Team Size: 8</span>
                    </div>
                    <p>Developed a web & mobile application for veterinary services using Ionic, AngularJS, and Google Cloud Firebase.</p>
                </div>

                <div class="project-card">
                    <h3>Spideren</h3>
                    <div class="project-meta">
                        <span class="project-role">Full Stack Developer, Architect</span>
                        <span class="team-size">Team Size: 4</span>
                    </div>
                    <p>Built a security vulnerability assessment tool using AWS Lambda, ReactJS, DynamoDB, and Docker.</p>
                </div>

                <div class="project-card">
                    <h3>TowMe</h3>
                    <div class="project-meta">
                        <span class="project-role">Full Stack Developer, Architect</span>
                        <span class="team-size">Team Size: 6</span>
                    </div>
                    <p>Designed a mobile towing service app optimized for low-connectivity environments using Google Cloud & Firebase.</p>
                </div>

                <div class="project-card">
                    <h3>Ktrade</h3>
                    <div class="project-meta">
                        <span class="project-role">Full Stack Developer, Architect</span>
                        <span class="team-size">Team Size: 5</span>
                    </div>
                    <p>Developed a blockchain-based agricultural tracking system using Ethereum, Solidity, and AWS Cloud.</p>
                </div>
            </div>
        </section>

        <!-- Education -->
        <section class="section fade-in">
            <h2><i class="fas fa-graduation-cap"></i>Education</h2>
            <div class="education-item">
                <div>
                    <strong>Masters of Computer Applications in Cybersecurity (MCA)</strong><br>
                    <em>Amrita University, India</em>
                </div>
                <div class="duration">Currently Pursuing (2025)</div>
            </div>
            <div class="education-item">
                <div>
                    <strong>Bachelor of Computer Applications (BCA)</strong><br>
                    <em>Bangalore University, India</em>
                </div>
                <div class="duration">First Class (2006)</div>
            </div>
        </section>

        <!-- Certifications & Languages -->
        <section class="section fade-in">
            <h2><i class="fas fa-certificate"></i>Certifications & Languages</h2>
            
            <h3 style="margin-bottom: 20px; color: #667eea;">Certifications</h3>
            <div class="certifications">
                <div class="cert-item">AWS Certified Solutions Architect</div>
                <div class="cert-item">Azure Fundamentals</div>
                <div class="cert-item">Oracle Cloud Infrastructure 2023 Certified Architect Associate</div>
                <div class="cert-item">AWS Cloud Certified</div>
                <div class="cert-item">ISC2 Certified in Cybersecurity (CC) - 2025</div>
                <div class="cert-item">Ec-council - Certified Penetration Tester (CPENT) 2025</div>
            </div>

            <h3 style="margin: 30px 0 20px; color: #667eea;">Languages</h3>
            <div class="languages-grid">
                <div class="language-item">
                    <strong>English</strong><br>
                    <em>C1 - IELTS 7.5 (Expert)</em>
                </div>
                <div class="language-item">
                    <strong>French</strong><br>
                    <em>B1 (Intermediate)</em>
                </div>
                <div class="language-item">
                    <strong>German</strong><br>
                    <em>A2 (Beginner)</em>
                </div>
                <div class="language-item">
                    <strong>Japanese</strong><br>
                    <em>N5 (Beginner)</em>
                </div>
                <div class="language-item">
                    <strong>Arabic</strong><br>
                    <em>A2 (Beginner)</em>
                </div>
            </div>
        </section>

        <!-- Availability -->
        <div class="availability fade-in">
            <h3><i class="fas fa-map-marker-alt"></i> Availability</h3>
            <p>Open to Full-Time & Contract Roles</p>
            <div class="locations">
                <strong>Preferred Locations:</strong> Oman, Saudi Arabia, Remote, Global Opportunities
            </div>
        </div>
    </div>

    <script>
        // Add smooth scrolling and fade-in animations
        document.addEventListener('DOMContentLoaded', function() {
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };

            const observer = new IntersectionObserver(function(entries) {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, observerOptions);

            // Observe all sections for animation
            document.querySelectorAll('.section, .header, .availability').forEach(section => {
                section.style.opacity = '0';
                section.style.transform = 'translateY(20px)';
                section.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
                observer.observe(section);
            });

            // Add hover effects for experience items
            document.querySelectorAll('.experience-item').forEach(item => {
                item.addEventListener('mouseenter', function() {
                    this.style.transform = 'translateX(10px)';
                });
                
                item.addEventListener('mouseleave', function() {
                    this.style.transform = 'translateX(0)';
                });
            });
        });
    </script>
</body>
</html>
