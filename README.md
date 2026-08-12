
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rank Keywords - Digital Marketing, Coding, Graphics & Video Training</title>
    
    <link rel="icon" href="/uploads/images/siteicon.webp" type="image/webp">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />

    <style>
        :root {
            --primary-blue: #0a4299;
            --hero-blue: #0a57cc;
            --accent-yellow: #ffc107;
            --dark-blue: #052a6b;
            --white: #ffffff;
        }

        @font-face {
          font-family: 'Banco';
          src: url('fonts/Banco.ttf') format('truetype');
          font-weight: normal;
          font-style: normal;
          font-display: swap;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f8f9fa;
            color: #333;
            overflow-x: hidden;
        }

        /* ========= MODERN NAVBAR ========= */
        .navbar {
            padding: 15px 5vw; 
            background: rgba(10, 87, 204, 0.95) !important;
            backdrop-filter: blur(15px);
            border-bottom: 1px solid rgba(255,255,255,0.1);
            transition: all 0.4s;
        }
        .navbar.scrolled {
            padding: 10px 5vw;
            background: rgba(5, 42, 107, 0.98) !important;
            box-shadow: 0 4px 30px rgba(0,0,0,0.2);
        }
        
        .navbar > .container {
            flex-wrap: nowrap !important;
        }
        
        .navbar-brand {
            font-family: 'Banco', cursive;
            font-size: clamp(2rem, 5vw, 2.3rem) !important;
            color: #fff !important;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2); 
            white-space: nowrap;
        }
        
        .navbar .nav-link {
            color: rgba(255,255,255,0.85) !important;
            font-weight: 500;
            padding: 10px 18px !important;
            transition: 0.3s;
        }
        .navbar .nav-link:hover, .navbar .nav-link.active {
            color: var(--accent-yellow) !important;
        }
        
        .navbar-toggler {
            border-color: rgba(255,255,255,0.3) !important;
            padding: 6px 10px;
        }

        .btn-download-app {
            background: var(--accent-yellow);
            color: #000 !important;
            font-weight: 700;
            border-radius: 50px;
            padding: 10px 24px !important;
            box-shadow: 0 4px 15px rgba(255,193,7,0.3);
            text-decoration: none;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
        }
        .btn-download-app:hover {
            transform: translateY(-2px);
            background: #e0a800;
        }

        /* ========= NEW MOBILE SLIDE-IN MENU ========= */
        .mobile-slide-menu {
            position: fixed;
            top: 0; left: 0; right: 0; bottom: 0;
            background: #ffffff;
            z-index: 2000;
            transform: translateX(100%);
            transition: transform 0.3s ease-in-out;
            display: flex;
            flex-direction: column;
        }
        .mobile-slide-menu.open {
            transform: translateX(0);
        }
        .mobile-menu-header {
            padding: 24px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #f1f5f9;
        }
        .mobile-brand {
            font-family: 'Banco', cursive;
            font-size: 1.8rem;
            color: var(--primary-blue);
        }
        .mobile-close-btn {
            background: #f8fafc;
            border: none;
            border-radius: 50%;
            width: 44px; height: 44px;
            font-size: 1.2rem;
            color: #334155;
            display: flex; justify-content: center; align-items: center;
        }
        .mobile-menu-body {
            padding: 32px 24px;
            display: flex; flex-direction: column; gap: 24px;
            overflow-y: auto;
        }
        .mobile-link {
            font-size: 1.25rem;
            font-weight: 700;
            color: #1e293b;
            text-decoration: none;
            display: flex; align-items: center; gap: 16px;
        }
        .mobile-link i { color: #64748b; width: 24px; text-align: center; }
        .mobile-btn {
            background: var(--accent-yellow); color: #000;
            padding: 16px; border-radius: 16px;
            font-weight: 700; text-align: center; text-decoration: none;
            font-size: 1.1rem; box-shadow: 0 10px 25px rgba(255,193,7,0.4);
            margin-top: 10px;
        }

        /* ========= MODERN HERO SECTION ========= */
        .hero-section {
            min-height: 100vh;
            background: linear-gradient(135deg, #052a6b 0%, #0a57cc 100%);
            position: relative;
            display: flex;
            align-items: center;
            padding: 120px 0 80px;
            overflow: hidden;
            color: white;
        }
        .hero-grid-bg {
            position: absolute; inset: 0;
            background-image: linear-gradient(rgba(255,255,255,0.03) 1px, transparent 1px), linear-gradient(90deg, rgba(255,255,255,0.03) 1px, transparent 1px);
            background-size: 50px 50px;
        }
        .hero-badge {
            display: inline-flex; align-items: center; gap: 8px;
            background: rgba(255,193,7,0.15);
            border: 1px solid rgba(255,193,7,0.3);
            color: var(--accent-yellow);
            font-size: 0.85rem; font-weight: 600; text-transform: uppercase;
            padding: 8px 20px; border-radius: 50px; margin-bottom: 25px;
        }
        .hero-section h1 {
            font-weight: 800;
            font-size: clamp(2.5rem, 5vw, 4rem);
            line-height: 1.1;
            margin-bottom: 20px;
            position: relative;
            z-index: 2;
        }
        .hero-section h1 span { color: var(--accent-yellow); }
        .hero-section p { 
            font-size: 1.15rem; opacity: 0.8; max-width: 600px; margin-bottom: 35px;
            position: relative; z-index: 2;
        }

        .btn-accent-yellow {
            background-color: #ffc107; color: #1a1a1a;
            border: none; font-weight: 600; transition: all 0.3s ease;
        }
        .btn-accent-yellow:hover {
            background-color: #e0a800; color: #1a1a1a;
            transform: translateY(-2px); box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }

        .hero-float-cards { 
            display: flex; flex-direction: column; gap: 15px; z-index: 2;
        }
        .h-card {
            background: rgba(255,255,255,0.08);
            backdrop-filter: blur(15px);
            border: 1px solid rgba(255,255,255,0.1);
            border-radius: 15px; padding: 15px 20px;
            display: flex; align-items: center; gap: 15px; 
            animation: float-anim 4s ease-in-out infinite;
            width: 100%; max-width: 350px;
            margin-left: auto;
        }
        @keyframes float-anim { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-8px); } }
        .h-card i { font-size: 1.5rem; color: var(--accent-yellow); }
        .h-card-text div:first-child { font-weight: 700; font-size: 0.95rem; }
        .h-card-text div:last-child { font-size: 0.75rem; opacity: 0.6; }

        @media (max-width: 991.98px) {
            .h-card { max-width: 100%; margin-left: 0; animation: none; }
        }

        /* ========= TICKER ========= */
        .ticker-wrap { background: #041a42; padding: 12px 0; overflow: hidden; }
        .ticker-inner { display: flex; white-space: nowrap; animation: ticker-move 40s linear infinite; }
        .ticker-item { padding: 0 30px; color: rgba(255,255,255,0.7); font-size: 0.85rem; font-weight: 500; }
        @keyframes ticker-move { from { transform: translateX(0); } to { transform: translateX(-50%); } }

        /* ========= SECTION HEADINGS ========= */
        .section-heading { margin-bottom: 50px; text-align: center; }
        .section-heading h2 { font-weight: 700; color: #0a4299; font-size: 2.5rem; position: relative; display: inline-block; padding-bottom: 10px; }
        .section-heading h2::after { content: ''; position: absolute; bottom: 0; left: 50%; transform: translateX(-50%); width: 80px; height: 4px; background-color: #ffc107; border-radius: 2px; }
        .section-heading p { font-size: 1.1rem; color: #555; max-width: 700px; margin: 10px auto 0; }

        /* ========= SERVICE CARDS ========= */
        .service-card { background: #ffffff; border: none; border-radius: 15px; box-shadow: 0 10px 30px rgba(0,0,0,0.07); padding: 30px; text-align: center; height: 100%; transition: all 0.3s ease; }
        .service-card:hover { transform: translateY(-10px); box-shadow: 0 15px 35px rgba(10, 66, 153, 0.15); }
        .service-card .icon { font-size: 3.5rem; line-height: 1; margin-bottom: 20px; color: #0a4299; }
        .service-card h3 { font-weight: 600; color: #111; font-size: 1.4rem; }

        /* ========= BATCH SECTION ========= */
        .batch-section { background: linear-gradient(135deg, #f5f7fa, #eef2f7); padding: 80px 0; }
        .batch-date-card { background: linear-gradient(135deg, #0a4299, #3b82f6); color: white; padding: 40px; border-radius: 15px; text-align: center; box-shadow: 0 10px 30px rgba(10, 66, 153, 0.3); height: 100%; display: flex; flex-direction: column; justify-content: center; }
        .batch-date-card h3 { font-weight: 300; font-size: 1.5rem; text-transform: uppercase; letter-spacing: 1px; }
        .batch-date-card #next-batch-date { font-weight: 700; font-size: 3rem; line-height: 1.2; color: #ffc107; margin-top: 10px; }
        .batch-details-card { background: #ffffff; border-radius: 15px; box-shadow: 0 10px 30px rgba(0,0,0,0.07); padding: 40px; height: 100%; }
        .batch-details-card h3 { font-weight: 600; color: #0a4299; margin-bottom: 25px; }
        .batch-details-list { list-style: none; padding-left: 0; display: flex; flex-wrap: wrap; }
        .batch-details-list li { position: relative; padding-left: 30px; font-size: 1rem; color: #333; margin-bottom: 15px; width: 50%; }
        .batch-details-list li i { position: absolute; left: 0; top: 4px; color: #ffc107; }

        /* ========= AWARD SECTION ========= */
        .award-section { background-color: #ffffff; padding: 80px 0; }
        .award-content h3 { font-weight: 600; color: #0a4299; font-size: 2rem; margin-bottom: 15px; }
        .award-content p { font-size: 1.1rem; color: #555; line-height: 1.7; }
        .video-wrapper { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 15px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); }
        .video-wrapper iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }
        .award-image { border-radius: 15px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); }

        /* ========= TEAM SECTION ========= */
        .team-card { background: #ffffff; border: none; border-radius: 15px; box-shadow: 0 10px 30px rgba(0,0,0,0.07); text-align: center; overflow: hidden; transition: all 0.3s ease; }
        .team-card:hover { transform: translateY(-10px); box-shadow: 0 15px 35px rgba(10, 66, 153, 0.15); }
        .team-card img { width: 100%; height: auto; aspect-ratio: 1 / 1; object-fit: cover; object-position: top; }
        .team-card-body { padding: 25px; }
        .team-card-body h4 { font-weight: 600; color: #0a4299; font-size: 1.3rem; }
        .team-card-body p { font-weight: 500; color: #ffc107; font-size: 1rem; margin-bottom: 0; }

        /* ========= TESTIMONIALS SECTION ========= */
        .testimonials-section { background: linear-gradient(135deg, #f5f7fa, #eef2f7); padding: 80px 0; }

        /* ========= GALLERY SECTION ========= */
        .gallery-item { overflow: hidden; border-radius: 15px; box-shadow: 0 5px 15px rgba(0,0,0,0.05); cursor: pointer; transition: all 0.3s ease; }
        .gallery-item:hover { transform: scale(1.05); box-shadow: 0 10px 25px rgba(0,0,0,0.15); }
        .gallery-item img { width: 100%; aspect-ratio: 1 / 1; object-fit: cover; transition: transform 0.3s ease; }
        
        /* Modal Lightbox */
        .modal-dialog-centered { display: flex; align-items: center; min-height: calc(100% - 1rem); }
        .modal-lg { max-width: 900px; }
        .modal-content { background-color: transparent; border: none; }
        .modal-body { padding: 0; position: relative; }
        #galleryModal img { width: 100%; border-radius: 10px; }
        .modal-close-btn { position: absolute; top: -15px; right: -15px; font-size: 2rem; color: white; background: rgba(0,0,0,0.5); border-radius: 50%; width: 40px; height: 40px; display: flex; align-items: center; justify-content: center; line-height: 1; text-decoration: none; opacity: 0.8; z-index: 1060; }
        .modal-close-btn:hover { opacity: 1; color: white; }
        .modal-nav-btn { position: absolute; top: 50%; transform: translateY(-50%); font-size: 2.5rem; color: white; background: rgba(0,0,0,0.4); border-radius: 50%; width: 50px; height: 50px; display: flex; align-items: center; justify-content: center; text-decoration: none; opacity: 0.7; transition: all 0.3s ease; z-index: 1059; user-select: none; }
        .modal-nav-btn:hover { opacity: 1; color: white; background: rgba(0,0,0,0.6); }
        .modal-nav-btn.prev { left: 15px; }
        .modal-nav-btn.next { right: 15px; }

        /* ========= CONTACT SECTION ========= */
        .contact-card { background: #ffffff; border: none; border-radius: 15px; box-shadow: 0 10px 30px rgba(0,0,0,0.07); padding: 30px; height: 100%; }
        .contact-card h4 { font-weight: 600; color: #0a4299; font-size: 1.5rem; margin-bottom: 20px; }
        .contact-card p { color: #555; margin-bottom: 10px; line-height: 1.7; }
        .contact-card p i { width: 20px; margin-right: 8px; color: #0a4299; }

        /* ========= FOOTER ========= */
        footer { background-color: #052a6b; color: rgba(255,255,255,0.8); padding: 50px 0 20px; }
        footer h5 { color: #ffc107; font-weight: 600; margin-bottom: 20px; }
        footer p, footer a { color: rgba(255,255,255,0.8); text-decoration: none; }
        footer a:hover { color: white; text-decoration: underline; }
        footer .footer-social a { font-size: 1.8rem; color: white; margin-right: 15px; transition: all 0.3s ease; }
        footer .footer-social a:hover { color: #ffc107; transform: translateY(-3px); }
        .footer-bottom { border-top: 1px solid rgba(255,255,255,0.1); padding-top: 20px; margin-top: 30px; text-align: center; font-size: 0.9rem; }

        /* ========= WHATSAPP ========= */
        .whatsapp-float { position: fixed; width: 60px; height: 60px; bottom: 40px; right: 40px; background-color: #25d366; color: #FFF; border-radius: 50px; text-align: center; font-size: 30px; box-shadow: 2px 2px 10px rgba(0,0,0,0.2); z-index: 100; display: flex; align-items: center; justify-content: center; transition: all 0.3s ease; }
        .whatsapp-float:hover { transform: scale(1.1); color: white; }

        /* ========= RESPONSIVE ========= */
        @media (max-width: 991.98px) {
            .batch-details-list li { width: 100%; }
        }
        @media (max-width: 767.98px) {
            .hero-section { padding: 120px 0 60px; text-align: center; }
            .hero-section p { margin-left: auto; margin-right: auto; }
            .batch-date-card { margin-bottom: 30px; }
            .award-content { text-align: center; }
            .award-image { margin-top: 30px; }
            .team-card { max-width: 300px; margin-left: auto; margin-right: auto; }
        }
    </style>
</head>
<body>

    <nav class="navbar navbar-expand-lg sticky-top navbar-dark">
        <div class="container">
            <a class="navbar-brand" href="#">Rank Keywords</a>
            
            <button class="navbar-toggler d-lg-none" type="button" id="openMenuBtn">
                <span class="navbar-toggler-icon"></span>
            </button>
            
            <div class="collapse navbar-collapse d-none d-lg-block">
                <ul class="navbar-nav mx-auto">
                    <li class="nav-item"><a class="nav-link active" href="#">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="#services">Courses</a></li>
                    <li class="nav-item"><a class="nav-link" href="#batch">Batch Details</a></li>
                    <li class="nav-item"><a class="nav-link" href="#team">Our Team</a></li>
                    <li class="nav-item"><a class="nav-link" href="#testimonials">Testimonials</a></li>
                    <li class="nav-item"><a class="nav-link" href="#gallery">Gallery</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
                </ul>
                <a href="https://play.google.com/store/apps/details?id=co.paige.zhsmx" target="_blank" class="btn-download-app mt-3 mt-lg-0">
                    <i class="fa-brands fa-google-play me-2"></i> Download App
                </a>
            </div>
        </div>
    </nav>

    <div id="mobileSlideMenu" class="mobile-slide-menu d-lg-none">
        <div class="mobile-menu-header">
            <span class="mobile-brand">Rank Keywords</span>
            <button id="closeMenuBtn" class="mobile-close-btn"><i class="fa-solid fa-xmark"></i></button>
        </div>
        <div class="mobile-menu-body">
            <a href="#home" class="mobile-link"><i class="fa-solid fa-house"></i> Home</a>
            <a href="#services" class="mobile-link"><i class="fa-solid fa-book-open"></i> Courses</a>
            <a href="#batch" class="mobile-link"><i class="fa-solid fa-calendar-check"></i> Batch Details</a>
            <a href="#team" class="mobile-link"><i class="fa-solid fa-users"></i> Our Team</a>
            <a href="#testimonials" class="mobile-link"><i class="fa-solid fa-star"></i> Testimonials</a>
            <a href="#gallery" class="mobile-link"><i class="fa-solid fa-image"></i> Gallery</a>
            <a href="#contact" class="mobile-link"><i class="fa-solid fa-phone"></i> Contact</a>
            
            <a href="https://play.google.com/store/apps/details?id=co.paige.zhsmx" target="_blank" class="mobile-btn">
                <i class="fa-brands fa-google-play me-2"></i> Download App
            </a>
        </div>
    </div>

    <section class="hero-section" id="home">
        <div class="hero-grid-bg"></div>
        <div class="container position-relative z-2">
            <div class="row align-items-center">
                
                <div class="col-lg-7 text-center text-lg-start">
                    <div class="hero-badge"><i class="fa-solid fa-award"></i> North India's #1 Training Institute</div>
                    <h1>Get High Salary Job <br><span>With AI Skills</span></h1>
                    <p>Join North India's most awarded training institute for Digital Marketing, Coding, Graphics Designing, and Video Editing.</p>
                    
                    <div class="d-flex gap-3 flex-wrap justify-content-center justify-content-lg-start">
                        <a href="#batch" class="btn btn-accent-yellow rounded-pill px-5 py-3 fs-5">View Batch Details</a>
                        <a href="#services" class="btn btn-outline-light rounded-pill px-5 py-3 fs-5">Explore Courses →</a>
                    </div>

                    <div class="row mt-5 pt-3">
                        <div class="col-4">
                            <h3 class="fw-bold mb-0">5000+</h3>
                            <small class="opacity-75">Students Placed</small>
                        </div>
                        <div class="col-4">
                            <h3 class="fw-bold mb-0">3×</h3>
                            <small class="opacity-75">Award Winner</small>
                        </div>
                        <div class="col-4">
                            <h3 class="fw-bold mb-0">100%</h3>
                            <small class="opacity-75">Job Support</small>
                        </div>
                    </div>
                </div>

                <div class="col-lg-5 mt-5 mt-lg-0">
                    <div class="hero-float-cards">
                        <div class="h-card">
                            <i class="fa-solid fa-chart-line"></i>
                            <div class="h-card-text"><div class="text-white">Digital Marketing</div><div class="text-white">50+ AI Modules</div></div>
                        </div>
                        <div class="h-card" style="animation-delay: 1s;">
                            <i class="fa-solid fa-code"></i>
                            <div class="h-card-text"><div class="text-white">Coding & Dev</div><div class="text-white">Live Projects</div></div>
                        </div>
                        <div class="h-card" style="animation-delay: 2s;">
                            <i class="fa-solid fa-palette"></i>
                            <div class="h-card-text"><div class="text-white">Graphics Design</div><div class="text-white">Pro Tools Access</div></div>
                        </div>
                        <div class="h-card" style="animation-delay: 3s;">
                            <i class="fa-solid fa-video"></i>
                            <div class="h-card-text"><div class="text-white">Video Editing</div><div class="text-white">Industry Ready</div></div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <div class="ticker-wrap">
        <div class="ticker-inner">
            <span class="ticker-item"><i class="fa-solid fa-circle-check text-warning"></i> 100% Job Placement Guarantee</span>
            <span class="ticker-item"><i class="fa-solid fa-circle-check text-warning"></i> 50+ AI Integrated Modules</span>
            <span class="ticker-item"><i class="fa-solid fa-circle-check text-warning"></i> Lifetime LMS Access</span>
            <span class="ticker-item"><i class="fa-solid fa-circle-check text-warning"></i> Awarded by WAC & PSIT Kanpur</span>
            <span class="ticker-item"><i class="fa-solid fa-circle-check text-warning"></i> 10+ Professional Certificates</span>
            <span class="ticker-item"><i class="fa-solid fa-circle-check text-warning"></i> 100% Job Placement Guarantee</span>
            <span class="ticker-item"><i class="fa-solid fa-circle-check text-warning"></i> 50+ AI Integrated Modules</span>
            <span class="ticker-item"><i class="fa-solid fa-circle-check text-warning"></i> Lifetime LMS Access</span>
            <span class="ticker-item"><i class="fa-solid fa-circle-check text-warning"></i> Awarded by WAC & PSIT Kanpur</span>
        </div>
    </div>

    <section id="learn-grow" class="py-5" style="padding: 80px 0; background-color: #ffffff;">
        <div class="container">
            <div class="section-heading">
                <h2>Learn & Grow With Experts</h2>
                <p>A glimpse into our learning environment and student success.</p>
            </div>
            <div class="row g-4">
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item"> <img src="uploads/images/batch1.jpg" class="img-fluid" alt="Batch Image 1" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Batch+1';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item">
                        <img src="uploads/images/batch2.jpg" class="img-fluid" alt="Batch Image 2" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Batch+2';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item">
                        <img src="uploads/images/batch51.jpg" class="img-fluid" alt="Batch Image 3" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Batch+3';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item">
                        <img src="uploads/images/batch4.jpg" class="img-fluid" alt="Batch Image 4" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Batch+4';">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- NEW ATTRACTIVE INQUIRY FORM SECTION -->
    <section id="inquiry-form" class="py-5" style="padding: 80px 0; background: linear-gradient(135deg, #f0f4f8, #d9e2ec);">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-8">
                    <div class="card border-0 shadow-lg" style="border-radius: 20px; overflow: hidden;">
                        <div class="card-header text-white text-center py-4" style="background-color: var(--primary-blue);">
                            <h3 class="mb-0 fw-bold">Book FREE DEMO Class </h3>
                        </div>
                        <div class="card-body p-4 p-md-5 bg-white">
                            
                            <!-- Success / Error Messages -->
                                                        
                            
                            <form action="home.php#inquiry-form" method="POST">
                                <div class="mb-4">
                                    <label for="name" class="form-label fw-bold text-secondary">Full Name</label>
                                    <div class="input-group">
                                        <span class="input-group-text bg-light border-end-0"><i class="fa-solid fa-user" style="color: var(--primary-blue);"></i></span>
                                        <input type="text" class="form-control py-3 border-start-0 ps-0" id="name" name="name" placeholder="Name" required style="box-shadow: none;">
                                    </div>
                                </div>
                                
                                <div class="mb-4">
                                    <label for="phone" class="form-label fw-bold text-secondary">Phone Number</label>
                                    <div class="input-group">
                                        <span class="input-group-text bg-light border-end-0"><i class="fa-solid fa-phone" style="color: var(--primary-blue);"></i></span>
                                        <input type="tel" class="form-control py-3 border-start-0 ps-0" id="phone" name="phone" placeholder="Enter your 10-digit phone number" required pattern="[0-9]{10,15}" title="Phone Number" style="box-shadow: none;">
                                    </div>
                                </div>
                                
                                <div class="mb-4">
                                    <label for="course" class="form-label fw-bold text-secondary">Course Interested In</label>
                                    <div class="input-group">
                                        <span class="input-group-text bg-light border-end-0"><i class="fa-solid fa-graduation-cap" style="color: var(--primary-blue);"></i></span>
                                        <select class="form-select py-3 border-start-0 ps-0" id="course" name="course" required style="box-shadow: none;">
                                            <option value="" disabled selected>Select a Course from the list</option>
                                            <option value="Digital Marketing">Advanced Digital Marketing With AI</option>
                                            <option value="Coding Development">Coding & Development With AI</option>
                                            <option value="Graphics Designing">Graphics Designing With AI</option>
                                            <option value="Video Editing">Video Editing With AI</option>
                                        </select>
                                    </div>
                                </div>
                                
                                <button type="submit" name="submit_inquiry" class="btn btn-accent-yellow w-100 py-3 rounded-pill fw-bold text-dark fs-5 mt-3 shadow-sm">
                                    <i class="fa-solid fa-paper-plane me-2"></i> Book Free Demo Class
                                </button>
                            </form>
                            
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="services" class="py-5" style="padding: 80px 0;">
        <div class="container">
            <div class="section-heading">
                <h2>Our Expert Trainings</h2>
                <p>We provide industry-leading training programs designed for 100% job placements.</p>
            </div>
            <div class="row g-4">
                <div class="col-lg-3 col-md-6">
                    <div class="service-card">
                        <div class="icon"><i class="fa-solid fa-chart-line"></i></div>
                        <h3>Digital Marketing</h3>
                        <p>Master SEO, SEM, SMM, and 50+ AI-integrated modules.</p>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6">
                    <div class="service-card">
                        <div class="icon"><i class="fa-solid fa-code"></i></div>
                        <h3>Coding Development</h3>
                        <p>Learn web and app development from scratch with live projects.</p>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6">
                    <div class="service-card">
                        <div class="icon"><i class="fa-solid fa-palette"></i></div>
                        <h3>Graphics Designing</h3>
                        <p>Bring your creative visions to life with professional design tools.</p>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6">
                    <div class="service-card">
                        <div class="icon"><i class="fa-solid fa-video"></i></div>
                        <h3>Video Editing</h3>
                        <p>Produce high-quality, engaging video content for any platform.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <section id="gallery" class="py-5" style="padding: 80px 0; background-color: #ffffff;">
        <div class="container">
            <div class="section-heading">
                <h2>Our Placed Students</h2>
                <p>A glimpse into placements at Rank Keywords.</p>
            </div>
            <div class="row g-4" id="gallery-grid">
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="0">
                        <img src="uploads/images/gallery1.jpg" class="img-fluid" alt="Gallery Image 1" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+1';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="1">
                        <img src="uploads/images/gallery2.jpg" class="img-fluid" alt="Gallery Image 2" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+2';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="2">
                        <img src="uploads/images/gallery3.jpg" class="img-fluid" alt="Gallery Image 3" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+3';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="3">
                        <img src="uploads/images/gallery4.jpg" class="img-fluid" alt="Gallery Image 4" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+4';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="4">
                        <img src="uploads/images/gallery5.jpg" class="img-fluid" alt="Gallery Image 5" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+5';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="5">
                        <img src="uploads/images/gallery6.jpg" class="img-fluid" alt="Gallery Image 6" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+6';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="6">
                        <img src="uploads/images/gallery7.jpg" class="img-fluid" alt="Gallery Image 7" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+7';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="7">
                        <img src="uploads/images/gallery8.jpg" class="img-fluid" alt="Gallery Image 8" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+8';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="8">
                        <img src="uploads/images/gallery9.jpg" class="img-fluid" alt="Gallery Image 9" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+9';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="9">
                        <img src="uploads/images/gallery10.jpg" class="img-fluid" alt="Gallery Image 10" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+10';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="10">
                        <img src="uploads/images/gallery11.jpg" class="img-fluid" alt="Gallery Image 11" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+11';">
                    </div>
                </div>
                <div class="col-lg-3 col-md-4 col-sm-6">
                    <div class="gallery-item" data-bs-toggle="modal" data-bs-target="#galleryModal" data-index="11">
                        <img src="uploads/images/gallery12.jpg" class="img-fluid" alt="Gallery Image 12" onerror="this.onerror=null; this.src='https://placehold.co/400x300/eeeeee/aaaaaa?text=Gallery+12';">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="awards" class="award-section">
        <div class="container">
            <div class="section-heading">
                <h2>Recognized for Excellence</h2>
            </div>
            <div class="row g-5 align-items-center">
                <div class="col-lg-6">
                    <div class="award-content">
                        <span class="text-accent-yellow fw-bold">Awarded by WAC & PSIT, Kanpur</span>
                        <h3 class="mt-2">Best Digital Marketing Course in North India</h3>
                        <p>We are proud to be awarded for three consecutive years (2020, 2021 & 2022). This recognition fuels our commitment to providing the highest quality education and ensuring the success of our students.</p>
                    </div>
                    <img src="uploads/images/80b8ce89-644f-4c75-9bec-bf6e6b23626e.jpg" class="img-fluid award-image mt-4" alt="Award Image" onerror="this.onerror=null; this.src='https://placehold.co/1024x682/eeeeee/aaaaaa?text=Award+Image+(1024x682)';">
                </div>
                <div class="col-lg-6">
                    <div class="video-wrapper">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/T_jJllx9X6c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <section id="batch" class="batch-section">
        <div class="container">
            <div class="section-heading">
                <h2>Join Our Next Batch</h2>
                <p>Start your journey with our comprehensive training program, available online and offline.</p>
            </div>
            <div class="row g-4 align-items-stretch">
                <div class="col-lg-4">
                    <div class="batch-date-card">
                        <h3>New Batch Starts On</h3>
                        <div id="next-batch-date">
                            Loading...
                        </div>
                    </div>
                </div>
                <div class="col-lg-8">
                    <div class="batch-details-card">
                        <h3>With AI Integrated Digital Marketing Training</h3>
                        <ul class="batch-details-list">
                            <li><i class="fa-solid fa-check"></i> Offline/Online Modes</li>
                            <li><i class="fa-solid fa-check"></i> 06 Months / 1 Year</li>
                            <li><i class="fa-solid fa-check"></i> 100% Jobs Placements</li>
                            <li><i class="fa-solid fa-check"></i> 50+ AI Integrated Modules</li>
                            <li><i class="fa-solid fa-check"></i> Work On LIVE Projects</li>
                            <li><i class="fa-solid fa-check"></i> Get Access To Premium Tools</li>
                            <li><i class="fa-solid fa-check"></i> Video Recordings After Class</li>
                            <li><i class="fa-solid fa-check"></i> 20+ Case Studies</li>
                            <li><i class="fa-solid fa-check"></i> Lifetime Access to LMS</li>
                            <li><i class="fa-solid fa-check"></i> 10+ Certificates</li>
                            <li><i class="fa-solid fa-check"></i> Doubt Sessions</li>
                            <li><i class="fa-solid fa-check"></i> High Salary Job Placement</li>
                            <li><i class="fa-solid fa-check"></i> Internships</li>
                            <li><i class="fa-solid fa-check"></i> Free English & Soft-Skills</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="team" class="py-5" style="padding: 80px 0; background-color: #ffffff;">
        <div class="container">
            <div class="section-heading">
                <h2>Meet Our Mentors</h2>
                <p>Learn from founders and industry experts with years of real-world experience.</p>
            </div>
            <div class="row g-4">
                <div class="col-lg-3 col-md-6 col-sm-6">
                    <div class="team-card">
                        <img src="uploads/images/New-Project-2022-10-02T144217.309.png" alt="Abhishek Singh" onerror="this.onerror=null; this.src='https://placehold.co/300x300/0a4299/FFFFFF?text=A.S.';">
                        <div class="team-card-body">
                            <h4>Abhishek Singh</h4>
                            <p>Founder</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 col-sm-6">
                    <div class="team-card">
                        <img src="uploads/images/New-Project-2022-10-02T144311.336.png" alt="ANAND SINGH" onerror="this.onerror=null; this.src='https://placehold.co/300x300/0a4299/FFFFFF?text=A.S.';">
                        <div class="team-card-body">
                            <h4>ANAND SINGH</h4>
                            <p>Director</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 col-sm-6">
                    <div class="team-card">
                        <img src="uploads/images/New-Project-2022-10-02T144647.963-pvm58prtrnoi5ew741xplia2gx3znpmf102o6unzkg.png" alt="DEEPTI AVASTHI" onerror="this.onerror=null; this.src='https://placehold.co/300x300/0a4299/FFFFFF?text=D.A.';">
                        <div class="team-card-body">
                            <h4>DEEPTI AVASTHI</h4>
                            <p>Trainer</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 col-sm-6">
                    <div class="team-card">
                        <img src="uploads/images/New-Project-2022-10-02T144741.186-pvm58nw5dzlxi6yxf14ggir5a5d98beycqrp8aqrww.png" alt="GOPAL TRIVEDI" onerror="this.onerror=null; this.src='https://placehold.co/300x300/0a4299/FFFFFF?text=G.T.';">
                        <div class="team-card-body">
                            <h4>GOPAL TRIVEDI</h4>
                            <p>Mentor</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="testimonials" class="testimonials-section">
        <div class="container">
            <div class="section-heading">
                <h2>Hear From Our Students</h2>
                <p>See what our successful alumni have to say about their experience.</p>
            </div>
            <div class="row g-4">
                <div class="col-lg-6">
                    <div class="video-wrapper">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/JBt3HjsZwmY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="video-wrapper">
<iframe width="560" height="315" src="https://www.youtube.com/embed/_qtPvlEQEJA?si=5qXPuasc56iwMK5A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>                    </div>
                </div>
            </div>
        </div>
    </section>

    <div class="modal fade" id="galleryModal" tabindex="-1" aria-labelledby="galleryModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-lg modal-dialog-centered">
            <div class="modal-content">
                <a href="javascript:void(0);" class="modal-close-btn" data-bs-dismiss="modal" aria-label="Close">&times;</a>
                <a href="javascript:void(0);" class="modal-nav-btn prev" id="galleryPrevBtn"><i class="fa-solid fa-chevron-left"></i></a>
                <a href="javascript:void(0);" class="modal-nav-btn next" id="galleryNextBtn"><i class="fa-solid fa-chevron-right"></i></a>
                <div class="modal-body">
                    <img src="" class="img-fluid" id="modalImage" alt="Gallery Popup Image">
                </div>
            </div>
        </div>
    </div>

    <section id="contact" class="py-5" style="padding: 80px 0; background-color: #f8f9fa;">
        <div class="container">
            <div class="section-heading">
                <h2>Contact Us</h2>
                <p>Visit us at one of our three locations or get in touch online. We're here to help!</p>
            </div>
            <div class="row g-4">
                <div class="col-lg-4 col-md-6">
                    <div class="contact-card">
                        <h4>Kanpur Office</h4>
                        <p><i class="fa-solid fa-location-dot"></i> 5th Floor, Surya Tower, Just Opposite Kulwanti Hospital Kakadeo Kanpur</p>
                        <p><i class="fa-solid fa-phone"></i> +91-8887599932</p>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6">
                    <div class="contact-card">
                        <h4>Chandigarh Office</h4>
                        <p><i class="fa-solid fa-location-dot"></i> Sector 34-A, Chandigarh – 160022</p>
                        <p><i class="fa-solid fa-phone"></i> +91-6387902411</p>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6">
                    <div class="contact-card">
                        <h4>Lucknow Office</h4>
                        <p><i class="fa-solid fa-location-dot"></i> 9/81, Indira Nagar, Near Central Academy School, Lucknow, U.P.</p>
                        <p><i class="fa-solid fa-phone"></i> +91-8299115093</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <div class="row g-4">
                <div class="col-lg-4">
                    <p>Rank Keywords is the leading institute for practical, job-oriented training in digital marketing, coding, and creative design.</p>
                    <a href="https://play.google.com/store/apps/details?id=co.paige.zhsmx" target="_blank" class="btn btn-accent-yellow btn-sm mt-2">
                        <i class="fa-brands fa-google-play me-2"></i> Download Our App
                    </a>
                </div>
                <div class="col-lg-2 col-md-6">
                    <h5>Quick Links</h5>
                    <ul class="list-unstyled">
                        <li><a href="#services">Courses</a></li> 
                        <li><a href="#batch">Batch Details</a></li>
                        <li><a href="#team">Team</a></li>
                        <li><a href="#gallery">Gallery</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <div class="col-lg-3 col-md-6">
                    <h5>Trainings</h5>
                    <ul class="list-unstyled">
                        <li><a href="#services">Digital Marketing</a></li>
                        <li><a href="#services">Coding Development</a></li>
                        <li><a href="#services">Graphics Designing</a></li>
                        <li><a href="#services">Video Editing</a></li>
                    </ul>
                </div>
                <div class="col-lg-3">
                    <h5>Follow Us</h5>
                    <p>Stay connected with us on social media for the latest updates and news.</p>
                    <div class="footer-social">
                        <a href="https://www.facebook.com/rankkeywords" target="_blank"><i class="fa-brands fa-facebook"></i></a>
                        <a href="https://www.instagram.com/rankkeywords/#" target="_blank"><i class="fa-brands fa-instagram"></i></a>
                        <a href="https://x.com/rank_group96838" target="_blank"><i class="fa-brands fa-twitter"></i></a>
                        <a href="https://www.linkedin.com/company/rankkeywords" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
                        <a href="https://www.youtube.com/@rankkeywords" target="_blank"><i class="fa-brands fa-youtube"></i></a>
                    </div>
                </div>
            </div>
            <div class="footer-bottom">
                &copy; <script>document.write(new Date().getFullYear())</script> Rank Keywords. All Rights Reserved.
            </div>
        </div>
    </footer>

    <a href="https://wa.me/918887599932" class="whatsapp-float" target="_blank">
        <i class="fa-brands fa-whatsapp"></i>
    </a>
    
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            
            // --- Mobile Menu Toggle Logic ---
            const openBtn = document.getElementById('openMenuBtn');
            const closeBtn = document.getElementById('closeMenuBtn');
            const mobileMenu = document.getElementById('mobileSlideMenu');
            const mobileLinks = document.querySelectorAll('.mobile-link');

            const openMenu = () => {
                mobileMenu.classList.add('open');
                document.body.style.overflow = 'hidden'; // Stop background scrolling
            };

            const closeMenu = () => {
                mobileMenu.classList.remove('open');
                document.body.style.overflow = '';
            };

            if(openBtn) openBtn.addEventListener('click', openMenu);
            if(closeBtn) closeBtn.addEventListener('click', closeMenu);
            mobileLinks.forEach(link => link.addEventListener('click', closeMenu));


            // --- Navbar Scroll Effect ---
            window.addEventListener('scroll', function() {
                if (window.scrollY > 50) {
                    document.querySelector('.navbar').classList.add('scrolled');
                } else {
                    document.querySelector('.navbar').classList.remove('scrolled');
                }
            });

            // --- Next Batch Date Logic ---
            try {
                const batchDateEl = document.getElementById('next-batch-date');
                if (batchDateEl) {
                    const today = new Date();
                    const dayOfWeek = today.getDay(); // 0=Sun, 1=Mon, ..., 6=Sat
                    
                    let daysUntilMonday;
                    if (dayOfWeek === 1) {
                        daysUntilMonday = 7; // If it's Monday, get next Monday
                    } else {
                        daysUntilMonday = (1 - dayOfWeek + 7) % 7;
                    }
                    if (daysUntilMonday === 0) { // Handle Sunday case
                        daysUntilMonday = 1;
                    }

                    const nextMonday = new Date(today.getTime());
                    nextMonday.setDate(today.getDate() + daysUntilMonday);
                    
                    const options = { year: 'numeric', month: 'long', day: 'numeric' };
                    batchDateEl.innerText = nextMonday.toLocaleDateString('en-US', options);
                }
            } catch (e) {
                console.error("Error calculating next batch date:", e);
                const batchDateEl = document.getElementById('next-batch-date');
                if(batchDateEl) batchDateEl.innerText = "Check Back Soon!";
            }

            // --- Gallery Lightbox Logic ---
            try {
                const galleryItems = document.querySelectorAll('#gallery .gallery-item'); 
                const modalImage = document.getElementById('modalImage');
                const prevBtn = document.getElementById('galleryPrevBtn');
                const nextBtn = document.getElementById('galleryNextBtn');
                
                const gallerySources = Array.from(galleryItems).map(item => item.querySelector('img').src);
                let currentIndex = 0;

                galleryItems.forEach(item => {
                    item.addEventListener('click', function() {
                        currentIndex = parseInt(this.dataset.index, 10);
                        updateModalImage();
                    });
                });

                function updateModalImage() {
                    if (modalImage) {
                        modalImage.src = gallerySources[currentIndex];
                        modalImage.onerror = function() {
                            this.onerror = null;
                            this.src = `https://placehold.co/800x600/eeeeee/aaaaaa?text=Image+${currentIndex + 1}+Not+Found`;
                        };
                    }
                }

                if (prevBtn) {
                    prevBtn.addEventListener('click', function(e) {
                        e.stopPropagation();
                        currentIndex = (currentIndex - 1 + gallerySources.length) % gallerySources.length;
                        updateModalImage();
                    });
                }
                
                if (nextBtn) {
                    nextBtn.addEventListener('click', function(e) {
                        e.stopPropagation();
                        currentIndex = (currentIndex + 1) % gallerySources.length;
                        updateModalImage();
                    });
                }

            } catch (e) {
                console.error("Error initializing gallery:", e);
            }

            // --- Navbar Active Link Scrolling (Desktop) ---
            const navLinks = document.querySelectorAll('.navbar-nav .nav-link');
            const sections = document.querySelectorAll('section[id]');

            function changeNav() {
                let index = sections.length;
                while(--index && window.scrollY + 100 < sections[index].offsetTop) {}
                
                navLinks.forEach((link) => link.classList.remove('active'));
                
                const sectionId = sections[index] ? sections[index].id : null;
                if (sectionId) {
                    const activeLink = document.querySelector(`.navbar-nav .nav-link[href="#${sectionId}"]`);
                    if(activeLink) {
                        activeLink.classList.add('active');
                    }
                } else {
                    const homeLink = document.querySelector('.navbar-nav .nav-link[href="#"]');
                    if (homeLink) homeLink.classList.add('active');
                }
            }

            changeNav(); 
            window.addEventListener('scroll', changeNav); 

        });
    </script>
</body>
</html>
