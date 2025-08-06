<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hello, I'm Evangel 👋</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f8f9fa;
            padding: 40px 20px;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.08);
            overflow: hidden;
        }

        .header {
            padding: 40px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            text-align: center;
        }

        .header h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            font-weight: 300;
        }

        .contact-links {
            margin-bottom: 30px;
        }

        .contact-links a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            opacity: 0.9;
            transition: opacity 0.3s ease;
        }

        .contact-links a:hover {
            opacity: 1;
            text-decoration: underline;
        }

        .main-content {
            display: grid;
            grid-template-columns: 1fr 300px;
            gap: 40px;
            padding: 40px;
        }

        .left-column {
            min-width: 0;
        }

        .right-column {
            position: relative;
        }

        .profile-image {
            width: 100%;
            height: 400px;
            background: #e9ecef;
            border-radius: 12px;
            margin-bottom: 20px;
            overflow: hidden;
            position: relative;
        }

        .profile-image::before {
            content: "👤";
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 4rem;
            opacity: 0.3;
        }

        .bio p {
            margin-bottom: 20px;
            font-size: 1.1rem;
            line-height: 1.7;
        }

        .bio a {
            color: #667eea;
            text-decoration: none;
            font-weight: 500;
        }

        .bio a:hover {
            text-decoration: underline;
        }

        .section {
            margin-top: 50px;
        }

        .section h2 {
            font-size: 1.8rem;
            margin-bottom: 30px;
            color: #2c3e50;
            position: relative;
            padding-bottom: 10px;
        }

        .section h2::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 50px;
            height: 3px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: 2px;
        }

        .date-range {
            color: #6c757d;
            font-size: 0.95rem;
            margin-bottom: 25px;
            font-style: italic;
        }

        .experience-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 25px;
            padding: 20px;
            background: #f8f9fa;
            border-radius: 10px;
            border-left: 4px solid #667eea;
            transition: all 0.3s ease;
        }

        .experience-item:hover {
            background: #e9ecef;
            transform: translateX(5px);
        }

        .experience-icon {
            width: 40px;
            height: 40px;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            font-size: 1.2rem;
            flex-shrink: 0;
        }

        .icon-ai { background: linear-gradient(135deg, #667eea, #764ba2); color: white; }
        .icon-robot { background: linear-gradient(135deg, #a8edea, #fed6e3); }
        .icon-scholar { background: linear-gradient(135deg, #ffecd2, #fcb69f); }
        .icon-stanford { background: linear-gradient(135deg, #ff9a9e, #fecfef); }
        .icon-university { background: linear-gradient(135deg, #a18cd1, #fbc2eb); }

        .experience-content h3 {
            font-size: 1.2rem;
            margin-bottom: 5px;
            color: #2c3e50;
        }

        .experience-role {
            color: #6c757d;
            font-size: 0.95rem;
        }

        .summary {
            background: #f8f9fa;
            padding: 30px;
            border-radius: 10px;
            margin-top: 30px;
        }

        .summary h3 {
            margin-bottom: 20px;
            color: #2c3e50;
            font-size: 1.3rem;
        }

        .summary ul {
            list-style: none;
        }

        .summary li {
            position: relative;
            padding-left: 25px;
            margin-bottom: 12px;
            line-height: 1.6;
        }

        .summary li::before {
            content: "▸";
            position: absolute;
            left: 0;
            color: #667eea;
            font-weight: bold;
        }

        .summary a {
            color: #667eea;
            text-decoration: none;
            font-weight: 500;
        }

        .summary a:hover {
            text-decoration: underline;
        }

        .frisbee-note {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 15px 20px;
            border-radius: 10px;
            text-align: center;
            font-style: italic;
            margin-top: 20px;
        }

        @media (max-width: 768px) {
            .main-content {
                grid-template-columns: 1fr;
                gap: 30px;
                padding: 30px 20px;
            }

            .header {
                padding: 30px 20px;
            }

            .header h1 {
                font-size: 2rem;
            }

            .profile-image {
                height: 250px;
            }

            .experience-item {
                flex-direction: column;
                text-align: center;
            }

            .experience-icon {
                margin: 0 auto 15px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Hello, I'm Evangel 👋</h1>
            <div class="contact-links">
                <a href="#">LinkedIn</a> | 
                <a href="mailto:shijentowterjsa@gmail.com">shijentowterjsa@gmail.com</a> | 
                <a href="#">Instagram</a>
            </div>
        </div>

        <div class="main-content">
            <div class="left-column">
                <div class="bio">
                    <p>Based in Los Angeles, I'm the Lead Developer for <a href="https://scholarbrilliance.com/">Scholar Brilliance</a>, an EdTech solution for students to live a debt-free college life.</p>
                    
                    <p>During my first and second years of University, I developed <a href="https://mychef.replit.app/">MyChef</a>, a recommendation system that provides users with healthy meals, based on their available ingredients at home. Additionally, I gathered training data for <a href="#">World Engine AI</a>'s advancements in robotics.</p>
                    
                    <p>Currently, I've partnered with <a href="https://www.siedu.org/">siEDU</a> to teach middle and high school students an introductory course to Artificial Intelligence. For more info on the course navigate <a href="https://www.notion.so/Intro-To-AI-23a5314941aa80e8d43f4da287748d4e">here</a>.</p>
                </div>

                <div class="section">
                    <h2>Experience & Education</h2>
                    <div class="date-range">As of 2023 - present</div>
                    
                    <div class="experience-item">
                        <div class="experience-icon icon-ai">🤖</div>
                        <div class="experience-content">
                            <h3>Intro to AI Instructor</h3>
                            <div class="experience-role">Using siEDU's curriculum</div>
                        </div>
                    </div>

                    <div class="experience-item">
                        <div class="experience-icon icon-robot">🔧</div>
                        <div class="experience-content">
                            <h3>World Engine AI</h3>
                            <div class="experience-role">Robotic Control Operator</div>
                        </div>
                    </div>

                    <div class="experience-item">
                        <div class="experience-icon icon-scholar">💡</div>
                        <div class="experience-content">
                            <h3>Scholar Brilliance</h3>
                            <div class="experience-role">Co-Founder and Lead Developer</div>
                        </div>
                    </div>

                    <div class="experience-item">
                        <div class="experience-icon icon-stanford">🎓</div>
                        <div class="experience-content">
                            <h3>Stanford Inspirit AI</h3>
                            <div class="experience-role">Ambassador</div>
                        </div>
                    </div>

                    <div class="experience-item">
                        <div class="experience-icon icon-university">🏫</div>
                        <div class="experience-content">
                            <h3>University of California, Santa Cruz</h3>
                            <div class="experience-role">BS in Computer Science & Game Design</div>
                        </div>
                    </div>
                </div>

                <div class="summary">
                    <h3>Summary</h3>
                    <ul>
                        <li>Tech professional based in Los Angeles with focus on educational technology and AI</li>
                        <li>Co-founder and Lead Developer at <a href="#">Scholar Brilliance</a>, creating EdTech solutions for debt-free college education</li>
                        <li>Developer of <a href="#">MyChef</a>, an AI-powered food recommendation system</li>
                        <li>Experienced in robotics data training with <a href="#">World Engine AI</a></li>
                        <li>Currently teaching AI to middle and high school students in <a href="#">partnership with siEDU</a></li>
                        <li>Strong background in both technical development and education</li>
                    </ul>
                </div>
            </div>

            <div class="right-column">
                <div class="profile-image"></div>
                <div class="frisbee-note">
                    I love playing Ultimate Frisbee, currently I play for the Men's D1 Club Team at UCSC!
                </div>
            </div>
        </div>
    </div>
</body>
</html>

