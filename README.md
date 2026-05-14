<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Almetric Technologies | AL Buds 1 Campaign</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --accent: #2ECC71; 
            --bg: #0a0a0a;
            --card-bg: #151515;
            --text: #ffffff;
            --text-dim: #888;
            --locked: #333;
        }

        /* Smooth Scrolling */
        html { scroll-behavior: smooth; }

        body {
            margin: 0;
            font-family: 'Inter', sans-serif;
            background-color: var(--bg);
            color: var(--text);
            line-height: 1.6;
        }

        /* --- HERO SECTION --- */
        .hero {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle at center, #1a1a1a 0%, #0a0a0a 100%);
            padding: 40px 20px;
        }

        h1 {
            font-size: clamp(2.5rem, 8vw, 4rem);
            margin: 0;
            letter-spacing: -2px;
            background: linear-gradient(to bottom, #fff 40%, #888 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .product-tagline {
            font-size: 1rem;
            font-weight: 300;
            color: var(--accent);
            text-transform: uppercase;
            letter-spacing: 5px;
            margin-bottom: 20px;
        }

        /* --- PROGRESS BAR --- */
        .campaign-status {
            width: 100%;
            max-width: 600px;
            margin: 20px auto;
            text-align: left;
        }

        .progress-container {
            width: 100%;
            height: 12px;
            background: #222;
            border-radius: 20px;
            margin: 10px 0;
            overflow: hidden;
        }

        .progress-bar {
            width: 80%; /* $32,000 of $40,000 HKD */
            height: 100%;
            background: var(--accent);
            box-shadow: 0 0 15px rgba(46, 204, 113, 0.4);
        }

        .stats {
            display: flex;
            justify-content: space-between;
            font-size: 0.8rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            color: var(--text-dim);
        }

        .stats span { color: var(--text); font-weight: 700; }

        .cta-group {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            margin-top: 30px;
        }

        .btn {
            display: inline-block;
            padding: 15px 35px;
            border-radius: 2px;
            text-decoration: none;
            font-weight: 700;
            transition: all 0.3s ease;
            text-transform: uppercase;
            font-size: 0.75rem;
            letter-spacing: 2px;
            text-align: center;
            cursor: pointer;
            border: none;
        }

        .btn-primary { background: var(--accent); color: #000; }
        .btn-outline { border: 1px solid var(--accent); color: var(--accent); }
        .btn:hover { transform: translateY(-3px); box-shadow: 0 10px 20px rgba(46, 204, 113, 0.1); }

        /* --- GENERAL SECTIONS --- */
        .section-padding { padding: 100px 20px; max-width: 1000px; margin: 0 auto; }
        h2 { font-size: 2.5rem; letter-spacing: -1px; text-align: center; margin-bottom: 20px; }
        .section-intro { text-align: center; color: var(--text-dim); max-width: 700px; margin: 0 auto 50px auto; }

        /* --- LEARN MORE SECTION --- */
        .img-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 30px; margin: 50px 0; }
        .img-card { background: var(--card-bg); padding: 15px; border: 1px solid #222; border-radius: 4px; }
        .img-card img { width: 100%; border-radius: 2px; filter: grayscale(20%); }
        .card-label { display: block; margin-top: 15px; font-weight: 700; color: var(--accent); font-size: 0.7rem; text-transform: uppercase; }

        /* --- TIERS SECTION --- */
        .tier-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 25px; }
        .tier-card {
            background: var(--card-bg);
            border: 1px solid #222;
            padding: 40px 30px;
            border-radius: 4px;
            display: flex;
            flex-direction: column;
            transition: border-color 0.3s ease;
        }
        .tier-card:hover { border-color: var(--accent); }
        .tier-name { color: var(--accent); text-transform: uppercase; letter-spacing: 2px; font-size: 0.75rem; font-weight: 700; }
        .tier-price { font-size: 2rem; margin: 10px 0; font-weight: 700; }
        .tier-price span { font-size: 1rem; color: var(--text-dim); }
        .tier-desc { font-size: 0.9rem; color: var(--text-dim); flex-grow: 1; margin-bottom: 30px; }

        /* --- STRETCH GOALS SECTION --- */
        .stretch-container { display: flex; flex-direction: column; gap: 20px; }
        .stretch-card { background: #0d0d0d; border: 1px solid var(--locked); padding: 30px; border-radius: 4px; opacity: 0.7; }
        .stretch-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 15px; }
        .stretch-amount { background: var(--locked); color: #fff; padding: 5px 15px; font-size: 0.8rem; font-weight: 700; border-radius: 20px; }

        footer { padding: 80px 20px; text-align: center; color: #444; font-size: 0.7rem; text-transform: uppercase; letter-spacing: 2px; border-top: 1px solid #111; }

        @media (max-width: 768px) { .img-grid { grid-template-columns: 1fr; } }
    </style>
</head>
<body>

    <!-- Hero Section -->
    <section class="hero">
        <div class="product-tagline">Almetric Technologies</div>
        <h1>AL Buds 1</h1>
        <p style="max-width: 500px; color: var(--text-dim); margin-bottom: 30px;">Crowdfunding the AL Buds 1: Clinical-grade biometric monitoring meets professional audio ergonomics.</p>
        
        <!-- Progress Tracker -->
        <div class="campaign-status">
            <div class="stats">
                <div>Raised: <span>$32,000 HKD</span></div>
                <div>Goal: <span>$40,000 HKD</span></div>
            </div>
            <div class="progress-container">
                <div class="progress-bar"></div>
            </div>
            <div class="stats" style="margin-top: 5px;">
                <div style="font-size: 0.65rem;">67% Funded</div>
                <div style="font-size: 0.65rem;">14 Days Remaining</div>
            </div>
        </div>

        <div class="cta-group">
            <a href="#tiers" class="btn btn-primary">Back This Campaign</a>
            <a href="#learn-more" class="btn btn-outline">Learn More</a>
            <a href="#stretch-goals" class="btn btn-outline">Stretch Goals</a>
        </div>
    </section>

    <!-- Learn More Section -->
    <section id="learn-more" class="section-padding" style="border-top: 1px solid #111;">
        <h2>The Technology</h2>
        <p class="section-intro">Almetric Technologies is redefining personal health. By utilizing the ear's unique vascularity, AL Buds 1 provide clinical-grade data that wrist-worn wearables simply cannot reach.</p>
        
        <div class="img-grid">
            <div class="img-card">
                <img src="sketch.png" alt="Vision Sketch">
                <span class="card-label">Design Vision</span>
                <p style="font-size: 0.85rem; color: var(--text-dim);">The original sketch that kickstarted all of this.</p>
            </div>
            <div class="img-card">
                <img src="prototype.png" alt="Current Prototype">
                <span class="card-label">Final Prototype</span>
                <p style="font-size: 0.85rem; color: var(--text-dim);">Our current prototype, closer to perfection than ever.</p>
            </div>
        </div>

        <p style="text-align: center; max-width: 800px; margin: 0 auto; color: var(--text-dim);">Our design incorporates a discreet, weighted battery pack positioned comfortably behind the ear, ensuring perfect balance for all-day monitoring and high-fidelity listening.</p>
    </section>

    <!-- Tiers Section -->
    <section id="tiers" class="section-padding" style="background: #0d0d0d;">
        <h2>Backing Tiers</h2>
        <p class="section-intro">Support the development of the technology of tomorrow.</p>

        <div class="tier-grid">
            <div class="tier-card">
                <div class="tier-name">Basic Plan</div>
                <div class="tier-price">120 <span>HKD</span></div>
                <p class="tier-desc">Support the technology of tomorrow. Backers of the Basic Tier will receive 1 keychain as a small thank you from the Almetric Team.</p>
                <a href="#" class="btn btn-outline">Pledge 120 HKD</a>
            </div>

            <div class="tier-card" style="border-color: var(--accent); transform: scale(1.02); background: #1a1a1a;">
                <div class="tier-name">Premium Plan</div>
                <div class="tier-price">1,600 <span>HKD</span></div>
                <p class="tier-desc">Support tomorrow's technology today. Receive the AL Buds 1 once polished to perfection as a big thank you from the team.</p>
                <a href="#" class="btn btn-primary">Pledge 1,600 HKD</a>
            </div>

            <div class="tier-card">
                <div class="tier-name">Luxury Plan</div>
                <div class="tier-price">2,400 <span>HKD</span></div>
                <p class="tier-desc">The ultimate plan. Receive the final AL Buds 1 with free laser-etching of any name, message, or symbol of your choice.</p>
                <a href="#" class="btn btn-outline">Pledge 2,400 HKD</a>
            </div>
        </div>
    </section>

    <!-- Stretch Goals Section -->
    <section id="stretch-goals" class="section-padding">
        <h2>Stretch Goals</h2>
        <p class="section-intro">Help us reach these milestones to unlock exclusive features and premium protection.</p>

        <div class="stretch-container">
            <!-- Goal 1 -->
            <div class="stretch-card">
                <div class="stretch-header">
                    <h3 style="margin:0; color:#fff;">Multi-Color & Jewel Customization</h3>
                    <span class="stretch-amount">HKD 50,000</span>
                </div>
                <p style="font-size: 0.9rem; color: var(--text-dim);">Unlocks Sierra Blue, Rose Gold, and Royal Amethyst options with matching jewels. Transform your tech into a high-fashion ensemble.</p>
            </div>
            <!-- Goal 2 -->
            <div class="stretch-card">
                <div class="stretch-header">
                    <h3 style="margin:0; color:#fff;">Premium Protective Earring Case</h3>
                    <span class="stretch-amount">HKD 60,000</span>
                </div>
                <p style="font-size: 0.9rem; color: var(--text-dim);">A jewelry-box-inspired sanctuary with soft-touch lining and shock resistance to keep your AL Buds pristine on the move.</p>
            </div>
        </div>
    </section>

    <footer>
        &copy; 2026 ALMETRIC TECHNOLOGIES // HONG KONG // PRECISION IN EVERY PULSE
    </footer>

</body>
</html>
