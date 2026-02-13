<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AquaFlow — Where Thoughts Flow Like Water</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;600&family=Montserrat:wght@200;300;400;600&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        :root {
            --ink-blue: #0a1828;
            --water-teal: #1e8c93;
            --silver: #c0c5ce;
            --pearl: #f8f9fa;
            --gold-accent: #d4af37;
            --deep-ocean: #001f3f;
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            background: var(--ink-blue);
            overflow-x: hidden;
            cursor: none;
        }
        
        .custom-cursor {
            width: 20px;
            height: 20px;
            border: 2px solid var(--silver);
            border-radius: 50%;
            position: fixed;
            pointer-events: none;
            z-index: 10000;
            transition: all 0.15s ease;
            mix-blend-mode: difference;
        }
        
        .cursor-dot {
            width: 4px;
            height: 4px;
            background: var(--pearl);
            border-radius: 50%;
            position: fixed;
            pointer-events: none;
            z-index: 10001;
            transition: transform 0.1s ease;
        }
        
        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
            background: linear-gradient(135deg, var(--ink-blue) 0%, var(--deep-ocean) 100%);
        }
        
        .water-background {
            position: absolute;
            width: 100%;
            height: 100%;
            opacity: 0.15;
        }
        
        .wave {
            position: absolute;
            width: 200%;
            height: 100%;
            background: linear-gradient(90deg, 
                transparent 0%, 
                var(--water-teal) 25%, 
                transparent 50%, 
                var(--water-teal) 75%, 
                transparent 100%);
            opacity: 0.3;
            animation: wave 20s linear infinite;
        }
        
        .wave:nth-child(2) {
            animation-delay: -5s;
            animation-duration: 25s;
            opacity: 0.2;
        }
        
        .wave:nth-child(3) {
            animation-delay: -10s;
            animation-duration: 30s;
            opacity: 0.1;
        }
        
        @keyframes wave {
            0% { transform: translateX(0) translateY(0) rotate(-3deg); }
            100% { transform: translateX(-50%) translateY(20px) rotate(-3deg); }
        }
        
        .hero-content {
            text-align: center;
            z-index: 10;
            animation: fadeInUp 2s ease-out;
        }
        
        @keyframes fadeInUp {
            0% {
                opacity: 0;
                transform: translateY(50px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .logo {
            font-family: 'Cormorant Garamond', serif;
            font-size: 5rem;
            font-weight: 300;
            color: var(--pearl);
            letter-spacing: 0.3em;
            margin-bottom: 1rem;
            position: relative;
            display: inline-block;
        }
        
        .logo::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 0%;
            height: 1px;
            background: linear-gradient(90deg, transparent, var(--gold-accent), transparent);
            animation: underlineExpand 3s ease-out 1s forwards;
        }
        
        @keyframes underlineExpand {
            to { width: 80%; }
        }
        
        .tagline {
            font-size: 1.2rem;
            font-weight: 200;
            color: var(--silver);
            letter-spacing: 0.15em;
            opacity: 0;
            animation: fadeIn 2s ease-out 1.5s forwards;
        }
        
        @keyframes fadeIn {
            to { opacity: 1; }
        }
        
        .scroll-indicator {
            position: absolute;
            bottom: 3rem;
            left: 50%;
            transform: translateX(-50%);
            color: var(--silver);
            font-size: 0.8rem;
            letter-spacing: 0.2em;
            animation: bounce 2s infinite;
        }
        
        @keyframes bounce {
            0%, 100% { transform: translateX(-50%) translateY(0); }
            50% { transform: translateX(-50%) translateY(10px); }
        }
        
        /* Pen Showcase Section */
        .showcase {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background: var(--pearl);
            position: relative;
            padding: 5rem 2rem;
        }
        
        .showcase-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 5rem;
            max-width: 1400px;
            width: 100%;
            align-items: center;
        }
        
        .pen-visual {
            position: relative;
            height: 600px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .pen {
            width: 500px;
            height: 30px;
            background: linear-gradient(90deg, 
                var(--ink-blue) 0%, 
                var(--water-teal) 50%, 
                var(--ink-blue) 100%);
            border-radius: 15px;
            position: relative;
            box-shadow: 0 30px 60px rgba(0, 0, 0, 0.3);
            animation: penFloat 6s ease-in-out infinite;
            transform-origin: center;
        }
        
        @keyframes penFloat {
            0%, 100% { 
                transform: translateY(0) rotate(-5deg);
                box-shadow: 0 30px 60px rgba(0, 0, 0, 0.3);
            }
            50% { 
                transform: translateY(-20px) rotate(5deg);
                box-shadow: 0 50px 80px rgba(0, 0, 0, 0.4);
            }
        }
        
        .pen-tip {
            position: absolute;
            right: -15px;
            top: 50%;
            transform: translateY(-50%);
            width: 0;
            height: 0;
            border-left: 20px solid var(--ink-blue);
            border-top: 15px solid transparent;
            border-bottom: 15px solid transparent;
        }
        
        .pen-clip {
            position: absolute;
            left: 50px;
            top: -10px;
            width: 4px;
            height: 50px;
            background: var(--gold-accent);
            border-radius: 2px;
            box-shadow: 0 2px 10px rgba(212, 175, 55, 0.5);
        }
        
        .pen-band {
            position: absolute;
            width: 60px;
            height: 100%;
            background: var(--gold-accent);
            left: 30%;
            box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.2);
        }
        
        .ink-flow {
            position: absolute;
            width: 2px;
            height: 100px;
            background: linear-gradient(to bottom, 
                var(--water-teal), 
                transparent);
            right: -20px;
            top: 50%;
            transform: translateY(-50%);
            opacity: 0;
            animation: inkDrip 3s ease-in-out infinite;
        }
        
        @keyframes inkDrip {
            0%, 100% { 
                opacity: 0;
                height: 0;
            }
            50% { 
                opacity: 0.8;
                height: 150px;
            }
        }
        
        .water-ripple {
            position: absolute;
            width: 300px;
            height: 300px;
            border: 2px solid var(--water-teal);
            border-radius: 50%;
            opacity: 0;
            animation: ripple 4s ease-out infinite;
        }
        
        .water-ripple:nth-child(2) {
            animation-delay: 1s;
        }
        
        .water-ripple:nth-child(3) {
            animation-delay: 2s;
        }
        
        @keyframes ripple {
            0% {
                transform: scale(0.5);
                opacity: 0.8;
            }
            100% {
                transform: scale(2);
                opacity: 0;
            }
        }
        
        .showcase-content {
            color: var(--ink-blue);
        }
        
        .showcase-content h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 3.5rem;
            font-weight: 300;
            margin-bottom: 2rem;
            line-height: 1.2;
        }
        
        .feature {
            margin-bottom: 2.5rem;
            opacity: 0;
            transform: translateX(-30px);
            animation: slideIn 1s ease-out forwards;
        }
        
        .feature:nth-child(2) { animation-delay: 0.3s; }
        .feature:nth-child(3) { animation-delay: 0.6s; }
        .feature:nth-child(4) { animation-delay: 0.9s; }
        
        @keyframes slideIn {
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        .feature h3 {
            font-size: 1.3rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: var(--water-teal);
            letter-spacing: 0.05em;
        }
        
        .feature p {
            font-size: 1rem;
            font-weight: 300;
            line-height: 1.8;
            color: var(--deep-ocean);
            opacity: 0.8;
        }
        
        /* Experience Section */
        .experience {
            min-height: 100vh;
            background: var(--ink-blue);
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 5rem 2rem;
            position: relative;
            overflow: hidden;
        }
        
        .ink-drops {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        
        .drop {
            position: absolute;
            width: 6px;
            height: 6px;
            background: var(--water-teal);
            border-radius: 50%;
            opacity: 0;
            animation: dropFall 5s ease-in infinite;
        }
        
        @keyframes dropFall {
            0% {
                opacity: 0;
                transform: translateY(-100px);
            }
            10% { opacity: 0.8; }
            90% { opacity: 0.8; }
            100% {
                opacity: 0;
                transform: translateY(100vh);
            }
        }
        
        .experience-content {
            max-width: 900px;
            text-align: center;
            z-index: 10;
        }
        
        .experience-content h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 4rem;
            font-weight: 300;
            color: var(--pearl);
            margin-bottom: 3rem;
            letter-spacing: 0.1em;
        }
        
        .writing-demo {
            width: 100%;
            height: 300px;
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(192, 197, 206, 0.2);
            border-radius: 8px;
            position: relative;
            overflow: hidden;
            backdrop-filter: blur(10px);
        }
        
        .signature-path {
            position: absolute;
            top: 50%;
            left: 10%;
            transform: translateY(-50%);
            width: 80%;
            height: 2px;
        }
        
        .signature-line {
            stroke: var(--water-teal);
            stroke-width: 3;
            fill: none;
            stroke-linecap: round;
            stroke-linejoin: round;
            filter: drop-shadow(0 0 8px var(--water-teal));
            stroke-dasharray: 1000;
            stroke-dashoffset: 1000;
            animation: drawSignature 4s ease-in-out infinite;
        }
        
        @keyframes drawSignature {
            0%, 100% { stroke-dashoffset: 1000; }
            50%, 90% { stroke-dashoffset: 0; }
        }
        
        /* CTA Section */
        .cta {
            height: 100vh;
            background: linear-gradient(135deg, 
                var(--deep-ocean) 0%, 
                var(--ink-blue) 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
        }
        
        .cta-content {
            text-align: center;
            z-index: 10;
        }
        
        .cta h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 4.5rem;
            font-weight: 300;
            color: var(--pearl);
            margin-bottom: 3rem;
            letter-spacing: 0.2em;
        }
        
        .cta-button {
            display: inline-block;
            padding: 1.5rem 4rem;
            background: transparent;
            border: 2px solid var(--gold-accent);
            color: var(--gold-accent);
            font-size: 1.1rem;
            font-weight: 400;
            letter-spacing: 0.2em;
            text-decoration: none;
            position: relative;
            overflow: hidden;
            transition: all 0.5s ease;
            cursor: pointer;
        }
        
        .cta-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: var(--gold-accent);
            transition: left 0.5s ease;
            z-index: -1;
        }
        
        .cta-button:hover {
            color: var(--ink-blue);
        }
        
        .cta-button:hover::before {
            left: 0;
        }
        
        .price {
            margin-top: 2rem;
            font-size: 1rem;
            color: var(--silver);
            letter-spacing: 0.1em;
            font-weight: 200;
        }
        
        .floating-particles {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        
        .particle {
            position: absolute;
            width: 3px;
            height: 3px;
            background: var(--gold-accent);
            border-radius: 50%;
            opacity: 0.6;
            animation: particleFloat 15s linear infinite;
        }
        
        @keyframes particleFloat {
            0% {
                transform: translate(0, 100vh) rotate(0deg);
                opacity: 0;
            }
            10% { opacity: 0.6; }
            90% { opacity: 0.6; }
            100% {
                transform: translate(200px, -100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .logo { font-size: 3rem; }
            .showcase-grid {
                grid-template-columns: 1fr;
                gap: 3rem;
            }
            .pen { width: 300px; }
            .showcase-content h2 { font-size: 2.5rem; }
            .experience-content h2 { font-size: 2.5rem; }
            .cta h2 { font-size: 2.5rem; }
        }
    </style>
</head>
<body>
    <div class="custom-cursor"></div>
    <div class="cursor-dot"></div>
    
    <!-- Hero Section -->
    <section class="hero">
        <div class="water-background">
            <div class="wave"></div>
            <div class="wave"></div>
            <div class="wave"></div>
        </div>
        
        <div class="hero-content">
            <h1 class="logo">AQUAFLOW</h1>
            <p class="tagline">WHERE THOUGHTS FLOW LIKE WATER</p>
        </div>
        
        <div class="scroll-indicator">SCROLL TO EXPLORE</div>
    </section>
    
    <!-- Showcase Section -->
    <section class="showcase">
        <div class="showcase-grid">
            <div class="pen-visual">
                <div class="water-ripple"></div>
                <div class="water-ripple"></div>
                <div class="water-ripple"></div>
                <div class="pen">
                    <div class="pen-tip"></div>
                    <div class="pen-clip"></div>
                    <div class="pen-band"></div>
                    <div class="ink-flow"></div>
                </div>
            </div>
            
            <div class="showcase-content">
                <h2>Precision<br>Meets<br>Fluidity</h2>
                
                <div class="feature">
                    <h3>AQUA-FLOW TECHNOLOGY</h3>
                    <p>Revolutionary micro-channel system ensures consistent ink flow from first stroke to last, eliminating skips and creating seamless lines.</p>
                </div>
                
                <div class="feature">
                    <h3>ERGONOMIC ELEGANCE</h3>
                    <p>Crafted from aerospace-grade aluminum with a perfectly balanced weight distribution for extended writing sessions without fatigue.</p>
                </div>
                
                <div class="feature">
                    <h3>SAPPHIRE-TIPPED NIB</h3>
                    <p>Ultra-smooth 0.5mm precision tip glides effortlessly across any paper surface, delivering unparalleled writing experience.</p>
                </div>
                
                <div class="feature">
                    <h3>REFILLABLE & SUSTAINABLE</h3>
                    <p>Premium Japanese ink cartridges, easily replaceable. A pen designed to last a lifetime, not a season.</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Experience Section -->
    <section class="experience">
        <div class="ink-drops" id="inkDrops"></div>
        
        <div class="experience-content">
            <h2>Your Thoughts, Perfected</h2>
            
            <div class="writing-demo">
                <svg class="signature-path" viewBox="0 0 800 200" preserveAspectRatio="xMidYMid meet">
                    <path class="signature-line" d="M 50 100 Q 150 50, 250 100 T 450 100 Q 550 80, 650 100 Q 700 110, 750 90" />
                </svg>
            </div>
        </div>
    </section>
    
    <!-- CTA Section -->
    <section class="cta">
        <div class="floating-particles" id="particles"></div>
        
        <div class="cta-content">
            <h2>ELEVATE YOUR CRAFT</h2>
            <a href="#" class="cta-button">ORDER NOW</a>
            <p class="price">$249 — Limited Edition</p>
        </div>
    </section>
    
    <script>
        // Custom cursor
        const cursor = document.querySelector('.custom-cursor');
        const cursorDot = document.querySelector('.cursor-dot');
        
        document.addEventListener('mousemove', (e) => {
            cursor.style.left = e.clientX + 'px';
            cursor.style.top = e.clientY + 'px';
            cursorDot.style.left = (e.clientX + 8) + 'px';
            cursorDot.style.top = (e.clientY + 8) + 'px';
        });
        
        // Ink drops animation
        const inkDrops = document.getElementById('inkDrops');
        for (let i = 0; i < 20; i++) {
            const drop = document.createElement('div');
            drop.className = 'drop';
            drop.style.left = Math.random() * 100 + '%';
            drop.style.animationDelay = Math.random() * 5 + 's';
            drop.style.animationDuration = (5 + Math.random() * 3) + 's';
            inkDrops.appendChild(drop);
        }
        
        // Floating particles
        const particlesContainer = document.getElementById('particles');
        for (let i = 0; i < 30; i++) {
            const particle = document.createElement('div');
            particle.className = 'particle';
            particle.style.left = Math.random() * 100 + '%';
            particle.style.animationDelay = Math.random() * 15 + 's';
            particle.style.animationDuration = (15 + Math.random() * 10) + 's';
            particlesContainer.appendChild(particle);
        }
        
        // Parallax scroll effect
        let lastScrollY = window.scrollY;
        
        window.addEventListener('scroll', () => {
            const scrollY = window.scrollY;
            const delta = scrollY - lastScrollY;
            
            document.querySelectorAll('.wave').forEach((wave, index) => {
                const speed = 0.1 + (index * 0.05);
                wave.style.transform = `translateX(-${scrollY * speed}px)`;
            });
            
            lastScrollY = scrollY;
        });
        
        // Smooth scroll behavior
        document.querySelector('.scroll-indicator').addEventListener('click', () => {
            document.querySelector('.showcase').scrollIntoView({ behavior: 'smooth' });
        });
        
        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.2,
            rootMargin: '0px'
        };
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animationPlayState = 'running';
                }
            });
        }, observerOptions);
        
        document.querySelectorAll('.feature').forEach(feature => {
            feature.style.animationPlayState = 'paused';
            observer.observe(feature);
        });
    </script>
</body>
</html>
