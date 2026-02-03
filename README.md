<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="الرحّال للخدمات السياحية - حجز تذاكر طيران، تأشيرات، فنادق، برامج سياحية، رحلات شهر عسل، وخدمات سفر متكاملة">
    <meta name="keywords" content="حجز طيران, برامج سياحية, استخراج تأشيرة, رحلات سفر, شهر عسل, فنادق, سياحة, سفر, عروض سياحية, تأشيرات شنغن">
    <meta name="author" content="الرحّال للخدمات السياحية">
    <meta name="robots" content="index, follow">
    <title>الرحّال للخدمات السياحية | كل خدمات سفرك في مكان واحد</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;500;600;700;800&family=Amiri:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --dark-blue: #0a2540;
            --gold: #d4af37;
            --gold-light: #e6c07b;
            --gold-dark: #b89e2b;
            --orange: #e67e22;
            --white: #ffffff;
            --light-gray: #f8f9fa;
            --gray: #6c757d;
            --dark-gray: #343a40;
            --shadow: 0 4px 20px rgba(0, 0, 0, 0.15);
            --shadow-hover: 0 6px 25px rgba(0, 0, 0, 0.2);
            --transition: all 0.3s ease;
            --border-radius: 12px;
            --border-radius-lg: 20px;
            --section-padding: 80px 0;
        }
        
        /* Dark Mode Variables */
        .dark-mode {
            --dark-blue: #081a2d;
            --gold: #c19a2e;
            --gold-light: #d4b06d;
            --white: #121212;
            --light-gray: #0f0f0f;
            --gray: #a0a0a0;
            --dark-gray: #e0e0e0;
            --shadow: 0 4px 20px rgba(0, 0, 0, 0.4);
            --shadow-hover: 0 6px 25px rgba(0, 0, 0, 0.5);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Cairo', sans-serif;
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
            background-color: var(--light-gray);
            transition: background-color 0.3s ease, color 0.3s ease;
        }
        
        body.dark-mode {
            background-color: var(--light-gray);
            color: var(--dark-gray);
        }
        
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Cairo', sans-serif;
            font-weight: 700;
            line-height: 1.3;
            margin-bottom: 20px;
            color: var(--dark-blue);
        }
        
        body.dark-mode h1, 
        body.dark-mode h2, 
        body.dark-mode h3, 
        body.dark-mode h4, 
        body.dark-mode h5, 
        body.dark-mode h6 {
            color: var(--white);
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        .btn {
            display: inline-block;
            background: var(--gold);
            color: var(--white);
            padding: 14px 32px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 18px;
            transition: var(--transition);
            border: 2px solid var(--gold);
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(212, 175, 55, 0.3);
        }
        
        .btn:hover {
            background: var(--gold-dark);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(212, 175, 55, 0.4);
        }
        
        .btn-outline {
            background: transparent;
            border: 2px solid var(--gold);
            color: var(--gold);
        }
        
        .btn-outline:hover {
            background: var(--gold);
            color: var(--white);
        }
        
        .btn-whatsapp {
            background: #25D366;
            border-color: #25D366;
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }
        
        .btn-whatsapp:hover {
            background: #128C7E;
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(37, 211, 102, 0.4);
        }
        
        .btn-primary {
            background: var(--dark-blue);
            border-color: var(--dark-blue);
            color: white;
        }
        
        .btn-primary:hover {
            background: #081a2d;
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(10, 37, 64, 0.4);
        }
        
        .btn-secondary {
            background: var(--gray);
            border-color: var(--gray);
            color: white;
        }
        
        .btn-secondary:hover {
            background: #5a6268;
            transform: translateY(-3px);
        }
        
        .btn-sm {
            padding: 8px 18px !important;
            font-size: 14px !important;
        }
        
        section {
            padding: var(--section-padding);
            background-color: var(--white);
            transition: background-color 0.3s ease;
        }
        
        body.dark-mode section {
            background-color: var(--white);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
            position: relative;
        }
        
        .section-title h2 {
            font-size: 36px;
            display: inline-block;
            padding-bottom: 15px;
            position: relative;
            z-index: 2;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 70px;
            height: 4px;
            background: var(--gold);
            border-radius: 2px;
            z-index: -1;
        }
        
        .section-title p {
            color: var(--gray);
            font-size: 18px;
            margin-top: 15px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        
        body.dark-mode .section-title p {
            color: #b0b0b0;
        }
        
        /* Header Styles */
        header {
            background-color: var(--white);
            box-shadow: var(--shadow);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            padding: 15px 0;
            transition: background-color 0.3s ease, box-shadow 0.3s ease;
        }
        
        body.dark-mode header {
            background-color: var(--dark-blue);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: relative;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            z-index: 10;
        }
        
        .logo-icon {
            font-size: 32px;
            color: var(--gold);
        }
        
        .logo-text {
            font-family: 'Cairo', sans-serif;
            font-size: 28px;
            font-weight: 800;
            color: var(--dark-blue);
        }
        
        body.dark-mode .logo-text {
            color: var(--white);
        }
        
        .logo-text span {
            color: var(--gold);
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
            z-index: 10;
        }
        
        nav a {
            text-decoration: none;
            color: var(--dark-blue);
            font-weight: 600;
            font-size: 17px;
            transition: var(--transition);
            position: relative;
            padding: 5px 0;
        }
        
        body.dark-mode nav a {
            color: var(--white);
        }
        
        nav a:hover, nav a.active {
            color: var(--gold);
        }
        
        nav a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--gold);
            transition: var(--transition);
        }
        
        nav a:hover::after, nav a.active::after {
            width: 100%;
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 28px;
            color: var(--dark-blue);
            cursor: pointer;
            z-index: 100;
        }
        
        body.dark-mode .mobile-menu-btn {
            color: var(--white);
        }
        
        .header-actions {
            display: flex;
            align-items: center;
            gap: 15px;
            z-index: 10;
        }
        
        .search-bar {
            max-width: 400px;
            position: relative;
            display: none;
        }
        
        .search-bar.active {
            display: block;
        }
        
        .search-bar input {
            width: 100%;
            padding: 12px 20px 12px 45px;
            border: 2px solid var(--gold);
            border-radius: 50px;
            font-size: 16px;
            font-family: 'Cairo', sans-serif;
            transition: var(--transition);
            background-color: var(--white);
            color: var(--dark-blue);
        }
        
        body.dark-mode .search-bar input {
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--white);
            border-color: var(--gold);
        }
        
        .search-bar input:focus {
            outline: none;
            box-shadow: 0 0 0 3px rgba(212, 175, 55, 0.3);
        }
        
        .search-bar button {
            position: absolute;
            left: 18px;
            top: 50%;
            transform: translateY(-50%);
            background: none;
            border: none;
            font-size: 18px;
            color: var(--gold);
            cursor: pointer;
        }
        
        .theme-toggle {
            width: 48px;
            height: 48px;
            border-radius: 50%;
            background: var(--gold);
            color: var(--dark-blue);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 20px;
            cursor: pointer;
            transition: var(--transition);
            border: none;
            box-shadow: 0 4px 10px rgba(212, 175, 55, 0.3);
        }
        
        .theme-toggle:hover {
            transform: rotate(20deg) scale(1.1);
            box-shadow: 0 6px 15px rgba(212, 175, 55, 0.5);
        }
        
        body.dark-mode .theme-toggle {
            background: var(--gold);
            color: var(--dark-blue);
        }
        
        .user-menu {
            position: relative;
            z-index: 10;
        }
        
        .user-btn {
            width: 48px;
            height: 48px;
            border-radius: 50%;
            background: var(--gold);
            color: var(--dark-blue);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 20px;
            cursor: pointer;
            transition: var(--transition);
            border: none;
            box-shadow: 0 4px 10px rgba(212, 175, 55, 0.3);
        }
        
        .user-btn:hover {
            transform: scale(1.1);
            box-shadow: 0 6px 15px rgba(212, 175, 55, 0.5);
        }
        
        body.dark-mode .user-btn {
            background: var(--gold);
            color: var(--dark-blue);
        }
        
        .user-dropdown {
            position: absolute;
            top: 60px;
            left: 0;
            background: var(--white);
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            min-width: 220px;
            padding: 15px 0;
            display: none;
            z-index: 999;
        }
        
        body.dark-mode .user-dropdown {
            background: var(--dark-blue);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.6);
        }
        
        .user-dropdown.show {
            display: block;
            animation: fadeInDown 0.3s ease;
        }
        
        .dropdown-item {
            padding: 12px 20px;
            display: flex;
            align-items: center;
            gap: 12px;
            color: var(--dark-blue);
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            font-size: 16px;
        }
        
        body.dark-mode .dropdown-item {
            color: var(--white);
        }
        
        .dropdown-item:hover {
            background: rgba(212, 175, 55, 0.15);
            padding-left: 28px;
        }
        
        body.dark-mode .dropdown-item:hover {
            background: rgba(212, 175, 55, 0.25);
        }
        
        .dropdown-item i {
            width: 20px;
            text-align: center;
            color: var(--gold);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(10, 37, 64, 0.85), rgba(10, 37, 64, 0.9)), url('https://images.unsplash.com/photo-1476514525535-07fb3b4ae5f1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: var(--white);
            padding-top: 80px;
        }
        
        body.dark-mode .hero {
            background: linear-gradient(rgba(8, 26, 45, 0.9), rgba(8, 26, 45, 0.95)), url('https://images.unsplash.com/photo-1476514525535-07fb3b4ae5f1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80');
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            padding-top: 60px;
        }
        
        .hero h1 {
            font-size: 52px;
            margin-bottom: 25px;
            color: var(--white);
            animation: fadeInDown 1s ease;
        }
        
        .hero p {
            font-size: 24px;
            margin-bottom: 40px;
            color: rgba(255, 255, 255, 0.9);
            animation: fadeInUp 1s ease 0.2s both;
        }
        
        .hero-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            animation: fadeIn 1.5s ease 0.4s both;
        }
        
        .hero-buttons .btn {
            padding: 16px 40px;
            font-size: 20px;
        }
        
        /* Services Section */
        .services {
            background-color: var(--white);
        }
        
        body.dark-mode .services {
            background-color: var(--white);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .service-card {
            background: var(--white);
            border-radius: var(--border-radius-lg);
            padding: 35px 25px;
            text-align: center;
            box-shadow: var(--shadow);
            transition: var(--transition);
            cursor: pointer;
            border: 2px solid transparent;
        }
        
        body.dark-mode .service-card {
            background: rgba(255, 255, 255, 0.08);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-hover);
            border-color: var(--gold);
        }
        
        .service-icon {
            font-size: 48px;
            color: var(--gold);
            margin-bottom: 20px;
            display: inline-block;
            width: 80px;
            height: 80px;
            background: rgba(212, 175, 55, 0.1);
            border-radius: 50%;
            line-height: 80px;
        }
        
        body.dark-mode .service-icon {
            background: rgba(212, 175, 55, 0.2);
        }
        
        .service-card h3 {
            font-size: 22px;
            margin-bottom: 15px;
        }
        
        .service-card p {
            color: var(--gray);
            font-size: 16px;
        }
        
        body.dark-mode .service-card p {
            color: #b0b0b0;
        }
        
        /* Trust Line */
        .trust-line {
            background: var(--dark-blue);
            color: var(--white);
            text-align: center;
            padding: 15px 0;
            font-size: 18px;
            font-weight: 500;
            transition: background-color 0.3s ease;
        }
        
        body.dark-mode .trust-line {
            background: #081a2d;
        }
        
        .trust-line i {
            margin-left: 8px;
            color: var(--gold);
        }
        
        /* Features Section */
        .features {
            background-color: var(--light-gray);
        }
        
        body.dark-mode .features {
            background-color: rgba(0, 0, 0, 0.2);
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .feature-card {
            background: var(--white);
            border-radius: var(--border-radius);
            padding: 30px;
            text-align: center;
            box-shadow: var(--shadow);
        }
        
        body.dark-mode .feature-card {
            background: rgba(255, 255, 255, 0.08);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }
        
        .feature-icon {
            font-size: 42px;
            color: var(--gold);
            margin-bottom: 20px;
        }
        
        .feature-card h3 {
            font-size: 24px;
            margin-bottom: 15px;
        }
        
        /* Tours Section */
        .tours-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .tour-card {
            background: var(--white);
            border-radius: var(--border-radius-lg);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }
        
        body.dark-mode .tour-card {
            background: rgba(255, 255, 255, 0.08);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }
        
        .tour-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-hover);
        }
        
        .tour-img {
            height: 220px;
            overflow: hidden;
        }
        
        .tour-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }
        
        .tour-card:hover .tour-img img {
            transform: scale(1.1);
        }
        
        .tour-content {
            padding: 25px;
        }
        
        .tour-title {
            font-size: 24px;
            margin-bottom: 10px;
        }
        
        .tour-duration {
            display: inline-block;
            background: var(--gold);
            color: var(--white);
            padding: 5px 15px;
            border-radius: 20px;
            font-weight: 600;
            margin: 10px 0;
        }
        
        .tour-price {
            font-size: 28px;
            font-weight: 700;
            color: var(--dark-blue);
            margin: 15px 0;
        }
        
        body.dark-mode .tour-price {
            color: var(--white);
        }
        
        .tour-price span {
            font-size: 16px;
            color: var(--gray);
            font-weight: 400;
            margin-left: 5px;
        }
        
        body.dark-mode .tour-price span {
            color: #b0b0b0;
        }
        
        /* About Section */
        .about {
            background-color: var(--white);
        }
        
        body.dark-mode .about {
            background-color: var(--white);
        }
        
        .about-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 50px;
            align-items: center;
            margin-top: 40px;
        }
        
        .about-text h2 {
            font-size: 36px;
            margin-bottom: 25px;
            color: var(--dark-blue);
        }
        
        body.dark-mode .about-text h2 {
            color: var(--white);
        }
        
        .about-text p {
            margin-bottom: 20px;
            font-size: 17px;
            color: var(--dark-gray);
        }
        
        body.dark-mode .about-text p {
            color: #d0d0d0;
        }
        
        .about-stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
            margin-top: 30px;
        }
        
        .stat-item {
            text-align: center;
        }
        
        .stat-number {
            font-size: 42px;
            font-weight: 800;
            color: var(--gold);
            margin-bottom: 5px;
        }
        
        .stat-label {
            font-size: 16px;
            color: var(--gray);
        }
        
        body.dark-mode .stat-label {
            color: #b0b0b0;
        }
        
        .about-img {
            border-radius: var(--border-radius-lg);
            overflow: hidden;
            box-shadow: var(--shadow-hover);
            position: relative;
        }
        
        .about-img img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        /* Testimonials Section */
        .testimonials {
            background: linear-gradient(rgba(10, 37, 64, 0.9), rgba(10, 37, 64, 0.95)), url('https://images.unsplash.com/photo-1503220317375-aaad61436b1b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80');
            background-size: cover;
            background-position: center;
            color: var(--white);
            text-align: center;
        }
        
        body.dark-mode .testimonials {
            background: linear-gradient(rgba(8, 26, 45, 0.95), rgba(8, 26, 45, 0.98)), url('https://images.unsplash.com/photo-1503220317375-aaad61436b1b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80');
        }
        
        .testimonials .section-title h2 {
            color: var(--white);
        }
        
        .testimonials .section-title h2::after {
            background: var(--gold);
        }
        
        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .testimonial-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: var(--border-radius-lg);
            padding: 35px;
            margin: 15px;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .stars {
            color: var(--gold);
            font-size: 24px;
            margin-bottom: 20px;
        }
        
        .testimonial-text {
            font-size: 18px;
            margin-bottom: 25px;
            font-style: italic;
            line-height: 1.7;
        }
        
        .testimonial-author {
            font-weight: 700;
            font-size: 20px;
        }
        
        .author-title {
            color: var(--gold-light);
            font-size: 16px;
            margin-top: 5px;
        }
        
        /* Offers Section */
        .offers {
            background-color: var(--white);
        }
        
        body.dark-mode .offers {
            background-color: var(--white);
        }
        
        .offers-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .offer-card {
            background: var(--white);
            border-radius: var(--border-radius-lg);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            position: relative;
            border: 2px solid transparent;
        }
        
        body.dark-mode .offer-card {
            background: rgba(255, 255, 255, 0.08);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }
        
        .offer-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-hover);
            border-color: var(--gold);
        }
        
        .offer-badge {
            position: absolute;
            top: 15px;
            left: 15px;
            background: var(--orange);
            color: var(--white);
            padding: 5px 15px;
            border-radius: 20px;
            font-weight: 700;
            font-size: 14px;
            z-index: 10;
        }
        
        .offer-img {
            height: 200px;
            overflow: hidden;
        }
        
        .offer-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }
        
        .offer-card:hover .offer-img img {
            transform: scale(1.1);
        }
        
        .offer-content {
            padding: 25px;
        }
        
        .offer-title {
            font-size: 24px;
            margin-bottom: 10px;
        }
        
        .offer-old-price {
            text-decoration: line-through;
            color: var(--gray);
            font-size: 20px;
            margin-right: 10px;
        }
        
        body.dark-mode .offer-old-price {
            color: #909090;
        }
        
        .offer-new-price {
            font-size: 32px;
            font-weight: 800;
            color: var(--orange);
        }
        
        .offer-savings {
            background: rgba(230, 126, 34, 0.1);
            color: var(--orange);
            padding: 5px 15px;
            border-radius: 20px;
            font-weight: 600;
            display: inline-block;
            margin: 10px 0;
        }
        
        body.dark-mode .offer-savings {
            background: rgba(230, 126, 34, 0.2);
        }
        
        .countdown {
            display: flex;
            gap: 10px;
            margin: 15px 0;
        }
        
        .countdown-item {
            background: var(--dark-blue);
            color: var(--white);
            padding: 8px 12px;
            border-radius: 8px;
            text-align: center;
            min-width: 60px;
        }
        
        body.dark-mode .countdown-item {
            background: rgba(255, 255, 255, 0.15);
        }
        
        .countdown-number {
            font-size: 24px;
            font-weight: 700;
            display: block;
        }
        
        .countdown-label {
            font-size: 12px;
            text-transform: uppercase;
        }
        
        /* FAQ Section */
        .faq {
            background-color: var(--light-gray);
        }
        
        body.dark-mode .faq {
            background-color: rgba(0, 0, 0, 0.2);
        }
        
        .faq-container {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .faq-item {
            background: var(--white);
            border-radius: var(--border-radius);
            margin-bottom: 15px;
            box-shadow: var(--shadow);
            overflow: hidden;
        }
        
        body.dark-mode .faq-item {
            background: rgba(255, 255, 255, 0.08);
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }
        
        .faq-question {
            padding: 20px 25px;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: var(--transition);
            color: var(--dark-blue);
        }
        
        body.dark-mode .faq-question {
            color: var(--white);
        }
        
        .faq-question:hover {
            background: rgba(212, 175, 55, 0.05);
        }
        
        body.dark-mode .faq-question:hover {
            background: rgba(212, 175, 55, 0.15);
        }
        
        .faq-question.active {
            background: rgba(212, 175, 55, 0.1);
            color: var(--gold);
        }
        
        body.dark-mode .faq-question.active {
            background: rgba(212, 175, 55, 0.25);
        }
        
        .faq-answer {
            padding: 0 25px;
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease, padding 0.3s ease;
            color: var(--dark-gray);
        }
        
        body.dark-mode .faq-answer {
            color: #d0d0d0;
        }
        
        .faq-answer.show {
            padding: 0 25px 20px;
            max-height: 500px;
        }
        
        .faq-toggle {
            font-size: 20px;
            transition: transform 0.3s ease;
            color: var(--gold);
        }
        
        .faq-toggle.active {
            transform: rotate(180deg);
        }
        
        /* Appointment Section */
        .appointment {
            background: linear-gradient(135deg, var(--dark-blue) 0%, #1a3a5f 100%);
            color: var(--white);
            text-align: center;
        }
        
        body.dark-mode .appointment {
            background: linear-gradient(135deg, #081a2d 0%, #0d2845 100%);
        }
        
        .appointment .section-title h2 {
            color: var(--white);
        }
        
        .appointment .section-title h2::after {
            background: var(--gold);
        }
        
        .appointment-form {
            max-width: 600px;
            margin: 40px auto 0;
            background: rgba(255, 255, 255, 0.1);
            padding: 40px;
            border-radius: var(--border-radius-lg);
            backdrop-filter: blur(10px);
        }
        
        .appointment-form .form-group {
            margin-bottom: 20px;
            text-align: right;
        }
        
        .appointment-form input,
        .appointment-form select {
            width: 100%;
            padding: 15px;
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 10px;
            background: rgba(255, 255, 255, 0.15);
            color: var(--white);
            font-family: 'Cairo', sans-serif;
            font-size: 16px;
        }
        
        .appointment-form input::placeholder,
        .appointment-form select {
            color: rgba(255, 255, 255, 0.7);
        }
        
        .appointment-form .btn {
            background: var(--gold);
            color: var(--dark-blue);
            width: 100%;
            padding: 16px;
            font-size: 18px;
            margin-top: 10px;
        }
        
        /* Contact Section */
        .contact {
            background-color: var(--white);
        }
        
        body.dark-mode .contact {
            background-color: var(--white);
        }
        
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 50px;
            margin-top: 40px;
        }
        
        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 30px;
        }
        
        .contact-item {
            display: flex;
            align-items: flex-start;
            gap: 20px;
        }
        
        .contact-icon {
            font-size: 28px;
            color: var(--gold);
            min-width: 40px;
        }
        
        .contact-form .form-group {
            margin-bottom: 20px;
        }
        
        .contact-form input,
        .contact-form textarea,
        .contact-form select {
            width: 100%;
            padding: 15px;
            border: 1px solid #ddd;
            border-radius: 10px;
            font-family: 'Cairo', sans-serif;
            font-size: 16px;
            transition: var(--transition);
            background-color: var(--white);
            color: var(--dark-blue);
        }
        
        body.dark-mode .contact-form input,
        body.dark-mode .contact-form textarea,
        body.dark-mode .contact-form select {
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--white);
            border-color: rgba(255, 255, 255, 0.2);
        }
        
        .contact-form input:focus,
        .contact-form textarea:focus,
        .contact-form select:focus {
            border-color: var(--gold);
            outline: none;
            box-shadow: 0 0 0 3px rgba(212, 175, 55, 0.2);
        }
        
        .contact-form textarea {
            min-height: 150px;
            resize: vertical;
        }
        
        .map-container {
            height: 350px;
            background: #e9ecef;
            border-radius: var(--border-radius-lg);
            overflow: hidden;
            box-shadow: var(--shadow);
            margin-top: 30px;
            position: relative;
        }
        
        .map-link {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(10, 37, 64, 0.85);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
            z-index: 10;
            transition: background 0.3s ease;
        }
        
        .map-link:hover {
            background: rgba(10, 37, 64, 0.95);
        }
        
        .map-link i {
            font-size: 48px;
            margin-bottom: 20px;
            color: var(--gold);
        }
        
        .map-link h3 {
            font-size: 24px;
            margin-bottom: 10px;
            color: white;
        }
        
        .map-link p {
            font-size: 18px;
            max-width: 80%;
            text-align: center;
            color: rgba(255, 255, 255, 0.9);
        }
        
        body.dark-mode .map-container {
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        /* Payment Section */
        .payment-methods {
            background-color: var(--white);
        }
        
        body.dark-mode .payment-methods {
            background-color: var(--white);
        }
        
        .payment-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-top: 40px;
            text-align: center;
        }
        
        .payment-card {
            padding: 25px 15px;
            border-radius: var(--border-radius);
            background: var(--light-gray);
            transition: var(--transition);
            border: 1px solid #eee;
        }
        
        body.dark-mode .payment-card {
            background: rgba(255, 255, 255, 0.08);
            border-color: rgba(255, 255, 255, 0.1);
        }
        
        .payment-card:hover {
            background: var(--dark-blue);
            color: var(--white);
            transform: translateY(-5px);
            border-color: var(--gold);
        }
        
        body.dark-mode .payment-card:hover {
            background: rgba(212, 175, 55, 0.2);
        }
        
        .payment-card:hover i {
            color: var(--gold);
        }
        
        .payment-icon {
            font-size: 42px;
            color: var(--dark-blue);
            margin-bottom: 15px;
        }
        
        body.dark-mode .payment-icon {
            color: var(--white);
        }
        
        .payment-card h3 {
            font-size: 20px;
        }
        
        .payment-note {
            background: rgba(212, 175, 55, 0.1);
            border-left: 4px solid var(--gold);
            padding: 20px;
            border-radius: 0 8px 8px 0;
            margin-top: 30px;
            font-weight: 500;
            font-size: 18px;
            color: var(--dark-blue);
        }
        
        body.dark-mode .payment-note {
            background: rgba(212, 175, 55, 0.15);
            color: var(--white);
        }
        
        /* Footer */
        footer {
            background: var(--dark-blue);
            color: var(--white);
            padding: 70px 0 0;
            transition: background-color 0.3s ease;
        }
        
        body.dark-mode footer {
            background: #081a2d;
        }
        
        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 50px;
        }
        
        .footer-col h3 {
            color: var(--gold);
            font-size: 24px;
            margin-bottom: 25px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-col h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 40px;
            height: 2px;
            background: var(--gold);
        }
        
        .footer-links {
            list-style: none;
            margin-top: 20px;
        }
        
        .footer-links li {
            margin-bottom: 12px;
        }
        
        .footer-links a {
            color: rgba(255, 255, 255, 0.7);
            text-decoration: none;
            transition: var(--transition);
            display: block;
            padding: 5px 0;
        }
        
        .footer-links a:hover {
            color: var(--gold);
            transform: translateX(5px);
        }
        
        .footer-links i {
            margin-left: 10px;
            color: var(--gold);
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 25px;
        }
        
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 45px;
            height: 45px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            color: var(--white);
            font-size: 18px;
            transition: var(--transition);
            text-decoration: none;
        }
        
        .social-links a:hover {
            background: var(--gold);
            transform: translateY(-3px);
            color: var(--dark-blue);
        }
        
        .partners {
            background: rgba(0, 0, 0, 0.2);
            padding: 30px 0;
            margin-top: 50px;
        }
        
        body.dark-mode .partners {
            background: rgba(0, 0, 0, 0.4);
        }
        
        .partners-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 30px;
            align-items: center;
        }
        
        .partner-logo {
            height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            color: var(--white);
            font-weight: 600;
            font-size: 24px;
            transition: var(--transition);
        }
        
        .partner-logo:hover {
            background: var(--gold);
            color: var(--dark-blue);
            transform: scale(1.05);
        }
        
        .copyright {
            text-align: center;
            padding: 25px 0;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 16px;
            color: rgba(255, 255, 255, 0.6);
        }
        
        body.dark-mode .copyright {
            border-top-color: rgba(255, 255, 255, 0.2);
        }
        
        /* WhatsApp Button */
        .whatsapp-float {
            position: fixed;
            width: 60px;
            height: 60px;
            bottom: 40px;
            left: 30px;
            background: #25D366;
            color: white;
            border-radius: 50px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(37, 211, 102, 0.4);
            z-index: 100;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            transition: var(--transition);
            animation: pulse 2s infinite;
            text-decoration: none;
        }
        
        .whatsapp-float:hover {
            transform: scale(1.1) rotate(10deg);
            box-shadow: 0 6px 20px rgba(37, 211, 102, 0.6);
        }
        
        /* Auth Modals */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.7);
            z-index: 2000;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .modal-content {
            background: var(--white);
            width: 100%;
            max-width: 500px;
            border-radius: var(--border-radius-lg);
            padding: 40px;
            position: relative;
            max-height: 90vh;
            overflow-y: auto;
            box-shadow: 0 15px 50px rgba(0, 0, 0, 0.3);
            animation: modalOpen 0.4s ease;
        }
        
        body.dark-mode .modal-content {
            background: var(--dark-blue);
            color: var(--white);
        }
        
        @keyframes modalOpen {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .close-modal {
            position: absolute;
            top: 20px;
            left: 20px;
            font-size: 32px;
            cursor: pointer;
            color: var(--gray);
            transition: var(--transition);
        }
        
        body.dark-mode .close-modal {
            color: var(--white);
        }
        
        .close-modal:hover {
            color: var(--dark-blue);
            transform: rotate(90deg);
        }
        
        body.dark-mode .close-modal:hover {
            color: var(--gold);
        }
        
        .modal-title {
            text-align: center;
            margin-bottom: 30px;
            font-size: 32px;
            color: var(--dark-blue);
        }
        
        body.dark-mode .modal-title {
            color: var(--white);
        }
        
        .modal-title i {
            color: var(--gold);
            margin-left: 10px;
        }
        
        .auth-form .form-group {
            margin-bottom: 20px;
        }
        
        .auth-form input {
            width: 100%;
            padding: 15px;
            border: 2px solid #ddd;
            border-radius: 10px;
            font-family: 'Cairo', sans-serif;
            font-size: 16px;
            transition: var(--transition);
            background-color: var(--white);
            color: var(--dark-blue);
        }
        
        body.dark-mode .auth-form input {
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--white);
            border-color: rgba(255, 255, 255, 0.3);
        }
        
        .auth-form input:focus {
            border-color: var(--gold);
            outline: none;
            box-shadow: 0 0 0 3px rgba(212, 175, 55, 0.2);
        }
        
        .form-label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            color: var(--dark-blue);
        }
        
        body.dark-mode .form-label {
            color: var(--white);
        }
        
        .auth-options {
            display: flex;
            justify-content: space-between;
            margin: 15px 0;
            font-size: 14px;
        }
        
        .auth-link {
            color: var(--gold);
            text-decoration: none;
            font-weight: 600;
            transition: var(--transition);
        }
        
        .auth-link:hover {
            color: var(--gold-dark);
            text-decoration: underline;
        }
        
        .social-login {
            text-align: center;
            margin: 25px 0;
            position: relative;
        }
        
        .social-login::before,
        .social-login::after {
            content: '';
            position: absolute;
            top: 50%;
            width: 40%;
            height: 1px;
            background: #ddd;
        }
        
        body.dark-mode .social-login::before,
        body.dark-mode .social-login::after {
            background: rgba(255, 255, 255, 0.3);
        }
        
        .social-login::before {
            left: 0;
        }
        
        .social-login::after {
            right: 0;
        }
        
        .social-login span {
            background: var(--white);
            padding: 0 15px;
            position: relative;
            color: var(--gray);
            font-size: 14px;
        }
        
        body.dark-mode .social-login span {
            background: var(--dark-blue);
            color: #b0b0b0;
        }
        
        .social-btns {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 15px;
        }
        
        .social-btn {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 20px;
            color: white;
            transition: var(--transition);
            border: none;
            cursor: pointer;
        }
        
        .social-btn.facebook { background: #3b5998; }
        .social-btn.google { background: #db4437; }
        .social-btn.apple { background: #000; }
        
        .social-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        /* Animations */
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.6); }
            70% { box-shadow: 0 0 0 15px rgba(37, 211, 102, 0); }
            100% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0); }
        }
        
        /* Responsive Design */
        @media (max-width: 992px) {
            :root {
                --section-padding: 60px 0;
            }
            
            .hero h1 {
                font-size: 44px;
            }
            
            .hero p {
                font-size: 20px;
            }
            
            nav ul {
                gap: 15px;
            }
            
            nav a {
                font-size: 16px;
            }
            
            .header-actions {
                gap: 10px;
            }
            
            .theme-toggle, .user-btn {
                width: 42px;
                height: 42px;
                font-size: 18px;
            }
        }
        
        @media (max-width: 768px) {
            .mobile-menu-btn {
                display: block;
            }
            
            nav ul {
                position: fixed;
                top: 80px;
                right: -100%;
                flex-direction: column;
                background: var(--white);
                width: 80%;
                height: calc(100vh - 80px);
                padding: 30px;
                box-shadow: -5px 0 15px rgba(0, 0, 0, 0.1);
                transition: var(--transition);
                z-index: 999;
            }
            
            body.dark-mode nav ul {
                background: var(--dark-blue);
                box-shadow: -5px 0 15px rgba(0, 0, 0, 0.4);
            }
            
            nav ul.active {
                right: 0;
            }
            
            .hero h1 {
                font-size: 36px;
            }
            
            .hero p {
                font-size: 18px;
            }
            
            .hero-buttons .btn {
                padding: 14px 25px;
                font-size: 18px;
            }
            
            .section-title h2 {
                font-size: 30px;
            }
            
            .section-title p {
                font-size: 16px;
            }
            
            .whatsapp-float {
                width: 50px;
                height: 50px;
                font-size: 24px;
                left: 20px;
                bottom: 25px;
            }
            
            .header-actions {
                display: none;
            }
            
            .mobile-actions {
                display: flex;
                align-items: center;
                gap: 15px;
            }
            
            .countdown {
                flex-wrap: wrap;
            }
        }
        
        @media (max-width: 480px) {
            :root {
                --section-padding: 40px 0;
            }
            
            .header-container {
                padding: 0 15px;
            }
            
            .hero h1 {
                font-size: 32px;
            }
            
            .hero p {
                font-size: 16px;
            }
            
            .hero-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .section-title h2 {
                font-size: 26px;
            }
            
            .service-card {
                padding: 25px 15px;
            }
            
            .service-icon {
                font-size: 40px;
                width: 70px;
                height: 70px;
                line-height: 70px;
            }
            
            .tour-price {
                font-size: 24px;
            }
            
            .appointment-form {
                padding: 25px 20px;
            }
            
            .modal-content {
                padding: 30px 25px;
            }
            
            .modal-title {
                font-size: 28px;
            }
            
            .close-modal {
                font-size: 28px;
            }
        }
    </style>
</head>
<body>
    <!-- WhatsApp Floating Button - Updated with Libyan number -->
    <a href="https://wa.me/218945175611" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <i class="fas fa-globe-asia logo-icon"></i>
                <div class="logo-text">الرحّال <span>للخدمات السياحية</span></div>
            </div>
            
            <div class="mobile-actions">
                <button class="theme-toggle" id="themeToggle">
                    <i class="fas fa-moon"></i>
                </button>
                <button class="user-btn" id="userBtn">
                    <i class="fas fa-user"></i>
                </button>
                <button class="mobile-menu-btn" id="mobileMenuBtn">
                    <i class="fas fa-bars"></i>
                </button>
            </div>
            
            <div class="header-actions">
                <button class="theme-toggle" id="themeToggleDesktop">
                    <i class="fas fa-moon"></i>
                </button>
                <div class="user-menu">
                    <button class="user-btn" id="userBtnDesktop">
                        <i class="fas fa-user"></i>
                    </button>
                    <div class="user-dropdown" id="userDropdown">
                        <a href="#" class="dropdown-item" id="loginLink">
                            <i class="fas fa-sign-in-alt"></i> تسجيل الدخول
                        </a>
                        <a href="#" class="dropdown-item" id="registerLink">
                            <i class="fas fa-user-plus"></i> إنشاء حساب
                        </a>
                        <a href="#" class="dropdown-item" id="dashboardLink" style="display:none;">
                            <i class="fas fa-tachometer-alt"></i> لوحة التحكم
                        </a>
                        <a href="#" class="dropdown-item" id="bookingsLink" style="display:none;">
                            <i class="fas fa-ticket-alt"></i> حجوزاتي
                        </a>
                        <a href="#" class="dropdown-item" id="favoritesLink" style="display:none;">
                            <i class="fas fa-heart"></i> المفضلة
                        </a>
                        <a href="#" class="dropdown-item" id="settingsLink" style="display:none;">
                            <i class="fas fa-cog"></i> الإعدادات
                        </a>
                        <a href="#" class="dropdown-item" id="logoutLink" style="display:none; color:#dc3545;">
                            <i class="fas fa-sign-out-alt"></i> تسجيل الخروج
                        </a>
                    </div>
                </div>
            </div>
            
            <nav>
                <ul>
                    <li><a href="#home" class="active">الرئيسية</a></li>
                    <li><a href="#about">من نحن</a></li>
                    <li><a href="#services">الخدمات</a></li>
                    <li><a href="#tours">البرامج السياحية</a></li>
                    <li><a href="#offers">العروض</a></li>
                    <li><a href="#faq">الأسئلة</a></li>
                    <li><a href="#contact">اتصل بنا</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container hero-content">
            <h1>كل خدمات سفرك في مكان واحد</h1>
            <p>الرحّال… لأن رحلتك تستاهل الأفضل</p>
            <div class="hero-buttons">
                <a href="#services" class="btn">استكشف خدماتنا</a>
                <a href="https://wa.me/218945175611" class="btn btn-whatsapp" target="_blank">
                    <i class="fab fa-whatsapp"></i> تواصل عبر الواتساب
                </a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>خدماتنا المتكاملة</h2>
                <p>نقدم لك كل ما تحتاجه لرحلة مثالية ومريحة، من التخطيط إلى التنفيذ</p>
            </div>
            
            <div class="services-grid">
                <div class="service-card">
                    <i class="fas fa-plane service-icon"></i>
                    <h3>حجز تذاكر طيران</h3>
                    <p>أفضل الأسعار والخيارات لجميع الوجهات العالمية مع دعم فوري</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-hotel service-icon"></i>
                    <h3>حجز فنادق</h3>
                    <p>مجموعة متنوعة من الفنادق تناسب جميع الميزانيات والتفضيلات</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-passport service-icon"></i>
                    <h3>استخراج تأشيرات</h3>
                    <p>مساعدة احترافية في استخراج جميع أنواع التأشيرات بسهولة</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-globe service-icon"></i>
                    <h3>برامج سياحية</h3>
                    <p>رحلات مصممة خصيصاً لاستكشاف أجمل الوجهات حول العالم</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-ring service-icon"></i>
                    <h3>رحلات شهر العسل</h3>
                    <p>باقات رومانسية متكاملة لتجربة لا تُنسى في أفضل الوجهات</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-briefcase service-icon"></i>
                    <h3>خدمات الشركات</h3>
                    <p>حلول سفر مخصصة للشركات ورحلات العمل مع متابعة مستمرة</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-suitcase-rolling service-icon"></i>
                    <h3>باقات سفر متكاملة</h3>
                    <p>باقات شاملة تغطي جميع جوانب رحلتك بأسعار تنافسية</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-tag service-icon"></i>
                    <h3>العروض الخاصة</h3>
                    <p>عروض حصرية وتخفيضات مميزة على مختلف الخدمات السياحية</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Trust Line - Updated with Libya location -->
    <div class="trust-line">
        <div class="container">
            <i class="fas fa-map-marker-alt"></i> مكتبنا في ليبيا - بني وليد | مكتب فعلي لخدمتكم
        </div>
    </div>

    <!-- Why Us Section -->
    <section class="features" id="why-us">
        <div class="container">
            <div class="section-title">
                <h2>لماذا تختار الرحّال؟</h2>
                <p>نقدم لك تجربة سفر استثنائية مدعومة بخبرة سنوات وشراكات عالمية</p>
            </div>
            
            <div class="features-grid">
                <div class="feature-card">
                    <i class="fas fa-dollar-sign feature-icon"></i>
                    <h3>أسعار منافسة</h3>
                    <p>نضمن لك أفضل الأسعار بفضل شراكاتنا الاستراتيجية مع شركات الطيران والفنادق العالمية</p>
                </div>
                <div class="feature-card">
                    <i class="fas fa-medal feature-icon"></i>
                    <h3>خبرة في السفر</h3>
                    <p>فريق من الخبراء المتخصصين في مجال السفر والسياحة لضمان تجربة مثالية</p>
                </div>
                <div class="feature-card">
                    <i class="fas fa-headset feature-icon"></i>
                    <h3>دعم مستمر</h3>
                    <p>دعم فوري على مدار الساعة قبل وأثناء وبعد رحلتك لضمان راحتك التامة</p>
                </div>
                <div class="feature-card">
                    <i class="fas fa-bolt feature-icon"></i>
                    <h3>سرعة إنجاز</h3>
                    <p>إجراءات سريعة وفعالة لجميع خدماتك مع متابعة دقيقة لكل تفصيل</p>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <div class="section-title">
                <h2>من نحن</h2>
                <p>تعرف على قصتنا ورؤيتنا في عالم السفر والسياحة</p>
            </div>
            
            <div class="about-content">
                <div class="about-text">
                    <h2>رحلة بدأت بالشغف ووصلت للعالمية</h2>
                    <p>تأسست شركة الرحّال للخدمات السياحية بهدف تقديم تجربة سفر استثنائية لكل مسافر. نفخر بكوننا أحد أبرز مزودي الخدمات السياحية في ليبيا، وتحديداً في مدينة بني وليد.</p>
                    <p>نسعى دائماً لتقديم أفضل الخدمات بأسعار تنافسية، معتمدين على شراكات استراتيجية مع كبرى شركات الطيران والفنادق العالمية. فريقنا من الخبراء يعمل على مدار الساعة لضمان رحلتك المثالية من التخطيط وحتى العودة.</p>
                    <p><strong>رؤيتنا:</strong> أن نكون الخيار الأول للمسافر الليبي، ونساهم في تعزيز السياحة وخلق تجارب لا تُنسى.</p>
                    <p><strong>رسالتنا:</strong> تقديم خدمات سياحية متكاملة بجودة عالية، مع التركيز على رضا العملاء وبناء علاقات طويلة الأمد.</p>
                    
                    <div class="about-stats">
                        <div class="stat-item">
                            <div class="stat-number">8+</div>
                            <div class="stat-label">سنوات خبرة</div>
                        </div>
                        <div class="stat-item">
                            <div class="stat-number">15K+</div>
                            <div class="stat-label">عميل سعيد</div>
                        </div>
                        <div class="stat-item">
                            <div class="stat-number">100+</div>
                            <div class="stat-label">وجهة عالمية</div>
                        </div>
                        <div class="stat-item">
                            <div class="stat-number">24/7</div>
                            <div class="stat-label">دعم فوري</div>
                        </div>
                    </div>
                </div>
                <div class="about-img">
                    <img src="https://images.unsplash.com/photo-1529626455594-4ff0e0d011cb?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80" alt="فريق الرحّال">
                </div>
            </div>
        </div>
    </section>

    <!-- Tours Section -->
    <section class="tours" id="tours">
        <div class="container">
            <div class="section-title">
                <h2>البرامج السياحية المميزة</h2>
                <p>استكشف أجمل الوجهات حول العالم مع برامجنا المصممة خصيصاً لتناسب احتياجاتك</p>
            </div>
            
            <div class="tours-grid">
                <div class="tour-card">
                    <div class="tour-img">
                        <img src="https://images.unsplash.com/photo-1524231757912-21f4fe3a72bc?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80" alt="تركيا">
                    </div>
                    <div class="tour-content">
                        <h3 class="tour-title">جولة ساحرة في تركيا</h3>
                        <div class="tour-duration">8 أيام / 7 ليالي</div>
                        <p>استكشف إسطنبول وأنطاليا وكابادوكيا في رحلة لا تُنسى</p>
                        <div class="tour-price">1,199 د.ل <span>لكل شخص</span></div>
                        <a href="https://wa.me/218945175611" class="btn btn-whatsapp" target="_blank">
                            <i class="fab fa-whatsapp"></i> احجز الآن
                        </a>
                    </div>
                </div>
                
                <div class="tour-card">
                    <div class="tour-img">
                        <img src="https://images.unsplash.com/photo-1566912621240-f54c3a5c9bad?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80" alt="دبي">
                    </div>
                    <div class="tour-content">
                        <h3 class="tour-title">دبي - عاصمة العراقة والحداثة</h3>
                        <div class="tour-duration">5 أيام / 4 ليالي</div>
                        <p>تجربة فريدة بين الأصالة والتطور في واحدة من أجمل مدن العالم</p>
                        <div class="tour-price">1,899 د.ل <span>لكل شخص</span></div>
                        <a href="https://wa.me/218945175611" class="btn btn-whatsapp" target="_blank">
                            <i class="fab fa-whatsapp"></i> احجز الآن
                        </a>
                    </div>
                </div>
                
                <div class="tour-card">
                    <div class="tour-img">
                        <img src="https://images.unsplash.com/photo-1530122034255-8e3bc8c643c4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80" alt="اليونان">
                    </div>
                    <div class="tour-content">
                        <h3 class="tour-title">سحر الجزر اليونانية</h3>
                        <div class="tour-duration">10 أيام / 9 ليالي</div>
                        <p>رحلة أسطورية إلى جزر سانتوريني وميكونوس وأثينا</p>
                        <div class="tour-price">2,499 د.ل <span>لكل شخص</span></div>
                        <a href="https://wa.me/218945175611" class="btn btn-whatsapp" target="_blank">
                            <i class="fab fa-whatsapp"></i> احجز الآن
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Offers Section -->
    <section class="offers" id="offers">
        <div class="container">
            <div class="section-title">
                <h2>العروض الحصرية</h2>
                <p>استفد من أفضل العروض والتخفيضات المحدودة الوقت</p>
            </div>
            
            <div class="offers-grid">
                <div class="offer-card">
                    <div class="offer-badge">خصم 40%</div>
                    <div class="offer-img">
                        <img src="https://images.unsplash.com/photo-1551882547-ff40c63fe5fa?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80" alt="عروض ماليزيا">
                    </div>
                    <div class="offer-content">
                        <h3 class="offer-title">رحلة عائلية إلى ماليزيا</h3>
                        <p>باقة شاملة للطيران + الإقامة + التنقلات</p>
                        <div>
                            <span class="offer-old-price">3,200 د.ل</span>
                            <span class="offer-new-price">1,920 د.ل</span>
                        </div>
                        <div class="offer-savings">وفر 1,280 د.ل</div>
                        <div class="countdown">
                            <div class="countdown-item">
                                <span class="countdown-number" id="days1">03</span>
                                <span class="countdown-label">أيام</span>
                            </div>
                            <div class="countdown-item">
                                <span class="countdown-number" id="hours1">12</span>
                                <span class="countdown-label">ساعات</span>
                            </div>
                            <div class="countdown-item">
                                <span class="countdown-number" id="minutes1">45</span>
                                <span class="countdown-label">دقائق</span>
                            </div>
                        </div>
                        <a href="https://wa.me/218945175611" class="btn btn-primary" style="margin-top: 15px; width: 100%;" target="_blank">
                            احجز العرض الآن
                        </a>
                    </div>
                </div>
                
                <div class="offer-card">
                    <div class="offer-badge">عرض خاص</div>
                    <div class="offer-img">
                        <img src="https://images.unsplash.com/photo-1518609878373-06d740f60d8b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80" alt="عروض باريس">
                    </div>
                    <div class="offer-content">
                        <h3 class="offer-title">شهر عسل في باريس</h3>
                        <p>باقة رومانسية شاملة مع جولات خاصة</p>
                        <div>
                            <span class="offer-old-price">5,800 د.ل</span>
                            <span class="offer-new-price">3,600 د.ل</span>
                        </div>
                        <div class="offer-savings">وفر 2,200 د.ل</div>
                        <div class="countdown">
                            <div class="countdown-item">
                                <span class="countdown-number" id="days2">05</span>
                                <span class="countdown-label">أيام</span>
                            </div>
                            <div class="countdown-item">
                                <span class="countdown-number" id="hours2">08</span>
                                <span class="countdown-label">ساعات</span>
                            </div>
                            <div class="countdown-item">
                                <span class="countdown-number" id="minutes2">30</span>
                                <span class="countdown-label">دقائق</span>
                            </div>
                        </div>
                        <a href="https://wa.me/218945175611" class="btn btn-primary" style="margin-top: 15px; width: 100%;" target="_blank">
                            احجز العرض الآن
                        </a>
                    </div>
                </div>
                
                <div class="offer-card">
                    <div class="offer-badge">فقط اليوم</div>
                    <div class="offer-img">
                        <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1740&q=80" alt="عروض مصر">
                    </div>
                    <div class="offer-content">
                        <h3 class="offer-title">رحلة إلى الأهرامات - مصر</h3>
                        <p>باقة سياحية شاملة مع مرشد سياحي</p>
                        <div>
                            <span class="offer-old-price">1,850 د.ل</span>
                            <span class="offer-new-price">1,050 د.ل</span>
                        </div>
                        <div class="offer-savings">وفر 800 د.ل</div>
                        <div class="countdown">
                            <div class="countdown-item">
                                <span class="countdown-number" id="days3">00</span>
                                <span class="countdown-label">أيام</span>
                            </div>
                            <div class="countdown-item">
                                <span class="countdown-number" id="hours3">18</span>
                                <span class="countdown-label">ساعات</span>
                            </div>
                            <div class="countdown-item">
                                <span class="countdown-number" id="minutes3">15</span>
                                <span class="countdown-label">دقائق</span>
                            </div>
                        </div>
                        <a href="https://wa.me/218945175611" class="btn btn-primary" style="margin-top: 15px; width: 100%;" target="_blank">
                            احجز العرض الآن
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials" id="testimonials">
        <div class="container">
            <div class="section-title">
                <h2>آراء عملائنا</h2>
                <p>نفخر بثقة عملائنا ورضاهم عن خدماتنا المتكاملة</p>
            </div>
            
            <div class="testimonials-grid">
                <div class="testimonial-card">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p class="testimonial-text">"تعاملت مع الرحّال لحجز رحلة شهر العسل إلى تركيا، وكانت التجربة ممتازة من البداية حتى النهاية. الفريق محترف وسريع في الرد على جميع استفساراتي، والأسعار كانت أفضل من غيرهم. أنصح الجميع بالتعامل معهم!"</p>
                    <div class="testimonial-author">أحمد الساحلي</div>
                    <div class="author-title">عميل من بني وليد</div>
                </div>
                
                <div class="testimonial-card">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p class="testimonial-text">"كنت أبحث عن برنامج سياحي شامل لأسرتي إلى دبي، ووجدت في الرحّال كل ما أحتاجه. البرنامج كان ممتازاً، الفنادق رائعة، والمرشد السياحي كان على قدر عالٍ من الاحترافية. شكراً لتجربة لا تُنسى!"</p>
                    <div class="testimonial-author">فاطمة الزنتاني</div>
                    <div class="author-title">عميلة من طرابلس</div>
                </div>
                
                <div class="testimonial-card">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star-half-alt"></i>
                    </div>
                    <p class="testimonial-text">"تعاملت معهم لحجز تذاكر طيران لرحلة عمل عاجلة، وأبهرني سرعة الإنجاز والاحترافية. تمكنت من السفر في الوقت المطلوب دون أي تعقيدات. سأتعامل معهم دائماً لجميع احتياجاتي السفرية."</p>
                    <div class="testimonial-author">خالد الورفلي</div>
                    <div class="author-title">عميل دائم</div>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section class="faq" id="faq">
        <div class="container">
            <div class="section-title">
                <h2>الأسئلة الشائعة</h2>
                <p>أجوبة على أكثر الأسئلة التي يطرحها عملاؤنا</p>
            </div>
            
            <div class="faq-container">
                <div class="faq-item">
                    <div class="faq-question">
                        <span>كيف يمكنني حجز تذكرة طيران؟</span>
                        <i class="fas fa-chevron-down faq-toggle"></i>
                    </div>
                    <div class="faq-answer">
                        <p>يمكنك حجز تذكرة طيران من خلال الاتصال بنا عبر الواتساب أو زيارة مكتبنا في بني وليد. سنساعدك في اختيار أفضل الخيارات من حيث السعر والمواعيد، وسنقوم بحجز التذكرة فوراً مع إرسال التأكيد إليك.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question">
                        <span>ما هي المستندات المطلوبة لاستخراج تأشيرة شنغن؟</span>
                        <i class="fas fa-chevron-down faq-toggle"></i>
                    </div>
                    <div class="faq-answer">
                        <p>المستندات المطلوبة لتأشيرة شنغن تشمل: جواز سفر ساري المفعول، صور شخصية حديثة، كشف حساب بنكي لآخر 6 أشهر، خطاب من جهة العمل، حجز طيران وفندق، وتأمين سفر يغطي مدة الرحلة. نوفر لك قائمة مفصلة حسب الدولة المطلوبة.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question">
                        <span>هل يمكنني الدفع بعد تأكيد الحجز؟</span>
                        <i class="fas fa-chevron-down faq-toggle"></i>
                    </div>
                    <div class="faq-answer">
                        <p>نعم، نوفر خيار الدفع بعد التأكيد لبعض الخدمات مثل حجوزات الفنادق وبرامج السفر المتكاملة. يمكنك دفع جزء من المبلغ كعربون والباقي عند الاستلام أو قبل السفر بفترة محددة حسب نوع الخدمة.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question">
                        <span>ما هي سياسة الإلغاء والاسترجاع؟</span>
                        <i class="fas fa-chevron-down faq-toggle"></i>
                    </div>
                    <div class="faq-answer">
                        <p>تختلف سياسة الإلغاء حسب نوع الخدمة وشركة الطيران أو الفندق. بشكل عام، يمكن إلغاء الحجوزات قبل 72 ساعة من موعد السفر مع استرداد جزئي أو كامل حسب الشروط. ننصح دائماً بقراءة الشروط قبل الحجز، وفريقنا جاهز لشرح جميع التفاصيل.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question">
                        <span>هل تقدمون خدمات للشركات ورحلات العمل؟</span>
                        <i class="fas fa-chevron-down faq-toggle"></i>
                    </div>
                    <div class="faq-answer">
                        <p>نعم، لدينا قسم متخصص في خدمات الشركات يوفر حلولاً متكاملة لرحلات العمل بما في ذلك حجز الطيران، الفنادق، التنقلات، وتنظيم المؤتمرات. نقدم عروضاً خاصة للشركات مع متابعة مخصصة وفواتير رسمية.</p>
                    </div>
                </div>
                
                <div class="faq-item">
                    <div class="faq-question">
                        <span>كيف يمكنني حجز موعد لزيارة المكتب؟</span>
                        <i class="fas fa-chevron-down faq-toggle"></i>
                    </div>
                    <div class="faq-answer">
                        <p>يمكنك حجز موعد لزيارة مكتبنا من خلال ملء نموذج الحجز في قسم "اتصل بنا" أو الاتصال مباشرة على الرقم 0945175611. نحرص على تخصيص وقت كافٍ لكل عميل لضمان تقديم أفضل خدمة.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section - Updated with Libya info -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>اتصل بنا</h2>
                <p>فريقنا جاهز لخدمتك ومساعدتك في تخطيط رحلتك المثالية</p>
            </div>
            
            <div class="contact-container">
                <div class="contact-info">
                    <div class="contact-item">
                        <i class="fas fa-map-marker-alt contact-icon"></i>
                        <div>
                            <h3>مكتبنا</h3>
                            <p>طريق المطار، بني وليد، ليبيا</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <i class="fas fa-phone contact-icon"></i>
                        <div>
                            <h3>اتصل بنا</h3>
                            <p><i class="fas fa-phone"></i> 0945175611</p>
                            <p><i class="fas fa-mobile-alt"></i> 091-234-5678 (دعم فني)</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <i class="fas fa-envelope contact-icon"></i>
                        <div>
                            <h3>راسلنا</h3>
                            <p><i class="fas fa-envelope"></i> <a href="mailto:AlRahal.travel0@gmail.com" style="color: var(--dark-blue); text-decoration: none;">AlRahal.travel0@gmail.com</a></p>
                            <p><i class="fas fa-headset"></i> support@alrahhal.ly</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <i class="fas fa-clock contact-icon"></i>
                        <div>
                            <h3>ساعات العمل</h3>
                            <p><i class="fas fa-calendar"></i> من السبت إلى الخميس: 9:00 صباحاً - 9:00 مساءً</p>
                            <p><i class="fas fa-calendar"></i> الجمعة: مغلق</p>
                        </div>
                    </div>
                </div>
                
                <div class="contact-form">
                    <form id="contactForm">
                        <div class="form-group">
                            <input type="text" placeholder="الاسم الكامل" required>
                        </div>
                        <div class="form-group">
                            <input type="email" placeholder="البريد الإلكتروني" required>
                        </div>
                        <div class="form-group">
                            <input type="tel" placeholder="رقم الجوال" required>
                        </div>
                        <div class="form-group">
                            <select required>
                                <option value="" disabled selected>نوع الاستفسار</option>
                                <option value="flights">حجز طيران</option>
                                <option value="visa">استخراج تأشيرة</option>
                                <option value="hotel">حجز فندق</option>
                                <option value="tour">برنامج سياحي</option>
                                <option value="honeymoon">رحلة شهر عسل</option>
                                <option value="business">خدمات شركات</option>
                                <option value="other">أخرى</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <textarea placeholder="رسالتك" required></textarea>
                        </div>
                        <button type="submit" class="btn">إرسال الرسالة</button>
                    </form>
                </div>
            </div>
            
            <div class="map-container">
                <a href="https://maps.app.goo.gl/Va1nHymHrQ1DP97N6" class="map-link" target="_blank">
                    <i class="fas fa-map-marked-alt"></i>
                    <h3>موقع مكتبنا في بني وليد</h3>
                    <p>اضغط هنا لفتح الموقع على خرائط جوجل</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Payment Section -->
    <section class="payment-methods">
        <div class="container">
            <div class="section-title">
                <h2>طرق الدفع المتاحة</h2>
                <p>نقدم لك مرونة في الدفع لتناسب جميع احتياجاتك</p>
            </div>
            
            <div class="payment-grid">
                <div class="payment-card">
                    <i class="fas fa-money-bill-wave payment-icon"></i>
                    <h3>نقداً في المكتب</h3>
                    <p>ادفع نقداً عند زيارة مكتبنا في بني وليد</p>
                </div>
                <div class="payment-card">
                    <i class="fas fa-credit-card payment-icon"></i>
                    <h3>بطاقات مصرفية</h3>
                    <p>Visa / MasterCard / Mada</p>
                </div>
                <div class="payment-card">
                    <i class="fas fa-file-invoice-dollar payment-icon"></i>
                    <h3>حوالة بنكية</h3>
                    <p>حوّل المبلغ إلى حسابنا البنكي</p>
                </div>
                <div class="payment-card">
                    <i class="fas fa-wallet payment-icon"></i>
                    <h3>محافظ إلكترونية</h3>
                    <p>PayPal، محافظ الهواتف المحلية</p>
                </div>
            </div>
            
            <div class="payment-note">
                <i class="fas fa-shield-alt" style="margin-left:10px;"></i>
                سيتم التواصل معك لتأكيد الحجز وإتمام الدفع بأمان
            </div>
        </div>
    </section>

    <!-- Footer - Updated with Libya info -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <div class="footer-col">
                    <div class="logo">
                        <i class="fas fa-globe-asia logo-icon"></i>
                        <div class="logo-text">الرحّال <span>للخدمات السياحية</span></div>
                    </div>
                    <p style="margin: 25px 0 20px; line-height: 1.7; color: rgba(255,255,255,0.7);">
                        شركة ليبية متكاملة تقدم جميع خدمات السفر: تذاكر طيران، تأشيرات، فنادق، برامج سياحية، رحلات شهر عسل، رحلات عمل، وباقات سفر كاملة.
                    </p>
                    <div class="social-links">
                        <a href="https://wa.me/218945175611" target="_blank">
                            <i class="fab fa-whatsapp"></i>
                        </a>
                        <a href="https://www.facebook.com/share/1CzZreEnTj/" target="_blank">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="https://www.instagram.com/raha.l09?igsh=MXkyNW95NnV1YzV3eg==" target="_blank">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="https://www.tiktok.com/@al.rah.al?_r=1&_t=ZS-93brFWUOeOn" target="_blank">
                            <i class="fab fa-tiktok"></i>
                        </a>
                    </div>
                </div>
                
                <div class="footer-col">
                    <h3>روابط سريعة</h3>
                    <ul class="footer-links">
                        <li><a href="#home"><i class="fas fa-chevron-left"></i> الرئيسية</a></li>
                        <li><a href="#about"><i class="fas fa-chevron-left"></i> من نحن</a></li>
                        <li><a href="#services"><i class="fas fa-chevron-left"></i> خدماتنا</a></li>
                        <li><a href="#tours"><i class="fas fa-chevron-left"></i> البرامج السياحية</a></li>
                        <li><a href="#offers"><i class="fas fa-chevron-left"></i> العروض الخاصة</a></li>
                        <li><a href="#faq"><i class="fas fa-chevron-left"></i> الأسئلة الشائعة</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h3>خدماتنا</h3>
                    <ul class="footer-links">
                        <li><a href="#"><i class="fas fa-chevron-left"></i> حجز تذاكر طيران</a></li>
                        <li><a href="#"><i class="fas fa-chevron-left"></i> استخراج تأشيرات</a></li>
                        <li><a href="#"><i class="fas fa-chevron-left"></i> حجز فنادق</a></li>
                        <li><a href="#"><i class="fas fa-chevron-left"></i> برامج سياحية</a></li>
                        <li><a href="#"><i class="fas fa-chevron-left"></i> رحلات شهر العسل</a></li>
                        <li><a href="#"><i class="fas fa-chevron-left"></i> خدمات الشركات</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h3>معلومات الاتصال</h3>
                    <ul class="footer-links">
                        <li>
                            <i class="fas fa-map-marker-alt"></i>
                            طريق المطار، بني وليد، ليبيا
                        </li>
                        <li>
                            <i class="fas fa-phone"></i>
                            0945175611
                        </li>
                        <li>
                            <i class="fas fa-envelope"></i>
                            <a href="mailto:AlRahal.travel0@gmail.com" style="color: rgba(255,255,255,0.7); text-decoration: none;">AlRahal.travel0@gmail.com</a>
                        </li>
                        <li>
                            <i class="fas fa-clock"></i>
                            السبت - الخميس: 9 صباحاً - 9 مساءً<br>
                            الجمعة: مغلق
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="partners">
                <div class="container">
                    <div class="partners-grid">
                        <div class="partner-logo">Libyan Airlines</div>
                        <div class="partner-logo">Turkish Airlines</div>
                        <div class="partner-logo">Rotana</div>
                        <div class="partner-logo">Hilton</div>
                        <div class="partner-logo">Visa</div>
                        <div class="partner-logo">MasterCard</div>
                    </div>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2026 الرحّال للخدمات السياحية. جميع الحقوق محفوظة. | 
                   <a href="#" style="color: var(--gold); text-decoration: underline;">سياسة الخصوصية</a> | 
                   <a href="#" style="color: var(--gold); text-decoration: underline;">شروط الاستخدام</a> |
                   <a href="#" style="color: var(--gold); text-decoration: underline;">خريطة الموقع</a>
                </p>
            </div>
        </div>
    </footer>

    <!-- Login Modal -->
    <div class="modal" id="loginModal">
        <div class="modal-content">
            <span class="close-modal" id="closeLogin">&times;</span>
            <h2 class="modal-title"><i class="fas fa-sign-in-alt"></i> تسجيل الدخول</h2>
            <form class="auth-form" id="loginForm">
                <div class="form-group">
                    <label class="form-label">البريد الإلكتروني أو رقم الجوال</label>
                    <input type="text" placeholder="example@email.com أو 09XXXXXXXX" required>
                </div>
                <div class="form-group">
                    <label class="form-label">كلمة المرور</label>
                    <input type="password" placeholder="أدخل كلمة المرور" required>
                </div>
                <div class="auth-options">
                    <label style="display:flex; align-items:center; gap:8px;">
                        <input type="checkbox"> تذكرني
                    </label>
                    <a href="#" class="auth-link">نسيت كلمة المرور؟</a>
                </div>
                <button type="submit" class="btn" style="width:100%;">
                    <i class="fas fa-sign-in-alt"></i> تسجيل الدخول
                </button>
            </form>
            
            <div class="social-login">
                <span>أو سجل الدخول باستخدام</span>
            </div>
            
            <div class="social-btns">
                <button class="social-btn facebook">
                    <i class="fab fa-facebook-f"></i>
                </button>
                <button class="social-btn google">
                    <i class="fab fa-google"></i>
                </button>
                <button class="social-btn apple">
                    <i class="fab fa-apple"></i>
                </button>
            </div>
            
            <div style="text-align:center; margin-top:25px; color:var(--gray);">
                ليس لديك حساب؟ <a href="#" class="auth-link" id="switchToRegisterModal">إنشاء حساب جديد</a>
            </div>
        </div>
    </div>

    <!-- Register Modal -->
    <div class="modal" id="registerModal">
        <div class="modal-content">
            <span class="close-modal" id="closeRegister">&times;</span>
            <h2 class="modal-title"><i class="fas fa-user-plus"></i> إنشاء حساب جديد</h2>
            <form class="auth-form" id="registerForm">
                <div class="form-group">
                    <label class="form-label">الاسم الكامل</label>
                    <input type="text" placeholder="أحمد محمد" required>
                </div>
                <div class="form-group">
                    <label class="form-label">رقم الجوال</label>
                    <input type="tel" placeholder="09XXXXXXXX" required>
                </div>
                <div class="form-group">
                    <label class="form-label">البريد الإلكتروني</label>
                    <input type="email" placeholder="example@email.com" required>
                </div>
                <div class="form-group">
                    <label class="form-label">كلمة المرور</label>
                    <input type="password" placeholder="كلمة مرور قوية (8+ أحرف)" required>
                </div>
                <div class="form-group">
                    <label class="form-label">تأكيد كلمة المرور</label>
                    <input type="password" placeholder="أعد إدخال كلمة المرور" required>
                </div>
                <div style="background:rgba(212, 175, 55, 0.1); padding:15px; border-radius:10px; margin:20px 0; font-size:14px;">
                    <i class="fas fa-shield-alt" style="color:var(--gold); margin-left:5px;"></i>
                    نحترم خصوصيتك ولن نشارك بياناتك مع أي جهة خارجية. سيتم تأكيد حسابك عبر رسالة نصية.
                </div>
                <button type="submit" class="btn" style="width:100%;">
                    <i class="fas fa-user-plus"></i> إنشاء الحساب
                </button>
            </form>
            
            <div style="text-align:center; margin-top:25px; color:var(--gray);">
                لديك حساب بالفعل؟ <a href="#" class="auth-link" id="switchToLoginModal">تسجيل الدخول</a>
            </div>
        </div>
    </div>

    <script>
        // ======================
        // نظام الوضع الداكن (Dark Mode) - مصحح
        // ======================
        const themeToggle = document.getElementById('themeToggle');
        const themeToggleDesktop = document.getElementById('themeToggleDesktop');
        const body = document.body;
        const themeIcon = document.querySelector('#themeToggle i');
        const themeIconDesktop = document.querySelector('#themeToggleDesktop i');
        
        // تحميل التفضيل من localStorage
        const savedTheme = localStorage.getItem('theme');
        if(savedTheme === 'dark') {
            body.classList.add('dark-mode');
            themeIcon.classList.replace('fa-moon', 'fa-sun');
            themeIconDesktop.classList.replace('fa-moon', 'fa-sun');
        }
        
        // تبديل الوضع
        function toggleTheme() {
            body.classList.toggle('dark-mode');
            
            if(body.classList.contains('dark-mode')) {
                localStorage.setItem('theme', 'dark');
                themeIcon.classList.replace('fa-moon', 'fa-sun');
                themeIconDesktop.classList.replace('fa-moon', 'fa-sun');
            } else {
                localStorage.setItem('theme', 'light');
                themeIcon.classList.replace('fa-sun', 'fa-moon');
                themeIconDesktop.classList.replace('fa-sun', 'fa-moon');
            }
        }
        
        if(themeToggle) themeToggle.addEventListener('click', toggleTheme);
        if(themeToggleDesktop) themeToggleDesktop.addEventListener('click', toggleTheme);
        
        // ======================
        // نظام تسجيل الدخول/التسجيل - مصحح
        // ======================
        const loginModal = document.getElementById('loginModal');
        const registerModal = document.getElementById('registerModal');
        const userBtn = document.getElementById('userBtn');
        const userBtnDesktop = document.getElementById('userBtnDesktop');
        const userDropdown = document.getElementById('userDropdown');
        const loginLink = document.getElementById('loginLink');
        const registerLink = document.getElementById('registerLink');
        const dashboardLink = document.getElementById('dashboardLink');
        const bookingsLink = document.getElementById('bookingsLink');
        const favoritesLink = document.getElementById('favoritesLink');
        const settingsLink = document.getElementById('settingsLink');
        const logoutLink = document.getElementById('logoutLink');
        const closeLogin = document.getElementById('closeLogin');
        const closeRegister = document.getElementById('closeRegister');
        const switchToRegisterModal = document.getElementById('switchToRegisterModal');
        const switchToLoginModal = document.getElementById('switchToLoginModal');
        const contactForm = document.getElementById('contactForm');
        
        // عرض/إخفاء قائمة المستخدم
        function toggleUserDropdown() {
            if(userDropdown) {
                userDropdown.classList.toggle('show');
            }
        }
        
        if(userBtn) userBtn.addEventListener('click', toggleUserDropdown);
        if(userBtnDesktop) userBtnDesktop.addEventListener('click', toggleUserDropdown);
        
        // إغلاق القائمة عند النقر خارجها
        document.addEventListener('click', function(e) {
            if(userBtn && !userBtn.contains(e.target) && 
               userDropdown && !userDropdown.contains(e.target) && 
               userBtnDesktop && !userBtnDesktop.contains(e.target)) {
                if(userDropdown) userDropdown.classList.remove('show');
            }
        });
        
        // عرض مودال تسجيل الدخول
        if(loginLink) {
            loginLink.addEventListener('click', function(e) {
                e.preventDefault();
                if(loginModal) loginModal.style.display = 'flex';
                if(userDropdown) userDropdown.classList.remove('show');
            });
        }
        
        // عرض مودال التسجيل
        if(registerLink) {
            registerLink.addEventListener('click', function(e) {
                e.preventDefault();
                if(registerModal) registerModal.style.display = 'flex';
                if(userDropdown) userDropdown.classList.remove('show');
            });
        }
        
        // إغلاق المودالات
        if(closeLogin) {
            closeLogin.addEventListener('click', () => {
                if(loginModal) loginModal.style.display = 'none';
            });
        }
        
        if(closeRegister) {
            closeRegister.addEventListener('click', () => {
                if(registerModal) registerModal.style.display = 'none';
            });
        }
        
        window.addEventListener('click', function(e) {
            if(loginModal && e.target === loginModal) loginModal.style.display = 'none';
            if(registerModal && e.target === registerModal) registerModal.style.display = 'none';
        });
        
        // التبديل بين مودالي الدخول والتسجيل
        if(switchToRegisterModal) {
            switchToRegisterModal.addEventListener('click', function(e) {
                e.preventDefault();
                if(loginModal) loginModal.style.display = 'none';
                if(registerModal) registerModal.style.display = 'flex';
            });
        }
        
        if(switchToLoginModal) {
            switchToLoginModal.addEventListener('click', function(e) {
                e.preventDefault();
                if(registerModal) registerModal.style.display = 'none';
                if(loginModal) loginModal.style.display = 'flex';
            });
        }
        
        // محاكاة تسجيل الدخول
        if(document.getElementById('loginForm')) {
            document.getElementById('loginForm').addEventListener('submit', function(e) {
                e.preventDefault();
                
                setTimeout(() => {
                    if(loginModal) loginModal.style.display = 'none';
                    alert('تم تسجيل الدخول بنجاح!');
                    
                    // تحديث واجهة المستخدم
                    if(loginLink) loginLink.style.display = 'none';
                    if(registerLink) registerLink.style.display = 'none';
                    if(dashboardLink) dashboardLink.style.display = 'block';
                    if(bookingsLink) bookingsLink.style.display = 'block';
                    if(favoritesLink) favoritesLink.style.display = 'block';
                    if(settingsLink) settingsLink.style.display = 'block';
                    if(logoutLink) logoutLink.style.display = 'block';
                }, 800);
            });
        }
        
        // محاكاة التسجيل
        if(document.getElementById('registerForm')) {
            document.getElementById('registerForm').addEventListener('submit', function(e) {
                e.preventDefault();
                
                setTimeout(() => {
                    if(registerModal) registerModal.style.display = 'none';
                    alert('تم إنشاء الحساب بنجاح! تم إرسال رسالة تأكيد إلى بريدك الإلكتروني.');
                    
                    // عرض مودال تسجيل الدخول
                    if(loginModal) loginModal.style.display = 'flex';
                }, 1000);
            });
        }
        
        // تسجيل الخروج
        if(logoutLink) {
            logoutLink.addEventListener('click', function(e) {
                e.preventDefault();
                
                if(confirm('هل أنت متأكد من تسجيل الخروج؟')) {
                    // تحديث واجهة المستخدم
                    if(loginLink) loginLink.style.display = 'block';
                    if(registerLink) registerLink.style.display = 'block';
                    if(dashboardLink) dashboardLink.style.display = 'none';
                    if(bookingsLink) bookingsLink.style.display = 'none';
                    if(favoritesLink) favoritesLink.style.display = 'none';
                    if(settingsLink) settingsLink.style.display = 'none';
                    if(logoutLink) logoutLink.style.display = 'none';
                    
                    alert('تم تسجيل الخروج بنجاح');
                }
            });
        }
        
        // ======================
        // القائمة المتنقلة
        // ======================
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const navMenu = document.querySelector('nav ul');
        
        if(mobileMenuBtn && navMenu) {
            mobileMenuBtn.addEventListener('click', () => {
                navMenu.classList.toggle('active');
                mobileMenuBtn.innerHTML = navMenu.classList.contains('active') 
                    ? '<i class="fas fa-times"></i>' 
                    : '<i class="fas fa-bars"></i>';
            });
            
            // إغلاق القائمة عند النقر على رابط
            document.querySelectorAll('nav ul li a').forEach(link => {
                link.addEventListener('click', () => {
                    navMenu.classList.remove('active');
                    mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
                });
            });
        }
        
        // ======================
        // التمرير السلس
        // ======================
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                const href = this.getAttribute('href');
                if(href === '#' || href === '#loginModal' || href === '#registerModal' || href.startsWith('https://') || href.startsWith('mailto:')) {
                    return;
                }
                
                e.preventDefault();
                const targetId = href;
                const targetElement = document.querySelector(targetId);
                
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // ======================
        // الأسئلة الشائعة (الطي/الفرد)
        // ======================
        document.querySelectorAll('.faq-question').forEach(question => {
            question.addEventListener('click', () => {
                const answer = question.nextElementSibling;
                const toggleIcon = question.querySelector('.faq-toggle');
                
                question.classList.toggle('active');
                toggleIcon.classList.toggle('active');
                
                if(answer.classList.contains('show')) {
                    answer.classList.remove('show');
                } else {
                    // إغلاق جميع الإجابات الأخرى
                    document.querySelectorAll('.faq-answer').forEach(ans => {
                        ans.classList.remove('show');
                    });
                    document.querySelectorAll('.faq-question').forEach(q => {
                        q.classList.remove('active');
                    });
                    document.querySelectorAll('.faq-toggle').forEach(t => {
                        t.classList.remove('active');
                    });
                    
                    // فتح الإجابة الحالية
                    answer.classList.add('show');
                    question.classList.add('active');
                    toggleIcon.classList.add('active');
                }
            });
        });
        
        // ======================
        // نموذج الاتصال
        // ======================
        if(contactForm) {
            contactForm.addEventListener('submit', function(e) {
                e.preventDefault();
                alert('تم استلام رسالتك! سيقوم فريق الدعم بالتواصل معك قريباً.');
                contactForm.reset();
            });
        }
        
        // ======================
        // محاكاة العداد التنازلي
        // ======================
        function updateCountdown() {
            const now = new Date();
            const targetDates = [
                new Date(now.getFullYear(), now.getMonth(), now.getDate() + 3, 23, 59, 59),
                new Date(now.getFullYear(), now.getMonth(), now.getDate() + 5, 23, 59, 59),
                new Date(now.getFullYear(), now.getMonth(), now.getDate() + 1, 23, 59, 59)
            ];
            
            targetDates.forEach((targetDate, index) => {
                const diff = targetDate - now;
                
                if(diff > 0) {
                    const days = Math.floor(diff / (1000 * 60 * 60 * 24));
                    const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                    const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
                    
                    const daysEl = document.getElementById(`days${index + 1}`);
                    const hoursEl = document.getElementById(`hours${index + 1}`);
                    const minutesEl = document.getElementById(`minutes${index + 1}`);
                    
                    if(daysEl) daysEl.textContent = days.toString().padStart(2, '0');
                    if(hoursEl) hoursEl.textContent = hours.toString().padStart(2, '0');
                    if(minutesEl) minutesEl.textContent = minutes.toString().padStart(2, '0');
                }
            });
        }
        
        setInterval(updateCountdown, 60000);
        updateCountdown();
    </script>
</body>
</html>
