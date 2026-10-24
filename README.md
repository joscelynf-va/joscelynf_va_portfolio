<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Joscelyn Flores | JF Virtual Assistant & Operations</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Playfair+Display:ital,wght@0,600;0,700;1,600&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-main: #FAFAF8;
            --bg-card: #FFFFFF;
            --primary-dark: #0F2C2C;       /* Deep Teal Slate */
            --teal-bright: #00A896;       /* Electric Vibrant Teal */
            --teal-soft: #E0F2F1;         /* Pale Teal Tint */
            --orange-bright: #FF6B35;     /* Vibrant Warm Orange */
            --orange-soft: #FFF3ED;       /* Pale Orange Tint */
            --text-dark: #1E292B;
            --text-muted: #526062;
            --border-light: #E2ECE9;
            --radius-sm: 10px;
            --radius-md: 18px;
            --radius-lg: 28px;
            --shadow-soft: 0 12px 32px rgba(0, 168, 150, 0.08);
            --shadow-hover: 0 18px 40px rgba(255, 107, 53, 0.15);
            /* Chic Cheetah Pattern Data URI */
            --cheetah-pattern: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='60' height='60' viewBox='0 0 60 60'%3E%3Cpath d='M12 10c2-3 6-3 8 0s1 7-2 8-7-1-6-8zM38 15c3-2 7 0 7 4s-3 6-6 4-3-6-1-8zM22 35c3-1 6 2 5 5s-5 4-7 1 0-5 2-6zM45 40c2-3 6-2 7 1s-2 6-5 5-3-4-2-6zM10 48c2-1 4 1 4 3s-3 4-5 2 0-4 1-5z' fill='%230F2C2C' fill-opacity='0.18'/%3E%3Cpath d='M15 13c1-1 3-1 4 0s0 3-1 4-3 0-3-1 0-2 0-3zM40 17c1-1 3 0 3 2s-1 3-3 2-1-3 0-4zM24 37c1 0 3 1 2 3s-2 2-3 1 0-3 1-4z' fill='%23FF6B35' fill-opacity='0.35'/%3E%3C/svg%3E");
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-main);
            color: var(--text-dark);
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        /* Cheetah Accent Strip */
        .cheetah-border-strip {
            height: 6px;
            background-color: var(--orange-soft);
            background-image: var(--cheetah-pattern);
            background-size: 40px 40px;
            width: 100%;
        }

        /* Top Banner */
        .announcement-banner {
            background-color: var(--primary-dark);
            color: #FFFFFF;
            text-align: center;
            padding: 10px 20px;
            font-size: 0.875rem;
            font-weight: 600;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }

        .pulse-badge {
            display: inline-block;
            width: 9px;
            height: 9px;
            background-color: var(--orange-bright);
            border-radius: 50%;
            box-shadow: 0 0 0 0 rgba(255, 107, 53, 0.7);
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(255, 107, 53, 0.7); }
            70% { transform: scale(1); box-shadow: 0 0 0 8px rgba(255, 107, 53, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(255, 107, 53, 0); }
        }

        /* Header */
        header {
            position: sticky;
            top: 0;
            background: rgba(250, 250, 248, 0.92);
            backdrop-filter: blur(14px);
            z-index: 1000;
            border-bottom: 1px solid var(--border-light);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 16px 24px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.6rem;
            font-weight: 700;
            color: var(--primary-dark);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .logo-badge {
            background: var(--teal-soft);
            color: var(--teal-bright);
            border: 1px solid var(--teal-bright);
            padding: 2px 8px;
            border-radius: 6px;
            font-size: 0.75rem;
            font-family: 'Plus Jakarta Sans', sans-serif;
            font-weight: 800;
        }

        .logo span {
            color: var(--orange-bright);
        }

        .nav-links {
            display: flex;
            gap: 32px;
            list-style: none;
            align-items: center;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-dark);
            font-weight: 600;
            font-size: 0.95rem;
            transition: color 0.2s ease;
        }

        .nav-links a:hover {
            color: var(--orange-bright);
        }

        .btn-primary {
            background-color: var(--orange-bright);
            color: #FFFFFF;
            padding: 12px 26px;
            border-radius: var(--radius-sm);
            text-decoration: none;
            font-weight: 700;
            font-size: 0.95rem;
            display: inline-block;
            transition: all 0.25s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 4px 14px rgba(255, 107, 53, 0.3);
        }

        .btn-primary:hover {
            background-color: #E85D04;
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(255, 107, 53, 0.4);
        }

        .btn-teal {
            background-color: var(--teal-bright);
            color: #FFFFFF;
            padding: 12px 26px;
            border-radius: var(--radius-sm);
            text-decoration: none;
            font-weight: 700;
            font-size: 0.95rem;
            display: inline-block;
            transition: all 0.25s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 4px 14px rgba(0, 168, 150, 0.3);
        }

        .btn-teal:hover {
            background-color: #00897B;
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(0, 168, 150, 0.4);
        }

        /* Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 60px 24px;
        }

        /* Hero */
        .hero {
            display: grid;
            grid-template-columns: 1.2fr 0.8fr;
            gap: 48px;
            align-items: center;
            padding: 30px 0 70px 0;
        }

        .hero-tag {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: var(--teal-soft);
            color: var(--teal-bright);
            padding: 6px 16px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 700;
            margin-bottom: 20px;
            border: 1px solid rgba(0, 168, 150, 0.2);
        }

        .hero-title {
            font-family: 'Playfair Display', serif;
            font-size: 3.3rem;
            line-height: 1.15;
            color: var(--primary-dark);
            margin-bottom: 24px;
        }

        .hero-title span {
            color: var(--orange-bright);
            position: relative;
        }

        .hero-subtitle {
            font-size: 1.15rem;
            color: var(--text-muted);
            margin-bottom: 32px;
            max-width: 580px;
        }

        /* Cheetah Highlight Box */
        .cheetah-card-frame {
            position: relative;
            background-color: var(--orange-soft);
            background-image: var(--cheetah-pattern);
            background-size: 50px 50px;
            padding: 12px;
            border-radius: var(--radius-lg);
            box-shadow: var(--shadow-soft);
        }

        .counter-card {
            background-color: #FFFFFF;
            border: 1px solid var(--border-light);
            border-radius: calc(var(--radius-lg) - 6px);
            padding: 32px;
            display: flex;
            flex-direction: column;
            gap: 16px;
        }

        .counter-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-size: 0.85rem;
            font-weight: 800;
            letter-spacing: 0.5px;
            color: var(--text-muted);
        }

        .counter-number {
            font-size: 3rem;
            font-weight: 800;
            color: var(--teal-bright);
        }

        .progress-bar {
            height: 10px;
            background-color: var(--teal-soft);
            border-radius: 5px;
            overflow: hidden;
        }

        .progress-fill {
            height: 100%;
            width: 100%;
            background: linear-gradient(90deg, var(--teal-bright), var(--orange-bright));
            transition: width 0.3s ease;
        }

        .badge-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 10px;
        }

        .pill-badge {
            background-color: var(--teal-soft);
            color: var(--primary-dark);
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 700;
            border: 1px solid rgba(0, 168, 150, 0.2);
        }

        .pill-badge.orange-pill {
            background-color: var(--orange-soft);
            color: var(--orange-bright);
            border-color: rgba(255, 107, 53, 0.2);
        }

        /* Section Headings */
        .section-header {
            text-align: center;
            max-width: 680px;
            margin: 0 auto 50px auto;
        }

        .section-header h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: var(--primary-dark);
            margin-bottom: 12px;
        }

        .section-header p {
            color: var(--text-muted);
            font-size: 1.05rem;
        }

        /* Services Grid */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 28px;
        }

        .service-card {
            background: var(--bg-card);
            border: 1px solid var(--border-light);
            border-radius: var(--radius-md);
            padding: 32px;
            box-shadow: var(--shadow-soft);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .service-card::top {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--teal-bright);
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-hover);
            border-color: var(--orange-bright);
        }

        .service-card h3 {
            font-size: 1.3rem;
            color: var(--primary-dark);
            margin-bottom: 12px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .service-card p {
            color: var(--text-muted);
            font-size: 0.95rem;
            margin-bottom: 16px;
        }

        /* Packages Section */
        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 28px;
            align-items: stretch;
        }

        .pricing-card {
            background: var(--bg-card);
            border: 1px solid var(--border-light);
            border-radius: var(--radius-lg);
            padding: 36px;
            position: relative;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            box-shadow: var(--shadow-soft);
        }

        .pricing-card.featured {
            border: 2px solid var(--orange-bright);
            box-shadow: var(--shadow-hover);
        }

        .featured-badge {
            position: absolute;
            top: -14px;
            right: 28px;
            background: var(--orange-bright);
            color: #FFFFFF;
            font-size: 0.75rem;
            font-weight: 800;
            text-transform: uppercase;
            padding: 6px 14px;
            border-radius: 14px;
            letter-spacing: 0.5px;
        }

        .price {
            font-size: 2.6rem;
            font-weight: 800;
            color: var(--primary-dark);
            margin: 16px 0 8px 0;
        }

        .price span {
            font-size: 1rem;
            font-weight: 500;
            color: var(--text-muted);
        }

        .feature-list {
            list-style: none;
            margin: 24px 0 32px 0;
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .feature-list li {
            font-size: 0.95rem;
            color: var(--text-dark);
            display: flex;
            align-items: flex-start;
            gap: 10px;
        }

        .feature-list li::before {
            content: "✦";
            color: var(--orange-bright);
            font-weight: bold;
        }

        /* Asynchronous Boundaries Banner */
        .boundaries-box {
            background-color: var(--primary-dark);
            color: #FFFFFF;
            padding: 48px;
            border-radius: var(--radius-lg);
            position: relative;
            overflow: hidden;
        }

        .boundaries-box h3 {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            color: var(--orange-soft);
            margin-bottom: 24px;
        }

        .boundaries-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 24px;
        }

        .boundary-item h4 {
            color: var(--teal-bright);
            font-size: 1.1rem;
            margin-bottom: 8px;
        }

        .boundary-item p {
            color: #D1E0DE;
            font-size: 0.9rem;
        }

        /* Form Section */
        .form-section {
            background-color: var(--bg-card);
            border: 1px solid var(--border-light);
            border-radius: var(--radius-lg);
            padding: 48px;
            max-width: 820px;
            margin: 0 auto;
            box-shadow: var(--shadow-soft);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            font-size: 0.9rem;
            font-weight: 700;
            color: var(--primary-dark);
            margin-bottom: 8px;
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 14px 18px;
            border: 1px solid var(--border-light);
            border-radius: var(--radius-sm);
            font-family: inherit;
            font-size: 0.95rem;
            color: var(--text-dark);
            background-color: var(--bg-main);
            transition: border-color 0.2s ease;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--teal-bright);
            box-shadow: 0 0 0 3px rgba(0, 168, 150, 0.15);
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        /* Accordion / Hosting Guide */
        .accordion {
            background: var(--bg-card);
            border: 1px solid var(--border-light);
            border-radius: var(--radius-md);
            overflow: hidden;
            max-width: 820px;
            margin: 0 auto;
        }

        .accordion-header {
            padding: 20px 24px;
            background: #FFFFFF;
            cursor: pointer;
            font-weight: 700;
            color: var(--primary-dark);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .accordion-content {
            padding: 24px;
            display: none;
            border-top: 1px solid var(--border-light);
            background: var(--bg-main);
            font-size: 0.95rem;
        }

        .accordion-content.open {
            display: block;
        }

        /* Footer */
        footer {
            background-color: var(--primary-dark);
            color: #FFFFFF;
            padding: 50px 24px 30px 24px;
            text-align: center;
            font-size: 0.9rem;
            margin-top: 80px;
        }

        footer a {
            color: var(--orange-bright);
            text-decoration: none;
            font-weight: 600;
        }

        @media (max-width: 768px) {
            .hero { grid-template-columns: 1fr; text-align: center; }
            .hero-subtitle { margin: 0 auto 32px auto; }
            .form-row { grid-template-columns: 1fr; }
            .nav-links { display: none; }
            .boundaries-box { padding: 28px; }
        }
    </style>
</head>
<body>

    <!-- Cheetah Pattern Top Border -->
    <div class="cheetah-border-strip"></div>

    <!-- Announcement Banner -->
    <div class="announcement-banner">
        <span class="pulse-badge"></span>
        Accepting 5 Retainer Clients for Q4 | Deliverable-Driven & Asynchronous Support
    </div>

    <!-- Navigation -->
    <header>
        <div class="nav-container">
            <a href="#" class="logo">
                JF <span class="logo-badge">VA</span> <span>Virtual Assistant</span>
            </a>
            <ul class="nav-links">
                <li><a href="#services">Services</a></li>
                <li><a href="#packages">Packages</a></li>
                <li><a href="#boundaries">Boundaries</a></li>
                <li><a href="#about">About</a></li>
            </ul>
            <a href="#inquire" class="btn-primary">Inquire Now</a>
        </div>
    </header>

    <!-- Main Content -->
    <main>
        <!-- Hero Section -->
        <section class="container hero">
            <div>
                <span class="hero-tag">✨ Marketing & Systems Strategist</span>
                <h1 class="hero-title">High-Impact Operations & <span>Creative Growth</span> for Business Owners</h1>
                <p class="hero-subtitle">
                    Streamline your back-office, CRM, and marketing execution with an outcome-driven Virtual Assistant. Vibrant storytelling and seamless organization delivered asynchronously.
                </p>
                <div class="badge-grid">
                    <span class="pill-badge">B.S. Marketing</span>
                    <span class="pill-badge orange-pill">UGC & Social Creator</span>
                    <span class="pill-badge">Google Certified</span>
                    <span class="pill-badge orange-pill">Salesforce & CRM Proficient</span>
                    <span class="pill-badge">Bilingual (EN/ES)</span>
                </div>
            </div>

            <div class="cheetah-card-frame">
                <div class="counter-card">
                    <div class="counter-header">
                        <span>Q4 CLIENT CAPACITY</span>
                        <span style="color: var(--teal-bright);">● 5 SPOTS OPEN</span>
                    </div>
                    <div class="counter-number" id="spotCounterDisplay">5 / 5</div>
                    <div class="progress-bar">
                        <div class="progress-fill" id="spotProgressFill"></div>
                    </div>
                    <p style="font-size: 0.85rem; color: var(--text-muted);">
                        All 5 client retainer spots are currently available for this quarter.
                    </p>
                </div>
            </div>
        </section>

        <!-- Services Section -->
        <section id="services" class="container">
            <div class="section-header">
                <h2>Specialized Core Services</h2>
                <p>Merging administrative precision, CRM proficiency, and vibrant visual content creation.</p>
            </div>

            <div class="services-grid">
                <div class="service-card">
                    <h3>📱 Social Media & UGC Content</h3>
                    <p>Monthly content calendar strategy, custom Canva graphic design, and engaging short-form UGC video creation (Reels/TikToks) aligned with your brand voice.</p>
                </div>
                <div class="service-card">
                    <h3>📊 CRM & Database Hygiene</h3>
                    <p>Contact list segmentation, lead workflow tagging, data audits, and record hygiene in Salesforce, HubSpot, or custom CRM systems.</p>
                </div>
                <div class="service-card">
                    <h3>✉️ Executive Inbox & Calendar</h3>
                    <p>High-volume email triage, appointment scheduling, meeting coordination, and professional client correspondence.</p>
                </div>
                <div class="service-card">
                    <h3>🎯 Project & Event Logistics</h3>
                    <p>Cross-functional coordination, marketing outreach support, partner communications, and event execution logistics.</p>
                </div>
                <div class="service-card">
                    <h3>🤝 Customer Relationship Care</h3>
                    <p>Onboarding workflows, client follow-up protocols, feedback collection, and multi-channel customer relationship management.</p>
                </div>
            </div>
        </section>

        <!-- Packages Section -->
        <section id="packages" class="container">
            <div class="section-header">
                <h2>Monthly Retainer Packages</h2>
                <p>Flat-rate monthly subscriptions focused on deliverables and outcomes—no hourly tracking required.</p>
            </div>

            <div class="pricing-grid">
                <!-- Tier 1 -->
                <div class="pricing-card">
                    <div>
                        <h3>Operations Foundations</h3>
                        <div class="price">$850 <span>/ month</span></div>
                        <p style="font-size: 0.9rem; color: var(--text-muted);">Essential back-office & admin hygiene</p>
                        <ul class="feature-list">
                            <li>Inbox & Calendar Triage</li>
                            <li>CRM Entry & Record Audit</li>
                            <li>Standard SOP Documentation</li>
                            <li>Weekly Friday Progress Digest</li>
                        </ul>
                    </div>
                    <button class="btn-teal" onclick="selectPackage('Tier 1 - Operations Foundations ($850/mo)')">Select Tier 1</button>
                </div>

                <!-- Tier 2 (Featured) -->
                <div class="pricing-card featured">
                    <span class="featured-badge">Most Popular</span>
                    <div>
                        <h3>Growth & Marketing</h3>
                        <div class="price">$2,000 <span>/ month</span></div>
                        <p style="font-size: 0.9rem; color: var(--text-muted);">Full content execution & admin support</p>
                        <ul class="feature-list">
                            <li>All Tier 1 Foundations Included</li>
                            <li>3–4 Social Posts/Week (2 Platforms)</li>
                            <li>4 Custom UGC Short-Form Videos</li>
                            <li>Monthly Analytics & Engagement Report</li>
                        </ul>
                    </div>
                    <button class="btn-primary" onclick="selectPackage('Tier 2 - Growth & Marketing ($2,000/mo)')">Select Tier 2</button>
                </div>

                <!-- Tier 3 -->
                <div class="pricing-card">
                    <div>
                        <h3>VIP Marketing & Ops</h3>
                        <div class="price">$3,500 <span>/ month</span></div>
                        <p style="font-size: 0.9rem; color: var(--text-muted);">Turnkey strategy & operations management</p>
                        <ul class="feature-list">
                            <li>All Tier 1 & Tier 2 Deliverables</li>
                            <li>Advanced CRM Workflows & Tagging</li>
                            <li>8 Custom UGC Video Assets/Month</li>
                            <li>Dedicated 60-Min Monthly Strategy Call</li>
                        </ul>
                    </div>
                    <button class="btn-teal" onclick="selectPackage('Tier 3 - VIP Marketing & Ops ($3,500/mo)')">Select Tier 3</button>
                </div>
            </div>
        </section>

        <!-- Asynchronous Boundaries Box -->
        <section id="boundaries" class="container">
            <div class="boundaries-box">
                <h3>Working Boundaries & Delivery Model</h3>
                <div class="boundaries-grid">
                    <div class="boundary-item">
                        <h4>Asynchronous First</h4>
                        <p>Primary communication takes place via email and shared project portals (Notion/Asana) to maximize focused execution.</p>
                    </div>
                    <div class="boundary-item">
                        <h4>24-Hour Response SLA</h4>
                        <p>Non-urgent communications received during standard business hours (Mon–Fri, 9–5 EST) receive a reply within 24 business hours.</p>
                    </div>
                    <div class="boundary-item">
                        <h4>Friday Updates</h4>
                        <p>Receive a weekly status report every Friday detailing completed tasks, open items, and upcoming priorities.</p>
                    </div>
                    <div class="boundary-item">
                        <h4>Outcome-Driven</h4>
                        <p>Work is measured by completed deliverables and agreed quality metrics rather than arbitrary logged hours.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Inquiry Form -->
        <section id="inquire" class="container">
            <div class="form-section">
                <div class="section-header" style="margin-bottom: 32px;">
                    <h2>Client Inquiry Form</h2>
                    <p>Submit your project details below to reserve one of the 5 Q4 retainer spots. Submissions route directly to <strong>contact.jfva@gmail.com</strong>.</p>
                </div>

                <form id="clientInquiryForm">
                    <div class="form-row">
                        <div class="form-group">
                            <label for="fullName">Full Name *</label>
                            <input type="text" id="fullName" required placeholder="Jane Doe">
                        </div>
                        <div class="form-group">
                            <label for="email">Email Address *</label>
                            <input type="email" id="email" required placeholder="jane@company.com">
                        </div>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label for="businessName">Business Name / Website</label>
                            <input type="text" id="businessName" placeholder="Acme Consulting">
                        </div>
                        <div class="form-group">
                            <label for="packageSelect">Preferred Service Tier *</label>
                            <select id="packageSelect" required>
                                <option value="">Select a package tier...</option>
                                <option value="Tier 1 - Operations Foundations ($850/mo)">Tier 1 - Operations Foundations ($850/mo)</option>
                                <option value="Tier 2 - Growth & Marketing ($2,000/mo)">Tier 2 - Growth & Marketing ($2,000/mo)</option>
                                <option value="Tier 3 - VIP Marketing & Ops ($3,500/mo)">Tier 3 - VIP Marketing & Ops ($3,500/mo)</option>
                            </select>
                        </div>
                    </div>

                    <div class="form-group">
                        <label for="asyncTool">Preferred Asynchronous Tool</label>
                        <select id="asyncTool">
                            <option value="Email & Google Drive">Email & Google Drive</option>
                            <option value="Notion Dashboard">Notion Dashboard</option>
                            <option value="Asana / Trello">Asana / Trello</option>
                        </select>
                    </div>

                    <div class="form-group">
                        <label for="goals">Primary Business Goals & Deliverable Needs *</label>
                        <textarea id="goals" rows="4" required placeholder="Describe your top 2-3 immediate priorities or back-office bottlenecks..."></textarea>
                    </div>

                    <button type="submit" class="btn-primary" style="width: 100%; padding: 16px; font-size: 1.05rem;">Submit Inquiry to contact.jfva@gmail.com</button>
                </form>

                <div id="formSuccessMessage" style="display: none; text-align: center; padding: 24px; background: #E0F2F1; border-radius: var(--radius-sm); color: #004D40; margin-top: 20px;">
                    <h3>Inquiry Received!</h3>
                    <p style="margin-top: 8px;">Thank you for your interest. A confirmation copy has been routed to <strong>contact.jfva@gmail.com</strong>. You will receive a response within 24 business hours.</p>
                </div>
            </div>
        </section>
    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Joscelyn Flores — JF Virtual Assistant. All rights reserved.</p>
        <p style="margin-top: 8px;">Direct Contact: <a href="mailto:contact.jfva@gmail.com">contact.jfva@gmail.com</a></p>
    </footer>

    <!-- Bottom Cheetah Accent Strip -->
    <div class="cheetah-border-strip"></div>

    <script>
        // State for Client Counter (Starts at 5 available)
        let availableSpots = 5;
        const totalSpots = 5;

        function updateCounterUI() {
            const display = document.getElementById('spotCounterDisplay');
            const fill = document.getElementById('spotProgressFill');
            
            display.innerText = `${availableSpots} / ${totalSpots}`;
            const percentage = (availableSpots / totalSpots) * 100;
            fill.style.width = `${percentage}%`;
        }

        // Initialize UI
        updateCounterUI();

        // Scroll and Pre-select Package
        function selectPackage(packageName) {
            const packageDropdown = document.getElementById('packageSelect');
            packageDropdown.value = packageName;
            document.getElementById('inquire').scrollIntoView({ behavior: 'smooth' });
        }

        // Form Submission Handling
        document.getElementById('clientInquiryForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const name = document.getElementById('fullName').value;
            const email = document.getElementById('email').value;
            const packageChoice = document.getElementById('packageSelect').value;

            // Decrement spot counter on successful inquiry simulation
            if (availableSpots > 0) {
                availableSpots -= 1;
                updateCounterUI();
            }

            // Hide form and show success confirmation
            document.getElementById('clientInquiryForm').style.display = 'none';
            const successBox = document.getElementById('formSuccessMessage');
            successBox.style.display = 'block';
            
            // Construct mailto link as direct fallback
            const subject = encodeURIComponent(`New Inquiry from ${name} - ${packageChoice}`);
            const body = encodeURIComponent(`Client Name: ${name}\nEmail: ${email}\nPackage: ${packageChoice}\n\nForm submitted via jfva website.`);
            
            // Trigger mailto window for client inquiry
            window.location.href = `mailto:contact.jfva@gmail.com?subject=${subject}&body=${body}`;
        });

        // Toggle Accordion Guide
        function toggleAccordion() {
            const content = document.getElementById('accordionContent');
            content.classList.toggle('open');
        }
    </script>
</body>
</html>
