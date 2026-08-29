# IslamBedirPharmacy
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>صيدلية الدكتور إسلام على بدير</title>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --primary-navy: #0d2240;
            --secondary-navy: #152c4f;
            --accent-green: #2ebd59;
            --accent-yellow: #f5b025;
            --light-bg: #f4f7f6;
            --white: #ffffff;
            --text-dark: #1e293b;
            --text-muted: #64748b;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Cairo', sans-serif;
        }

        body {
            background-color: var(--light-bg);
            color: var(--text-dark);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Navbar */
        .navbar {
            background-color: var(--primary-navy);
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 10px rgba(0,0,0,0.15);
        }

        .logo-container {
            display: flex;
            align-items: center;
            gap: 12px;
            color: var(--white);
        }

        .logo-icon {
            width: 45px;
            height: 45px;
            background: var(--white);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--primary-navy);
            font-size: 22px;
            border: 2px solid var(--accent-green);
        }

        .logo-text h1 {
            font-size: 18px;
            font-weight: 800;
            color: var(--accent-yellow);
            line-height: 1.2;
        }

        .logo-text span {
            font-size: 11px;
            color: var(--accent-green);
            letter-spacing: 1px;
            font-weight: 700;
        }

        .nav-links {
            display: flex;
            gap: 20px;
            list-style: none;
        }

        .nav-links a {
            color: var(--white);
            text-decoration: none;
            font-weight: 600;
            font-size: 15px;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: var(--accent-yellow);
        }

        .btn-call-nav {
            background-color: var(--accent-green);
            color: var(--white);
            padding: 8px 20px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 8px;
            transition: 0.3s;
        }

        .btn-call-nav:hover {
            background-color: #249946;
            transform: translateY(-2px);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary-navy) 0%, var(--secondary-navy) 100%);
            color: var(--white);
            padding: 60px 5% 80px;
            text-align: center;
            position: relative;
        }

        .hero-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(46, 189, 89, 0.15);
            border: 1px solid var(--accent-green);
            color: var(--accent-green);
            padding: 6px 18px;
            border-radius: 30px;
            font-weight: 700;
            margin-bottom: 25px;
        }

        .hero h2 {
            font-size: 38px;
            font-weight: 800;
            color: var(--accent-yellow);
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            color: #cbd5e1;
            margin-bottom: 30px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .btn-whatsapp-hero {
            background-color: var(--accent-green);
            color: var(--white);
            padding: 14px 35px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 700;
            font-size: 18px;
            display: inline-flex;
            align-items: center;
            gap: 10px;
            box-shadow: 0 4px 15px rgba(46, 189, 89, 0.4);
            transition: 0.3s;
        }

        .btn-whatsapp-hero:hover {
            transform: scale(1.05);
            background-color: #249946;
        }

        /* Management Section */
        .management-section {
            background-color: #0b1a30;
            padding: 30px 5%;
            color: var(--white);
            border-bottom: 4px solid var(--accent-green);
        }

        .management-title {
            text-align: center;
            font-size: 20px;
            color: #e2e8f0;
            margin-bottom: 25px;
            font-weight: 700;
        }

        .doctors-grid {
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
        }

        .doctor-card {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            padding: 20px 30px;
            border-radius: 15px;
            text-align: center;
            min-width: 220px;
        }

        .doctor-avatar {
            width: 70px;
            height: 70px;
            background: var(--white);
            color: var(--primary-navy);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 32px;
            margin: 0 auto 12px;
            border: 3px solid var(--accent-green);
        }

        .doctor-card h3 {
            font-size: 17px;
            color: var(--accent-yellow);
        }

        /* Services Section */
        .services-section {
            padding: 70px 5%;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 45px;
        }

        .section-title h2 {
            font-size: 28px;
            color: var(--primary-navy);
            font-weight: 800;
        }

        .section-title div {
            width: 60px;
            height: 4px;
            background: var(--accent-green);
            margin: 8px auto 0;
            border-radius: 2px;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .service-card {
            background: var(--white);
            padding: 30px 20px;
            border-radius: 16px;
            text-align: center;
            box-shadow: 0 5px 20px rgba(0,0,0,0.05);
            border: 1px solid #e2e8f0;
            transition: 0.3s;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            border-color: var(--accent-green);
        }

        .service-icon {
            width: 65px;
            height: 65px;
            background: rgba(46, 189, 89, 0.1);
            color: var(--accent-green);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            margin: 0 auto 18px;
        }

        .service-card h3 {
            font-size: 18px;
            color: var(--primary-navy);
            font-weight: 700;
        }

        /* Contact & Map Section */
        .contact-section {
            background: var(--white);
            padding: 70px 5%;
            border-top: 1px solid #e2e8f0;
        }

        .contact-container {
            max-width: 1100px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .info-item {
            display: flex;
            align-items: flex-start;
            gap: 15px;
        }

        .info-icon {
            width: 45px;
            height: 45px;
            background: var(--primary-navy);
            color: var(--accent-yellow);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 20px;
            flex-shrink: 0;
        }

        .info-text h4 {
            font-size: 16px;
            color: var(--primary-navy);
        }

        .info-text p, .info-text a {
            color: var(--text-muted);
            text-decoration: none;
            font-weight: 600;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }

        .social-btn {
            width: 45px;
            height: 45px;
            border-radius: 50%;
            background: var(--primary-navy);
            color: var(--white);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 20px;
            text-decoration: none;
            transition: 0.3s;
        }

        .social-btn:hover {
            background: var(--accent-green);
            transform: scale(1.1);
        }

        .map-box {
            width: 100%;
            height: 320px;
            border-radius: 16px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .map-box iframe {
            width: 100%;
            height: 100%;
            border: 0;
        }

        /* Footer */
        footer {
            background: var(--primary-navy);
            color: var(--white);
            text-align: center;
            padding: 25px 5%;
            font-size: 14px;
            border-top: 1px solid rgba(255,255,255,0.1);
        }

        /* Floating WhatsApp Button */
        .floating-whatsapp {
            position: fixed;
            bottom: 25px;
            left: 25px;
            background-color: var(--accent-green);
            color: var(--white);
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 32px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            z-index: 9999;
            text-decoration: none;
            transition: 0.3s;
        }

        .floating-whatsapp:hover {
            transform: scale(1.1);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 15px;
            }
            .nav-links {
                gap: 15px;
            }
            .contact-container {
                grid-template-columns: 1fr;
            }
            .hero h2 {
                font-size: 28px;
            }
        }
    </style>
</head>
<body>

    <a href="https://wa.me/201006033627?text=السلام%20علكم،%20أستفسر%20عن%20روشتة/دواء" class="floating-whatsapp" target="_blank" title="تواصل عبر الواتساب">
        <i class="fa-brands fa-whatsapp"></i>
    </a>

    <nav class="navbar">
        <div class="logo-container">
            <div class="logo-icon">
                <i class="fa-solid fa-prescription-bottle-medical"></i>
            </div>
            <div class="logo-text">
                <h1>صيدلية د/ إسلام بدير</h1>
                <span>ISLAM ALI BADIR PHARMACY</span>
            </div>
        </div>

        <ul class="nav-links">
            <li><a href="#hero">الرئيسية</a></li>
            <li><a href="#services">خدماتنا</a></li>
            <li><a href="#contact">اتصل بنا</a></li>
        </ul>

        <a href="tel:01006033627" class="btn-call-nav">
            <i class="fa-solid fa-phone"></i> اتصل الآن
        </a>
    </nav>

    <section class="hero" id="hero">
        <div class="hero-badge">
            <i class="fa-solid fa-clock"></i> خدمة 24 ساعة طول الأسبوع
        </div>
        <h2>صيدلية الدكتور إسلام على بدير</h2>
        <p>رعايتكم هي أولويتنا.. خدمات طبية متكاملة على مدار الساعة واستشارات صيدلانية متخصصة.</p>
        
        <a href="https://wa.me/201006033627?text=السلام%20علكم،%20أريد%20إرسال%20الروشتة" class="btn-whatsapp-hero" target="_blank">
            <i class="fa-brands fa-whatsapp"></i> اطلب الروشتة عبر الواتساب
        </a>
    </section>

    <section class="management-section">
        <div class="management-title">تحت إدارة النخبة</div>
        <div class="doctors-grid">
            <div class="doctor-card">
                <div class="doctor-avatar">
                    <i class="fa-solid fa-user-doctor"></i>
                </div>
                <h3>د/ أحمد إيهاب القصبي</h3>
            </div>
            <div class="doctor-card">
                <div class="doctor-avatar">
                    <i class="fa-solid fa-user-doctor"></i>
                </div>
                <h3>د/ محمد حازم القصبي</h3>
            </div>
        </div>
    </section>

    <section class="services-section" id="services">
        <div class="section-title">
            <h2>خدماتنا المتميزة</h2>
            <div></div>
        </div>

        <div class="services-grid">
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-motorcycle"></i></div>
                <h3>خدمة التوصيل المجاني داخل شربين</h3>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-heart-pulse"></i></div>
                <h3>قياس السكر والضغط وقياس InBody</h3>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-user-nurse"></i></div>
                <h3>استشارات صيدلانية متخصصة</h3>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-file-medical"></i></div>
                <h3>تجهيز الروشتات بدقة</h3>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-pills"></i></div>
                <h3>توفر جميع نواقص السوق</h3>
            </div>
            <div class="service-card">
                <div class="service-icon"><i class="fa-solid fa-notes-medical"></i></div>
                <h3>متابعة الحالات المزمنة</h3>
            </div>
        </div>
    </section>

    <section class="contact-section" id="contact">
        <div class="section-title">
            <h2>تواصل معنا</h2>
            <div></div>
        </div>

        <div class="contact-container">
            <div class="contact-info">
                <div class="info-item">
                    <div class="info-icon"><i class="fa-solid fa-location-dot"></i></div>
                    <div class="info-text">
                        <h4>العنوان</h4>
                        <p>شربين - شارع الثانوية بنات - بجوار مقلة هجرس</p>
                    </div>
                </div>

                <div class="info-item">
                    <div class="info-icon"><i class="fa-solid fa-phone-volume"></i></div>
                    <div class="info-text">
                        <h4>الهاتف / الواتساب</h4>
                        <p><a href="tel:01006033627">01006033627</a></p>
                    </div>
                </div>

                <div class="info-item">
                    <div class="info-icon"><i class="fa-solid fa-share-nodes"></i></div>
                    <div class="info-text">
                        <h4>صفحاتنا على التواصل الاجتماعي</h4>
                        <div class="social-links">
                            <a href="https://www.facebook.com/share/1Ghp3WgPwN/" class="social-btn" target="_blank" title="فيسبوك"><i class="fa-brands fa-facebook-f"></i></a>
                            <a href="https://www.instagram.com/islambdiarpharmacy?igsi=YjBnZTAxYWtocnI=" class="social-btn" target="_blank" title="انستجرام"><i class="fa-brands fa-instagram"></i></a>
                            <a href="https://wa.me/201006033627" class="social-btn" target="_blank" title="واتساب"><i class="fa-brands fa-whatsapp"></i></a>
                        </div>
                    </div>
                </div>
            </div>

            <div class="map-box">
                <iframe 
                    src="https://maps.google.com/maps?q=Sherbin%20Dakahlia&t=&z=15&ie=UTF8&iwloc=&output=embed" 
                    allowfullscreen="" 
                    loading="lazy">
                </iframe>
            </div>
        </div>
    </section>

    <footer>
        <p>© جميع الحقوق محفوظة - صيدلية الدكتور إسلام على بدير 2026</p>
    </footer>

</body>
</html>
