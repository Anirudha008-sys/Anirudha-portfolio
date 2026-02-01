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
        }

        body {
            font-family: 'Hind', 'Poppins', sans-serif;
            line-height: 1.5;
            color: #333;
            overflow-x: hidden;
            font-size: 15px;
        }

        /* Navigation - Smaller */
        nav {
            background: rgba(26, 26, 26, 0.95);
            padding: 0.6rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 10px rgba(0,0,0,0.2);
        }

        nav.scrolled {
            padding: 0.4rem 0;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 5px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: 600;
            padding: 0.4rem 0.8rem;
            border-radius: 20px;
            transition: all 0.3s;
            font-size: 0.85rem;
            display: flex;
            align-items: center;
            gap: 4px;
        }

        nav ul li a:hover {
            background: var(--primary-color);
        }

        /* Hero Section - Smaller fonts */
        .hero {
            margin-top: 50px;
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), 
                        url('photo1.jpg');
            background-size: cover;
            background-position: center;
            min-height: 85vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            position: relative;
        }

        .hero-content {
            z-index: 2;
            padding: 15px;
            animation: fadeInUp 0.8s ease;
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .hero img.profile-pic {
            width: 160px;
            height: 160px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid var(--primary-color);
            margin-bottom: 20px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.4);
        }

        .hero h1 {
            font-size: 2.2rem;
            margin-bottom: 8px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
            font-weight: 700;
        }

        .hero .tagline {
            font-size: 1.3rem;
            margin-bottom: 12px;
            color: var(--accent-color);
            font-weight: 600;
        }

        .hero .info {
            font-size: 0.95rem;
            margin-bottom: 20px;
            opacity: 0.9;
        }

        .btn-group {
            display: flex;
            gap: 10px;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 10px 25px;
            background: var(--primary-color);
            color: white;
            text-decoration: none;
            border-radius: 30px;
            font-weight: 600;
            font-size: 0.85rem;
            transition: all 0.3s;
            border: 2px solid var(--primary-color);
        }

        .btn:hover {
            background: transparent;
            transform: translateY(-2px);
        }

        .btn-outline {
            background: transparent;
            border: 2px solid white;
        }

        /* Stats Bar */
        .stats-bar {
            background: var(--secondary-color);
            color: white;
            padding: 25px 15px;
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
        }

        .stat-item {
            text-align: center;
        }

        .stat-item h3 {
            font-size: 1.8rem;
            color: var(--accent-color);
            margin-bottom: 3px;
        }

        .stat-item p {
            font-size: 0.85rem;
            opacity: 0.9;
        }

        /* Sections General - Smaller */
        section {
            padding: 50px 15px;
            max-width: 1100px;
            margin: 0 auto;
        }

        h2 {
            text-align: center;
            font-size: 1.8rem;
            margin-bottom: 30px;
            color: var(--secondary-color);
            position: relative;
            font-weight: 700;
        }

        h2::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background: var(--primary-color);
            margin: 10px auto;
            border-radius: 2px;
        }

        h2 i {
            color: var(--primary-color);
            margin-right: 8px;
            font-size: 1.5rem;
        }

        /* About Section */
        .about {
            background: #f9f9f9;
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            align-items: center;
        }

        .about-text p {
            font-size: 0.95rem;
            margin-bottom: 15px;
            text-align: justify;
            line-height: 1.6;
        }

        .skills-list {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 15px;
        }

        .skill-tag {
            background: var(--secondary-color);
            color: white;
            padding: 5px 12px;
            border-radius: 15px;
            font-size: 0.75rem;
            display: flex;
            align-items: center;
            gap: 4px;
        }

        .skill-tag i {
            color: var(--accent-color);
            font-size: 0.8rem;
        }

        /* Photo Gallery */
        .gallery {
            background: white;
        }

        .photo-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 15px;
        }

        .photo-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            cursor: pointer;
            aspect-ratio: 3/4;
            background: #f0f0f0;
        }

        .photo-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.4s;
            display: block;
        }

        .photo-item:hover img {
            transform: scale(1.08);
        }

        .photo-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(to top, rgba(0,0,0,0.8), transparent);
            color: white;
            padding: 15px;
            transform: translateY(100%);
            transition: transform 0.3s;
            font-size: 0.9rem;
        }

        .photo-item:hover .photo-overlay {
            transform: translateY(0);
        }

        .photo-item i {
            position: absolute;
            top: 10px;
            right: 10px;
            color: white;
            background: rgba(0,0,0,0.5);
            padding: 8px;
            border-radius: 50%;
            font-size: 0.8rem;
            opacity: 0;
            transition: all 0.3s;
        }

        .photo-item:hover i {
            opacity: 1;
        }

        /* Projects Section */
        .projects {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }

        .project-category {
            margin-bottom: 35px;
        }

        .project-category h3 {
            font-size: 1.3rem;
            color: var(--secondary-color);
            margin-bottom: 20px;
            padding-left: 15px;
            border-left: 4px solid var(--primary-color);
        }

        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .project-card {
            background: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            transition: all 0.3s;
            display: flex;
            flex-direction: column;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }

        .project-thumbnail {
            position: relative;
            height: 160px;
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
            width: 45px;
            height: 45px;
            background: rgba(255,255,255,0.95);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--primary-color);
            font-size: 1.1rem;
            transition: all 0.3s;
        }

        .project-card:hover .play-btn {
            transform: scale(1.1);
            background: var(--primary-color);
            color: white;
        }

        .project-info {
            padding: 18px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }

        .project-type {
            display: inline-block;
            background: var(--primary-color);
            color: white;
            padding: 4px 10px;
            border-radius: 12px;
            font-size: 0.7rem;
            margin-bottom: 8px;
            font-weight: 600;
            align-self: flex-start;
        }

        .project-info h4 {
            font-size: 1.1rem;
            color: var(--secondary-color);
            margin-bottom: 6px;
        }

        .project-info .director {
            color: #666;
            font-size: 0.8rem;
            margin-bottom: 6px;
            font-style: italic;
        }

        .project-info .role {
            font-weight: 600;
            color: var(--accent-color);
            margin-bottom: 10px;
            font-size: 0.9rem;
        }

        .watch-btn {
            margin-top: auto;
            display: inline-block;
            padding: 8px 18px;
            background: var(--secondary-color);
            color: white;
            text-decoration: none;
            border-radius: 20px;
            text-align: center;
            transition: all 0.3s;
            font-weight: 600;
            font-size: 0.8rem;
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
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
        }

        .work-item {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            border-left: 4px solid var(--primary-color);
            transition: all 0.3s;
        }

        .work-item:hover {
            transform: translateX(5px);
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }

        .work-item i {
            font-size: 1.8rem;
            color: var(--primary-color);
            margin-bottom: 10px;
        }

        .work-item h3 {
            font-size: 1.1rem;
            margin-bottom: 5px;
        }

        .work-item p {
            font-size: 0.8rem;
            color: #666;
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
            padding: 25px;
            border-radius: 15px;
            max-width: 700px;
            margin: 0 auto;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
        }

        .showreel-box h3 {
            font-size: 1.3rem;
            margin-bottom: 15px;
        }

        .showreel-box p {
            font-size: 0.9rem;
            margin-bottom: 20px;
        }

        .reel-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: 10px;
            margin-top: 20px;
        }

        .reel-link {
            background: var(--primary-color);
            color: white;
            padding: 10px;
            border-radius: 8px;
            text-decoration: none;
            transition: all 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 6px;
            font-weight: 600;
            font-size: 0.8rem;
        }

        .reel-link:hover {
            background: var(--accent-color);
            transform: translateY(-2px);
        }

        .physical-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 15px;
            margin-top: 20px;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.2);
        }

        .info-item h4 {
            color: var(--accent-color);
            font-size: 0.9rem;
            margin-bottom: 3px;
        }

        .info-item p {
            font-size: 0.85rem;
        }

        /* Contact */
        .contact {
            background: #1a1a1a;
            color: white;
            text-align: center;
            padding: 40px 15px;
        }

        .contact h2 {
            color: white;
            margin-bottom: 20px;
        }

        .contact > p {
            font-size: 1rem;
            margin-bottom: 25px;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
            margin: 30px 0;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 0.95rem;
        }

        .contact-item i {
            font-size: 1.1rem;
            color: var(--primary-color);
            width: 38px;
            height: 38px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .social-links {
            margin-top: 30px;
            display: flex;
            justify-content: center;
            gap: 12px;
        }

        .social-links a {
            width: 40px;
            height: 40px;
            background: rgba(255,255,255,0.1);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.1rem;
            transition: all 0.3s;
            text-decoration: none;
        }

        .social-links a:hover {
            background: var(--primary-color);
            transform: translateY(-3px);
        }

        footer {
            background: #0a0a0a;
            color: #666;
            text-align: center;
            padding: 15px;
            font-size: 0.8rem;
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
            max-height: 85%;
            border-radius: 8px;
        }

        .close-lightbox {
            position: absolute;
            top: 20px;
            right: 20px;
            color: white;
            font-size: 28px;
            cursor: pointer;
            width: 45px;
            height: 45px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s;
        }

        .close-lightbox:hover {
            background: var(--primary-color);
        }

        /* Scroll to Top */
        .scroll-top {
            position: fixed;
            bottom: 20px;
            right: 20px;
            width: 45px;
            height: 45px;
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
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
            font-size: 1.1rem;
        }

        .scroll-top.visible {
            opacity: 1;
        }

        .scroll-top:hover {
            background: var(--secondary-color);
            transform: translateY(-3px);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 1.8rem;
            }

            .hero .tagline {
                font-size: 1.1rem;
            }

            .hero img.profile-pic {
                width: 140px;
                height: 140px;
            }

            nav ul li a {
                padding: 0.3rem 0.6rem;
                font-size: 0.75rem;
            }

            h2 {
                font-size: 1.5rem;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .photo-grid {
                grid-template-columns: repeat(2, 1fr);
                gap: 10px;
            }

            .photo-item {
                aspect-ratio: 1/1.2;
            }

            .project-grid {
                grid-template-columns: 1fr;
            }

            .contact-info {
                flex-direction: column;
                gap: 15px;
            }

            .reel-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 480px) {
            .photo-grid {
                grid-template-columns: 1fr;
            }

            .stats-bar {
                gap: 20px 15px;
            }

            .stat-item h3 {
                font-size: 1.5rem;
            }
        }
    </style>
<base target="_blank">
</head>
<body>

    <!-- Navigation -->
    <nav id="navbar">
        <ul>
            <li><a href="#home"><i class="fas fa-home"></i> होम</a></li>
            <li><a href="#about"><i class="fas fa-user"></i> माहिती</a></li>
            <li><a href="#photos"><i class="fas fa-camera"></i> फोटो</a></li>
            <li><a href="#projects"><i class="fas fa-film"></i> प्रोजेक्ट्स</a></li>
            <li><a href="#audition"><i class="fas fa-video"></i> ऑडिशन</a></li>
            <li><a href="#contact"><i class="fas fa-phone"></i> संपर्क</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <img src="photo1.jpg" alt="Anirudha Devdikar" class="profile-pic">
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
            <p>कौशल्ये</p>
        </div>
    </div>

    <!-- About Section -->
    <section id="about" class="about">
        <h2><i class="fas fa-user-circle"></i> माझी ओळख</h2>
        <div class="about-content">
            <div class="about-text">
                <p>नमस्कार, मी अनिरुद्ध देवडीकर. मराठी चित्रपटसृष्टीतील एक उत्सुक अभिनेता. मी विनम्र स्वभावाचा आणि लवचिक व्यक्तिमत्वाचा धनी आहे.</p>
                <p>मी मुक्ती, वन टू का फोर, अ‍ॅक्टर्स आणि बॅशिंग या लोकप्रिय वेबसिरीजमध्ये काम केले आहे. धर्मरक्षक अहिल्यादेवी होळकर आणि सजना या मराठी चित्रपटांमध्ये महत्त्वाच्या भूमिका साकारल्या आहेत.</p>
                <p style="margin-top: 15px; font-weight: 600; color: var(--primary-color);">विशेष कौशल्ये:</p>
                <div class="skills-list">
                    <span class="skill-tag"><i class="fas fa-fire"></i> Real Stunt</span>
                    <span class="skill-tag"><i class="fas fa-hand-fist"></i> Real Fight</span>
                    <span class="skill-tag"><i class="fas fa-swimmer"></i> Swimming</span>
                    <span class="skill-tag"><i class="fas fa-horse"></i> Horse Riding</span>
                    <span class="skill-tag"><i class="fas fa-car"></i> Driving</span>
                    <span class="skill-tag"><i class="fas fa-bicycle"></i> Cycling</span>
                    <span class="skill-tag"><i class="fas fa-baseball-ball"></i> Cricket</span>
                    <span class="skill-tag"><i class="fas fa-futbol"></i> Football</span>
                </div>
            </div>
            <div class="about-image">
                <img src="photo2.jpg" alt="Anirudha on Bike" style="width: 100%; border-radius: 12px; box-shadow: 0 5px 15px rgba(0,0,0,0.15);">
            </div>
        </div>
    </section>

    <!-- Photo Gallery -->
    <section id="photos" class="gallery">
        <h2><i class="fas fa-images"></i> फोटो गॅलरी</h2>
        <div class="photo-grid">
            <div class="photo-item" onclick="openLightbox('photo1.jpg')">
                <img src="photo1.jpg" alt="Portfolio">
                <i class="fas fa-expand"></i>
                <div class="photo-overlay">
                    <strong>Portfolio Shot</strong><br>
                    <small>Professional</small>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('photo2.jpg')">
                <img src="photo2.jpg" alt="Action">
                <i class="fas fa-expand"></i>
                <div class="photo-overlay">
                    <strong>Action Look</strong><br>
                    <small>Bike Shoot</small>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('photo3.jpg')">
                <img src="photo3.jpg" alt="Artistic">
                <i class="fas fa-expand"></i>
                <div class="photo-overlay">
                    <strong>Artistic</strong><br>
                    <small>Black & White</small>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('photo4.jpg')">
                <img src="photo4.jpg" alt="Vintage">
                <i class="fas fa-expand"></i>
                <div class="photo-overlay">
                    <strong>Vintage Look</strong><br>
                    <small>Traditional</small>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('photo5.jpg')">
                <img src="photo5.jpg" alt="Intense">
                <i class="fas fa-expand"></i>
                <div class="photo-overlay">
                    <strong>Intense</strong><br>
                    <small>Character</small>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('photo6.jpg')">
                <img src="photo6.jpg" alt="Close Up">
                <i class="fas fa-expand"></i>
                <div class="photo-overlay">
                    <strong>Close Up</strong><br>
                    <small>Expression</small>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('photo7.jpg')">
                <img src="photo7.jpg" alt="Rural">
                <i class="fas fa-expand"></i>
                <div class="photo-overlay">
                    <strong>Rural Style</strong><br>
                    <small>Village</small>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('photo8.jpg')">
                <img src="photo8.jpg" alt="Traditional">
                <i class="fas fa-expand"></i>
                <div class="photo-overlay">
                    <strong>Traditional</strong><br>
                    <small>Ethnic Wear</small>
                </div>
            </div>
            <div class="photo-item" onclick="openLightbox('photo9.jpg')">
                <img src="photo9.jpg" alt="Royal">
                <i class="fas fa-expand"></i>
                <div class="photo-overlay">
                    <strong>Royal Character</strong><br>
                    <small>Historical</small>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects">
        <h2><i class="fas fa-film"></i> माझे प्रोजेक्ट्स</h2>

        <div class="project-category">
            <h3>🎬 वेबसिरीज</h3>
            <div class="project-grid">
                <div class="project-card">
                    <div class="project-thumbnail">
                        <i class="fas fa-play play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type">वेबसिरीज</span>
                        <h4>मुक्ती (Mukti)</h4>
                        <p class="role">मुख्य भूमिका</p>
                        <a href="https://youtu.be/VKy5G3M5HBg" target="_blank" class="watch-btn">
                            <i class="fab fa-youtube"></i> पहा
                        </a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-thumbnail">
                        <i class="fas fa-play play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type">वेबसिरीज</span>
                        <h4>वन टू का फोर</h4>
                        <p class="role">मुख्य भूमिका</p>
                        <a href="https://youtu.be/KeqDqxl6Hm0" target="_blank" class="watch-btn">
                            <i class="fab fa-youtube"></i> पहा
                        </a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-thumbnail">
                        <i class="fas fa-play play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type">वेबसिरीज</span>
                        <h4>अ‍ॅक्टर्स (Actors)</h4>
                        <p class="director">जलिंदर कुंभार सर</p>
                        <p class="role">मुख्य भूमिका</p>
                        <a href="https://youtu.be/C7xbLRCRbEM" target="_blank" class="watch-btn">
                            <i class="fab fa-youtube"></i> पहा
                        </a>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-thumbnail">
                        <i class="fas fa-play play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type">वेबसिरीज</span>
                        <h4>बॅशिंग (Bashing)</h4>
                        <p class="director">योगेश गडगे</p>
                        <p class="role">मुख्य भूमिका</p>
                        <a href="https://youtu.be/DOKvfjyqmUI" target="_blank" class="watch-btn">
                            <i class="fab fa-youtube"></i> पहा
                        </a>
                    </div>
                </div>
            </div>
        </div>

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
                        <p class="director">सुशांत सोनवले सर</p>
                        <p class="role">सरसेनापती बर्गळ</p>
                    </div>
                </div>

                <div class="project-card">
                    <div class="project-thumbnail" style="background: linear-gradient(135deg, #e74c3c, #f39c12);">
                        <i class="fas fa-running play-btn"></i>
                    </div>
                    <div class="project-info">
                        <span class="project-type" style="background: #e74c3c;">चित्रपट</span>
                        <h4>सजना (Sajana)</h4>
                        <p class="role">प्रतिस्पर्धी भूमिका</p>
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
                <p>4-5 अल्बम गाण्यांमध्ये पार्श्वभूमी नर्तक</p>
            </div>
            <div class="work-item">
                <i class="fas fa-star"></i>
                <h3>विशेष कौशल्ये</h3>
                <p>Stunt, Fight, Sports</p>
            </div>
            <div class="work-item">
                <i class="fas fa-theater-masks"></i>
                <h3>अभिनय शैली</h3>
                <p>विनम्र स्वभाव, लवचिक</p>
            </div>
        </div>
    </section>

    <!-- Audition Section -->
    <section id="audition" class="audition">
        <h2><i class="fas fa-video"></i> Casting Directors</h2>
        <div class="showreel-box">
            <h3>🎥 Showreel Links</h3>
            <p>माझे सर्व प्रोजेक्ट्सचे लिंक्स:</p>

            <div class="reel-grid">
                <a href="https://youtu.be/VKy5G3M5HBg" target="_blank" class="reel-link">
                    <i class="fab fa-youtube"></i> मुक्ती
                </a>
                <a href="https://youtu.be/KeqDqxl6Hm0" target="_blank" class="reel-link">
                    <i class="fab fa-youtube"></i> वन टू का फोर
                </a>
                <a href="https://youtu.be/C7xbLRCRbEM" target="_blank" class="reel-link">
                    <i class="fab fa-youtube"></i> अ‍ॅक्टर्स
                </a>
                <a href="https://youtu.be/DOKvfjyqmUI" target="_blank" class="reel-link">
                    <i class="fab fa-youtube"></i> बॅशिंग
                </a>
            </div>

            <div class="physical-info">
                <div class="info-item">
                    <h4>वय</h4>
                    <p>29</p>
                </div>
                <div class="info-item">
                    <h4>उंची</h4>
                    <p>5'8"</p>
                </div>
                <div class="info-item">
                    <h4>भाषा</h4>
                    <p>मराठी, हिंदी</p>
                </div>
                <div class="info-item">
                    <h4>ठिकाण</h4>
                    <p>पुणे</p>
                </div>
            </div>

            <div style="margin-top: 20px; padding: 15px; background: rgba(231, 76, 60, 0.2); border-radius: 8px; border: 2px solid var(--primary-color); font-size: 0.85rem;">
                <strong style="color: var(--accent-color);">स्टंट, स्विमिंग, हॉर्स राइडिंग, ड्रायव्हिंग, स्पोर्ट्स</strong>
            </div>
        </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="contact">
        <h2><i class="fas fa-address-card"></i> संपर्क</h2>
        <p>नवीन प्रोजेक्ट्ससाठी मला संपर्क करा</p>

        <div class="contact-info">
            <div class="contact-item">
                <i class="fas fa-envelope"></i>
                <div>
                    anidevadikar008@gmail.com
                </div>
            </div>
            <div class="contact-item">
                <i class="fas fa-phone"></i>
                <div>
                    +91 98902 24073
                </div>
            </div>
            <div class="contact-item">
                <i class="fas fa-map-marker-alt"></i>
                <div>
                    पुणे, महाराष्ट्र
                </div>
            </div>
        </div>

        <div class="social-links">
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-youtube"></i></a>
            <a href="#"><i class="fab fa-whatsapp"></i></a>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 अनिरुद्ध देवडीकर. सर्व हक्क राखीव.</p>
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

        // Smooth scrolling for nav links
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
    </script>

</body>
</html>
    </script>

</body>
</html>
