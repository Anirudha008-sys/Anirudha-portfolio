<!DOCTYPE html>
<html lang="mr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anirudha Devdikar - Actor | Marathi Cinema</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Hind:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-color: #e74c3c;
            --secondary-color: #2c3e50;
            --accent-color: #f39c12;
            --text-light: #ecf0f1;
            --bg-dark: #1a1a1a;
            --gradient-hero: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }

        body {
            font-family: 'Hind', 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
            overflow-x: hidden;
        }

        /* Navigation */
        nav {
            background: rgba(26, 26, 26, 0.95);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 20px rgba(0,0,0,0.3);
            transition: all 0.3s ease;
        }

        nav.scrolled {
            padding: 0.5rem 0;
            background: rgba(26, 26, 26, 0.98);
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: 600;
            padding: 0.5rem 1.2rem;
            border-radius: 25px;
            transition: all 0.3s;
            font-size: 1rem;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        nav ul li a:hover {
            background: var(--primary-color);
            transform: translateY(-2px);
        }

        /* Hero Section */
        .hero {
            margin-top: 0;
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), 
                        url('photo1.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            position: relative;
        }

        .hero-content {
            z-index: 2;
            padding: 20px;
            animation: fadeInUp 1s ease;
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
            }

        .hero img.profile-pic {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid var(--primary-color);
            margin-bottom: 30px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.5);
            transition: transform 0.3s;
        }

        .hero img.profile-pic:hover {
            transform: scale(1.05);
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
            font-weight: 700;
        }

        .hero .tagline {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--accent-color);
            font-weight: 600;
        }

        .hero .info {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0.9;
        }

        .btn-group {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 12px 35px;
            background: var(--primary-color);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            transition: all 0.3s;
            border: 2px solid var(--primary-color);
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .btn:hover {
            background: transparent;
            color: white;
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.3);
        }

        .btn-outline {
            background: transparent;
            border: 2px solid white;
        }

        .btn-outline:hover {
            background: white;
            color: var(--secondary-color);
        }

        /* Stats Bar */
        .stats-bar {
            background: var(--secondary-color);
            color: white;
            padding: 40px 20px;
            display: flex;
            justify-content: center;
            gap: 50px;
            flex-wrap: wrap;
        }

        .stat-item {
            text-align: center;
        }

        .stat-item h3 {
            font-size: 2.5rem;
            color: var(--accent-color);
            margin-bottom: 5px;
        }

        .stat-item p {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        /* Sections General */
        section {
            padding: 80px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        h2 {
            text-align: center;
            font-size: 2.8rem;
            margin-bottom: 50px;
            color: var(--secondary-color);
            position: relative;
            font-weight: 700;
        }

        h2::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: var(--primary-color);
            margin: 15px auto;
            border-radius: 2px;
        }

        h2 i {
            color: var(--primary-color);
            margin-right: 10px;
        }

        /* About Section */
        .about {
            background: #f9f9f9;
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about-text p {
            font-size: 1.1rem;
            margin-bottom: 20px;
            text-align: justify;
        }

        .skills-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 20px;
        }

        .skill-tag {
            background: var(--secondary-color);
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .skill-tag i {
            color: var(--accent-color);
        }

        /* Photo Gallery */
        .gallery {
            background: white;
        }

        .photo-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .photo-item {
            position: relative;
            overflow: hidden;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            cursor: pointer;
            aspect-ratio: 3/4;
        }

        .photo-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }

        .photo-item:hover img {
            transform: scale(1.1);
        }

        .photo-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(to top, rgba(0,0,0,0.8), transparent);
            color: white;
            padding: 20px;
            transform: translateY(100%);
            transition: transform 0.3s;
        }

        .photo-item:hover .photo-overlay {
            transform: translateY(0);
        }

        /* Projects Section */
        .projects {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }

        .project-category {
            margin-bottom: 50px;
        }

        .project-category h3 {
            font-size: 1.8rem;
            color: var(--secondary-color);
            margin-bottom: 30px;
            padding-left: 20px;
            border-left: 5px solid var(--primary-color);
        }

        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
        }

        .project-card {
            background: white;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.3s;
            display: flex;
            flex-direction: column;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.2);
        }

        .project-thumbnail {
            position: relative;
            height: 220px;
            background: var(--secondary-color);
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }

        .project-thumbnail img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .play-btn {
            position: absolute;
            width: 60px;
            height: 60px;
            background: rgba(255,255,255,0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--primary-color);
            font-size: 1.5rem;
            transition: all 0.3s;
        }

        .project-card:hover .play-btn {
            transform: scale(1.1);
            background: var(--primary-color);
            color: white;
        }

        .project-info {
            padding: 25px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }

        .project-type {
            display: inline-block;
            background: var(--primary-color);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.85rem;
            margin-bottom: 10px;
            font-weight: 600;
            align-self: flex-start;
        }

        .project-info h4 {
            font-size: 1.4rem;
            color: var(--secondary-color);
            margin-bottom: 10px;
        }

        .project-info .director {
            color: #666;
            font-size: 0.95rem;
            margin-bottom: 10px;
            font-style: italic;
        }

        .project-info .role {
            font-weight: 600;
            color: var(--accent-color);
            margin-bottom: 15px;
        }

        .watch-btn {
            margin-top: auto;
            display: inline-block;
            padding: 10px 25px;
            background: var(--secondary-color);
            color: white;
            text-decoration: none;
            border-radius: 25px;
            text-align: center;
            transition: all 0.3s;
            font-weight: 600;
        }

        .watch-btn:hover {
            background: var(--primary-color);
        }

        /* Other Work */
        .other-work {
            background: white;
        }

        .work-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .work-item {
            background: #f8f9fa;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            border-left: 5px solid var(--primary-color);
            transition: all 0.3s;
        }

        .work-item:hover {
            transform: translateX(10px);
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        }

        .work-item i {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        /* Audition Section */
        .audition {
            background: var(--secondary-color);
            color: white;
            text-align: center;
        }

        .audition h2 {
            color: white;
        }

        .audition h2::after {
            background: var(--accent-color);
        }

        .showreel-box {
            background: rgba(255,255,255,0.1);
            padding: 40px;
            border-radius: 20px;
            max-width: 800px;
            margin: 0 auto;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
        }

        .showreel-box h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
        }

        .reel-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-top: 30px;
        }

        .reel-link {
            background: var(--primary-color);
            color: white;
            padding: 15px;
            border-radius: 10px;
            text-decoration: none;
            transition: all 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            font-weight: 600;
        }

        .reel-link:hover {
            background: var(--accent-color);
            transform: translateY(-3px);
        }

        .physical-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            margin-top: 30px;
            padding-top: 30px;
            border-top: 1px solid rgba(255,255,255,0.2);
        }

        .info-item h4 {
            color: var(--accent-color);
            font-size: 1.2rem;
            margin-bottom: 5px;
        }

        /* Contact */
        .contact {
            background: #1a1a1a;
            color: white;
            text-align: center;
        }

        .contact h2 {
            color: white;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 50px;
            flex-wrap: wrap;
            margin: 40px 0;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.2rem;
        }

        .contact-item i {
            font-size: 1.5rem;
            color: var(--primary-color);
            width: 50px;
            height: 50px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .social-links {
            margin-top: 40px;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        .social-links a {
            width: 50px;
            height: 50px;
            background: rgba(255,255,255,0.1);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.3rem;
            transition: all 0.3s;
            text-decoration: none;
        }

        .social-links a:hover {
            background: var(--primary-color);
            transform: translateY(-5px);
        }

        footer {
            background: #0a0a0a;
            color: #666;
            text-align: center;
            padding: 20px;
        }

        /* Lightbox */
        .lightbox {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.95);
            z-index: 2000;
            justify-content: center;
            align-items: center;
        }

        .lightbox.active {
            display: flex;
        }

        .lightbox img {
            max-width: 90%;
            max-height: 90%;
            border-radius: 10px;
            box-shadow: 0 0 40px rgba(0,0,0,0.5);
        }

        .close-lightbox {
            position: absolute;
            top: 30px;
            right: 40px;
            color: white;
            font-size: 40px;
            cursor: pointer;
            width: 50px;
            height: 50px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s;
        }

        .close-lightbox:hover {
            background: var(--primary-color);
            transform: rotate(90deg);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.2rem;
            }

            .hero .tagline {
                font-size: 1.2rem;
            }

            nav ul {
                gap: 5px;
            }

            nav ul li a {
                padding: 0.4rem 0.8rem;
                font-size: 0.9rem;
            }

            h2 {
                font-size: 2rem;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .project-grid {
                grid-template-columns: 1fr;
            }

            .stats-bar {
                gap: 20px;
            }

            .contact-info {
                flex-direction: column;
                gap: 20px;
            }
        }

        .scroll-top {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 50px;
            height: 50px;
            background: var(--primary-color);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            opacity: 0;
            transition: all 0.3s;
            z-index: 999;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
        }

        .scroll-top.visible {
            opacity: 1;
        }

        .scroll-top:hover {
            background: var(--secondary-color);
            transform: translateY(-5px);
        }
    </style>
<base target="_blank">
</head>
<body>

    <!-- Navigation -->
    <nav id="navbar">
        <ul>
            <li><a href="#home" onclick="scrollToSection('home')"><i class="fas fa-home"></i> होम</a></li>
            <li><a href="#about" onclick="scrollToSection('about')"><i class="fas fa-user"></i> माहिती</a></li>
            <li><a href="#photos" onclick="scrollToSection('photos')"><i class="fas fa-camera"></i> फोटो</a></li>
            <li><a href="#projects" onclick="scrollToSection('projects')"><i class="fas fa-film"></i> प्रोजेक्ट्स</a></li>
            <li><a href="#audition" onclick="scrollToSection('audition')"><i class="fas fa-video"></i> ऑडिशन</a></li>
            <li><a href="#contact" onclick="scrollToSection('contact')"><i class="fas fa-phone"></i> संपर्क</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <img src="WhatsApp Image 2026-02-01 at 12.42.03 PM - Copy.jpeg" alt="Anirudha Devdikar" class="profile-pic">
            <h1>अनिरुद्ध देवडीकर</h1>
            <p class="tagline">Anirudha Devdikar</p>
            <p class="info">🎭 अभिनेता | वय: 29 | पुणे, महाराष्ट्र</p>
            <div class="btn-group">
                <a href="#projects" class="btn"><i class="fas fa-play"></i> माझे काम पहा</a>
                <a href="#contact" class="btn btn-outline"><i class="fas fa-envelope"></i> संपर्क करा</a>
            </div>
        </div>
    </section>

    <!-- Stats Bar -->
    <div class="stats-bar">
        <div class="stat-item">
            <h3>4+</h3>
            <p>वेबसिरीज</p>
        </div>
        <div class="stat-item">
            <h3>2+</h3>
            <p>मराठी चित्रपट</p>
        </div>
        <div class="stat-item">
            <h3>5+</h3>
            <p>अल्बम गाणी</p>
        </div>
        <div class="stat-item">
            <h3>10+</h3>
            <p>विविध कौशल्ये</p>
        </div>
    </div>

    <!-- About Section -->
    <section id="about" class="about">
        <h2><i class="fas fa-user-circle"></i> माझी ओळख</h2>
        <div class="about-content">
            <div class="about-text">
                <p>नमस्कार, मी अनिरुद्ध देवडीकर. मराठी चित्रपटसृष्टीतील एक उत्सुक अभिनेता. मी विनम्र स्वभावाचा आणि लवचिक व्यक्तिमत्वाचा धनी आहे.</p>
                <p>मी मुक्ती, वन टू का फोर, अ‍ॅक्टर्स आणि बॅशिंग या लोकप्रिय वेबसिरीजमध्ये काम केले आहे. धर्मरक्षक अहिल्यादेवी होळकर आणि सजना या मराठी चित्रपटांमध्ये महत्त्वाच्या भूमिका साकारल्या आहेत.</p>
                <p style="margin-top: 20px; font-weight: 600; color: var(--primary-color);">विशेष कौशल्ये:</p>
                <div class="skills-list">
                    <span class="skill-tag"><i class="fas fa-fire"></i> Real Stunt</span>
                    <span class="skill-tag"><i class="fas fa-hand-fist"></i> Real Fight</span>
                    <span class="skill-tag"><i class="fas fa-swimmer"></i> Swimming</span>
                    <span class="skill-tag"><i class="fas fa-horse"></i> Horse Riding</span>
                    <span class="skill-tag"><i class="fas fa-car"></i> Driving</span>
                    <span class="skill-tag"><i class="fas fa-bicycle"></i> Cycling</span>
                    <span class="skill-tag"><i class="fas fa-baseball-ball"></i> Cricket</span>
                    <span class="skill-tag"><i class="fas fa-futbol"></i> Football</span>
                    <span class="skill-tag"><i class="fas fa-running"></i> Sports</span>
                </div>
            </div>
            <div class="about-image">
                <img src="WhatsApp Image 2026-02-01 at 12.42.02 PM (1) - Copy.jpeg" alt="Anirudha on Bike" style="width: 100%; border-radius: 20px; box-shadow: 0 10px 30px rgba(0,0,0,0.2);">
            </div>
        </div>
    </section>

    <!-- Photo Gallery -->
    <section id="photos" class="gallery">
        <h2><i class="fas fa-images"></i> फोटो गॅलरी</h2>
        <div class="photo-grid">
            <div class="photo-item" onclick="openLightbox('WhatsApp Image 2026-02-01 at 12.42.03 PM - Copy.jpeg')">
                <img src="WhatsApp Image 2026-02-01 at 12.42.03 PM - Copy.jpeg" alt="Portfolio 1">
                <div class="photo-overlay">
                    <h4>Portfolio Shot</h4>
                    <p>Professional Headshot</p>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('WhatsApp Image 2026-02-01 at 12.42.02 PM (1) - Copy.jpeg')">
                <img src="WhatsApp Image 2026-02-01 at 12.42.02 PM (1) - Copy.jpeg" alt="On Bike">
                <div class="photo-overlay">
                    <h4>Action Look</h4>
                    <p>Bike Shoot</p>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('WhatsApp Image 2026-02-01 at 12.42.02 PM.jpeg')">
                <img src="WhatsApp Image 2026-02-01 at 12.42.02 PM.jpeg" alt="Umbrella Black White">
                <div class="photo-overlay">
                    <h4>Artistic</h4>
                    <p>Black & White</p>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('WhatsApp Image 2026-02-01 at 12.42.01 PM (1) - Copy.jpeg')">
                <img src="WhatsApp Image 2026-02-01 at 12.42.01 PM (1) - Copy.jpeg" alt="Umbrella">
                <div class="photo-overlay">
                    <h4>Vintage Look</h4>
                    <p>Traditional Style</p>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('WhatsApp Image 2026-02-01 at 12.42.01 PM.jpeg')">
                <img src="WhatsApp Image 2026-02-01 at 12.42.01 PM.jpeg" alt="Temple Scene">
                <div class="photo-overlay">
                    <h4>Intense</h4>
                    <p>Character Look</p>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('WhatsApp Image 2026-02-01 at 12.42.00 PM (2).jpeg')">
                <img src="WhatsApp Image 2026-02-01 at 12.42.00 PM (2).jpeg" alt="Black White Closeup">
                <div class="photo-overlay">
                    <h4>Close Up</h4>
                    <p>Expression</p>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('WhatsApp Image 2026-02-01 at 12.42.00 PM (1).jpeg')">
                <img src="WhatsApp Image 2026-02-01 at 12.42.00 PM (1).jpeg" alt="Rural Look">
                <div class="photo-overlay">
                    <h4>Rural Style</h4>
                    <p>Village Character</p>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('WhatsApp Image 2026-02-01 at 12.42.00 PM.jpeg')">
                <img src="WhatsApp Image 2026-02-01 at 12.42.00 PM.jpeg" alt="Traditional">
                <div class="photo-overlay">
                    <h4>Traditional</h4>
                    <p>Ethnic Wear</p>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('WhatsApp Image 2026-02-01 at 12.41.59 PM.jpeg')">
                <img src="WhatsApp Image 2026-02-01 at 12.41.59 PM.jpeg" alt="Royal Look">
                <div class="photo-overlay">
                    <h4>Royal Character</h4>
                    <p>Historical Role</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects">
        <h2><i class="fas fa-film"></i> माझे प्रोजेक्ट्स</h2>

        <!-- Web Series -->
        <div class="project-category">
            <h3>🎬 वेबसिरीज</h3>
            <div class="project-grid">
                <div class="project-card">
                    <div class="project-thumbnail">
                        <i class="fas fa-play-circle play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type">वेबसिरीज</span>
                        <h4>मुक्ती (Mukti)</h4>
                        <p class="role">मुख्य भूमिका</p>
                        <a href="https://youtu.be/VKy5G3M5HBg?si=PSn1YwSYgmcLaCKU" target="_blank" class="watch-btn">
                            <i class="fab fa-youtube"></i> पहा
                        </a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-thumbnail">
                        <i class="fas fa-play-circle play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type">वेबसिरीज</span>
                        <h4>वन टू का फोर (One Two Ka Four)</h4>
                        <p class="role">मुख्य भूमिका</p>
                        <a href="https://youtu.be/KeqDqxl6Hm0?si=Ddew1cxbV3q0I6hi" target="_blank" class="watch-btn">
                            <i class="fab fa-youtube"></i> पहा
                        </a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-thumbnail">
                        <i class="fas fa-play-circle play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type">वेबसिरीज</span>
                        <h4>अ‍ॅक्टर्स (Actors)</h4>
                        <p class="director">दिग्दर्शक: जलिंदर कुंभार सर</p>
                        <p class="role">मुख्य भूमिका</p>
                        <a href="https://youtu.be/C7xbLRCRbEM?si=dKRdzHWmWenPW5Pr" target="_blank" class="watch-btn">
                            <i class="fab fa-youtube"></i> पहा
                        </a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-thumbnail">
                        <i class="fas fa-play-circle play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type">वेबसिरीज</span>
                        <h4>बॅशिंग (Bashing)</h4>
                        <p class="director">दिग्दर्शक: योगेश गडगे</p>
                        <p class="role">मुख्य भूमिका</p>
                        <a href="https://youtu.be/DOKvfjyqmUI?si=gmnHd6X0rfWrf-Ht" target="_blank" class="watch-btn">
                            <i class="fab fa-youtube"></i> पहा
                        </a>
                    </div>
                </div>
            </div>
        </div>

        <!-- Movies -->
        <div class="project-category">
            <h3>🎞️ मराठी चित्रपट</h3>
            <div class="project-grid">
                <div class="project-card">
                    <div class="project-thumbnail" style="background: linear-gradient(135deg, #8e44ad, #3498db);">
                        <i class="fas fa-crown play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type" style="background: #8e44ad;">चित्रपट</span>
                        <h4>धर्मरक्षक अहिल्यादेवी होळकर</h4>
                        <p class="director">दिग्दर्शक: सुशांत सोनवले सर</p>
                        <p class="role">सरसेनापती बर्गळ (सततची भूमिका)</p>
                        <p style="margin-top: 10px; font-size: 0.9rem; color: #666;">ऐतिहासिक चित्रपटातील महत्त्वाची भूमिका</p>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-thumbnail" style="background: linear-gradient(135deg, #e74c3c, #f39c12);">
                        <i class="fas fa-running play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type" style="background: #e74c3c;">चित्रपट</span>
                        <h4>सजना (Sajana)</h4>
                        <p class="role">प्रतिस्पर्धी भूमिका (क्रीडा विषयक)</p>
                        <p style="margin-top: 10px; font-size: 0.9rem; color: #666;">मुख्य अभिनetyाच्या विरुद्ध भूमिका</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Other Work -->
    <section class="other-work">
        <h2><i class="fas fa-music"></i> इतर कामे</h2>
        <div class="work-list">
            <div class="work-item">
                <i class="fas fa-compact-disc"></i>
                <h3>अल्बम गाणी</h3>
                <p>4-5 अल्बम गाण्यांमध्ये पार्श्वभूमी नर्तक म्हणून काम</p>
            </div>
            <div class="work-item">
                <i class="fas fa-star"></i>
                <h3>विशेष कौशल्ये</h3>
                <p>Stunt, Fight, Sports अनुभवी कलाकार</p>
            </div>
            <div class="work-item">
                <i class="fas fa-theater-masks"></i>
                <h3>अभिनय शैली</h3>
                <p>विनम्र स्वभाव, लवचिक व्यक्तिमत्व</p>
            </div>
        </div>
    </section>

    <!-- Audition Section -->
    <section id="audition" class="audition">
        <h2><i class="fas fa-video"></i> Casting Directors साठी</h2>
        <div class="showreel-box">
            <h3>🎥 माझे Showreel Links</h3>
            <p>माझे सर्व प्रोजेक्ट्सचे थेट लिंक्स:</p>

            <div class="reel-grid">
                <a href="https://youtu.be/VKy5G3M5HBg?si=PSn1YwSYgmcLaCKU" target="_blank" class="reel-link">
                    <i class="fab fa-youtube"></i> मुक्ती
                </a>
                <a href="https://youtu.be/KeqDqxl6Hm0?si=Ddew1cxbV3q0I6hi" target="_blank" class="reel-link">
                    <i class="fab fa-youtube"></i> वन टू का फोर
                </a>
                <a href="https://youtu.be/C7xbLRCRbEM?si=dKRdzHWmWenPW5Pr" target="_blank" class="reel-link">
                    <i class="fab fa-youtube"></i> अ‍ॅक्टर्स
                </a>
                <a href="https://youtu.be/DOKvfjyqmUI?si=gmnHd6X0rfWrf-Ht" target="_blank" class="reel-link">
                    <i class="fab fa-youtube"></i> बॅशिंग
                </a>
            </div>

            <div class="physical-info">
                <div class="info-item">
                    <h4>वय</h4>
                    <p>29 वर्षे</p>
                </div>
                <div class="info-item">
                    <h4>उंची</h4>
                    <p>5'8" (अंदाजे)</p>
                </div>
                <div class="info-item">
                    <h4>भाषा</h4>
                    <p>मराठी, हिंदी, इंग्रजी</p>
                </div>
                <div class="info-item">
                    <h4>ठिकाण</h4>
                    <p>पुणे, महाराष्ट्र</p>
                </div>
            </div>

            <div style="margin-top: 30px; padding: 20px; background: rgba(231, 76, 60, 0.2); border-radius: 10px; border: 2px solid var(--primary-color);">
                <h4 style="color: var(--accent-color); margin-bottom: 10px;">⚡ विशेष कौशल्ये:</h4>
                <p>Real Stunt | Real Fight | Swimming | Horse Riding | Driving | Cycling | Cricket | Football | Any Sports</p>
            </div>
        </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="contact">
        <h2><i class="fas fa-address-card"></i> संपर्क करा</h2>
        <p style="font-size: 1.3rem; margin-bottom: 30px; opacity: 0.9;">नवीन प्रोजेक्ट्ससाठी मला संपर्क करा</p>

        <div class="contact-info">
            <div class="contact-item">
                <i class="fas fa-envelope"></i>
                <div>
                    <strong>ईमेल</strong><br>
                    anidevadikar008@gmail.com
                </div>
            </div>
            <div class="contact-item">
                <i class="fas fa-phone"></i>
                <div>
                    <strong>फोन</strong><br>
                    +91 98902 24073
                </div>
            </div>
            <div class="contact-item">
                <i class="fas fa-map-marker-alt"></i>
                <div>
                    <strong>ठिकाण</strong><br>
                    पुणे, महाराष्ट्र
                </div>
            </div>
        </div>

        <div class="social-links">
            <a href="#" title="Instagram"><i class="fab fa-instagram"></i></a>
            <a href="#" title="Facebook"><i class="fab fa-facebook-f"></i></a>
            <a href="#" title="YouTube"><i class="fab fa-youtube"></i></a>
            <a href="#" title="WhatsApp"><i class="fab fa-whatsapp"></i></a>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 अनिरुद्ध देवडीकर. सर्व हक्क राखीव.</p>
        <p style="margin-top: 10px; font-size: 0.9rem;">Made with ❤️ for Marathi Cinema</p>
    </footer>

    <!-- Lightbox -->
    <div class="lightbox" id="lightbox" onclick="closeLightbox()">
        <span class="close-lightbox">&times;</span>
        <img src="" alt="Full size" id="lightbox-img">
    </div>

    <!-- Scroll to Top -->
    <div class="scroll-top" id="scrollTop" onclick="window.scrollTo({top: 0, behavior: 'smooth'})">
        <i class="fas fa-arrow-up"></i>
    </div>

    <script>
        // Smooth scrolling for navigation
        function scrollToSection(id) {
            const element = document.getElementById(id);
            if (element) {
                element.scrollIntoView({ behavior: 'smooth' });
            }
        }

        // Lightbox functionality
        function openLightbox(src) {
            const lightbox = document.getElementById('lightbox');
            const lightboxImg = document.getElementById('lightbox-img');
            lightboxImg.src = src;
            lightbox.classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        function closeLightbox() {
            document.getElementById('lightbox').classList.remove('active');
            document.body.style.overflow = 'auto';
        }

        // Navbar scroll effect
        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            const scrollTop = document.getElementById('scrollTop');

            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
                scrollTop.classList.add('visible');
            } else {
                navbar.classList.remove('scrolled');
                scrollTop.classList.remove('visible');
            }
        });

        // Close lightbox on Escape key
        document.addEventListener('keydown', function(e) {
            if (e.key === 'Escape') {
                closeLightbox();
            }
        });
    </script>

</body>
</html>
