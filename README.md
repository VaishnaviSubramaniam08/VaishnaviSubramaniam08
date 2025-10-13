<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vaishnavi Subramaniam | Full-Stack Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Hero Section */
        .hero {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 60px 40px;
            margin-bottom: 30px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            text-align: center;
        }

        .hero h1 {
            font-size: 3em;
            color: #667eea;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .hero .tagline {
            font-size: 1.4em;
            color: #764ba2;
            margin-bottom: 20px;
            font-weight: 500;
        }

        .hero .subtitle {
            font-size: 1.1em;
            color: #555;
            margin-bottom: 30px;
        }

        .badges {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        .badge {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 8px 20px;
            border-radius: 25px;
            font-size: 0.9em;
            font-weight: 500;
        }

        /* Content Sections */
        .section {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            margin-bottom: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }

        .section h2 {
            color: #667eea;
            font-size: 2em;
            margin-bottom: 30px;
            padding-bottom: 15px;
            border-bottom: 3px solid #764ba2;
        }

        /* Tech Stack */
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .tech-item {
            text-align: center;
            padding: 20px;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            border-radius: 15px;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .tech-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(102, 126, 234, 0.3);
        }

        .tech-item img {
            width: 60px;
            height: 60px;
            margin-bottom: 10px;
        }

        .tech-item span {
            display: block;
            font-weight: 600;
            color: #333;
        }

        /* Stats Grid */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .stat-card {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 25px;
            border-radius: 15px;
            color: white;
            text-align: center;
        }

        .stat-card h3 {
            font-size: 1.3em;
            margin-bottom: 15px;
        }

        .progress-bar {
            background: rgba(255, 255, 255, 0.3);
            border-radius: 10px;
            height: 12px;
            overflow: hidden;
            margin: 10px 0;
        }

        .progress-fill {
            height: 100%;
            background: white;
            border-radius: 10px;
            transition: width 1s ease;
        }

        .percentage {
            font-size: 1.5em;
            font-weight: 700;
            margin-top: 10px;
        }

        /* Code Philosophy */
        .code-block {
            background: #1e1e1e;
            color: #d4d4d4;
            padding: 25px;
            border-radius: 10px;
            font-family: 'Courier New', monospace;
            font-size: 0.95em;
            overflow-x: auto;
            margin-top: 20px;
        }

        .code-block .keyword {
            color: #569cd6;
        }

        .code-block .function {
            color: #dcdcaa;
        }

        .code-block .string {
            color: #ce9178;
        }

        .code-block .comment {
            color: #6a9955;
        }

        /* Contact Section */
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .contact-card {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            transition: transform 0.3s;
        }

        .contact-card:hover {
            transform: translateY(-5px);
        }

        .contact-card h3 {
            color: #667eea;
            margin-bottom: 10px;
        }

        .contact-card a {
            color: #764ba2;
            text-decoration: none;
            font-weight: 500;
            word-break: break-all;
        }

        .contact-card a:hover {
            text-decoration: underline;
        }

        /* Platform Links */
        .platform-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 30px;
            flex-wrap: wrap;
        }

        .platform-btn {
            background: white;
            padding: 15px 30px;
            border-radius: 10px;
            text-decoration: none;
            color: #667eea;
            font-weight: 600;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: all 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 10px;
        }

        .platform-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(102, 126, 234, 0.3);
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2em;
            }

            .hero .tagline {
                font-size: 1.1em;
            }

            .section {
                padding: 25px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Hero Section -->
        <div class="hero">
            <h1>Vaishnavi Subramaniam</h1>
            <div class="tagline">From "Hello World" to Real World</div>
            <div class="subtitle">Computer Science Engineer | Full-Stack Developer | Problem Solver</div>
            <div class="badges">
                <span class="badge">🎓 Kongu Engineering College</span>
                <span class="badge">📍 Tiruppur, Tamil Nadu</span>
                <span class="badge">🚀 Building Tomorrow's Tech</span>
            </div>
        </div>

        <!-- Tech Stack Section -->
        <div class="section">
            <h2>🛠 Tech Stack & Expertise</h2>
            <div class="tech-grid">
                <div class="tech-item">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5">
                    <span>HTML5</span>
                </div>
                <div class="tech-item">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3">
                    <span>CSS3</span>
                </div>
                <div class="tech-item">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript">
                    <span>JavaScript</span>
                </div>
                <div class="tech-item">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" alt="React">
                    <span>React</span>
                </div>
                <div class="tech-item">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" alt="Node.js">
                    <span>Node.js</span>
                </div>
                <div class="tech-item">
                    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python">
                    <span>Python</span>
                </div>
            </div>
        </div>

        <!-- Skills Dashboard -->
        <div class="section">
            <h2>📊 Skills Dashboard</h2>
            <div class="stats-grid">
                <div class="stat-card">
                    <h3>⚡ Energy Level</h3>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: 80%"></div>
                    </div>
                    <div class="percentage">80%</div>
                    <p>Powered by Code & Coffee</p>
                </div>
                <div class="stat-card">
                    <h3>🧠 Learning Mode</h3>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: 100%"></div>
                    </div>
                    <div class="percentage">100%</div>
                    <p>Always ON</p>
                </div>
                <div class="stat-card">
                    <h3>🔧 Problem Solving</h3>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: 85%"></div>
                    </div>
                    <div class="percentage">85%</div>
                    <p>Debugging Champion</p>
                </div>
                <div class="stat-card">
                    <h3>🎨 Creativity</h3>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: 75%"></div>
                    </div>
                    <div class="percentage">75%</div>
                    <p>Code Artist</p>
                </div>
                <div class="stat-card">
                    <h3>🤝 Collaboration</h3>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: 85%"></div>
                    </div>
                    <div class="percentage">85%</div>
                    <p>Team Player Ready</p>
                </div>
            </div>
        </div>

        <!-- Code Philosophy -->
        <div class="section">
            <h2>🔥 Code Philosophy</h2>
            <div class="code-block">
<span class="keyword">def</span> <span class="function">my_approach</span>():
    <span class="keyword">while</span> problem_exists:
        <span class="function">analyze_deeply</span>()
        <span class="function">code_with_passion</span>()
        <span class="function">test_rigorously</span>()
        <span class="function">iterate_until_perfect</span>()
    
    <span class="keyword">return</span> <span class="string">"impactful_solution"</span>
            </div>
        </div>

        <!-- Coding Platforms -->
        <div class="section">
            <h2>💻 Competitive Programming</h2>
            <p style="text-align: center; font-size: 1.1em; color: #555; margin-bottom: 20px;">
                Regularly sharpening my problem-solving skills on top coding platforms
            </p>
            <div class="platform-links">
                <a href="https://leetcode.com/vaishnavisubramaniam/" target="_blank" class="platform-btn">
                    <span>📈</span> LeetCode Profile
                </a>
                <a href="https://auth.geeksforgeeks.org/user/vaishnavis08/profile" target="_blank" class="platform-btn">
                    <span>📗</span> GeeksforGeeks Profile
                </a>
            </div>
        </div>

        <!-- Contact Section -->
        <div class="section">
            <h2>📬 Let's Connect</h2>
            <div class="contact-grid">
                <div class="contact-card">
                    <h3>📧 Email</h3>
                    <a href="mailto:vaishnavisubramaniam247@gmail.com">vaishnavisubramaniam247@gmail.com</a>
                </div>
                <div class="contact-card">
                    <h3>📍 Location</h3>
                    <p>Tiruppur, Tamil Nadu</p>
                </div>
                <div class="contact-card">
                    <h3>🎓 Institution</h3>
                    <p>Kongu Engineering College<br>Perundurai</p>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
