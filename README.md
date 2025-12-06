<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gestão de Tráfego Pago - Transforme Seu Negócio | R9</title>
    <meta name="description" content="Transforme seu negócio com gestão profissional de tráfego pago. Resultados reais, clientes reais, crescimento previsível. Planos a partir de R$ 990.">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --neon: 82 100% 50%;
            --neon-glow: 82 100% 60%;
            --background: 160 30% 3%;
            --foreground: 82 20% 95%;
            --card: 160 25% 6%;
            --card-foreground: 82 20% 95%;
            --muted: 160 20% 12%;
            --muted-foreground: 82 10% 60%;
            --border: 160 20% 15%;
            --accent: 82 80% 45%;
            --destructive: 0 84% 60%;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Outfit', sans-serif;
            background: hsl(var(--background));
            color: hsl(var(--foreground));
            line-height: 1.6;
            overflow-x: hidden;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Space Grotesk', sans-serif;
        }

        /* Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: hsl(var(--background));
        }
        ::-webkit-scrollbar-thumb {
            background: hsl(var(--neon) / 0.3);
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: hsl(var(--neon) / 0.5);
        }

        /* Animations */
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(5deg); }
        }

        @keyframes pulse-glow {
            0%, 100% { box-shadow: 0 0 20px hsl(var(--neon) / 0.3), 0 0 40px hsl(var(--neon) / 0.1); }
            50% { box-shadow: 0 0 40px hsl(var(--neon) / 0.5), 0 0 80px hsl(var(--neon) / 0.2); }
        }

        @keyframes gradient-shift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        @keyframes orbit {
            from { transform: rotate(0deg) translateX(150px) rotate(0deg); }
            to { transform: rotate(360deg) translateX(150px) rotate(-360deg); }
        }

        @keyframes orbit-reverse {
            from { transform: rotate(360deg) translateX(200px) rotate(-360deg); }
            to { transform: rotate(0deg) translateX(200px) rotate(0deg); }
        }

        @keyframes fade-in-up {
            from {
                opacity: 0;
                transform: translateY(40px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes scale-in {
            from {
                opacity: 0;
                transform: scale(0.9);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        @keyframes shine {
            from { left: -100%; }
            to { left: 200%; }
        }

        @keyframes particle-float {
            0%, 100% { transform: translateY(0) translateX(0); opacity: 0.5; }
            25% { transform: translateY(-20px) translateX(10px); opacity: 1; }
            50% { transform: translateY(-10px) translateX(-5px); opacity: 0.7; }
            75% { transform: translateY(-30px) translateX(15px); opacity: 0.9; }
        }

        .animate-on-scroll {
            opacity: 0;
            transform: translateY(40px);
            transition: all 0.8s cubic-bezier(0.16, 1, 0.3, 1);
        }

        .animate-on-scroll.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .stagger-1 { transition-delay: 0.1s; }
        .stagger-2 { transition-delay: 0.2s; }
        .stagger-3 { transition-delay: 0.3s; }
        .stagger-4 { transition-delay: 0.4s; }
        .stagger-5 { transition-delay: 0.5s; }
        .stagger-6 { transition-delay: 0.6s; }
        .stagger-7 { transition-delay: 0.7s; }
        .stagger-8 { transition-delay: 0.8s; }
        .stagger-9 { transition-delay: 0.9s; }

        /* Utilities */
        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 1.5rem;
        }

        .text-gradient {
            background: linear-gradient(135deg, hsl(var(--neon)), hsl(var(--neon-glow)), hsl(82 100% 70%));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
            padding: 1rem 2rem;
            border-radius: 9999px;
            font-weight: 600;
            font-size: 1rem;
            text-decoration: none;
            cursor: pointer;
            border: none;
            transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
            position: relative;
            overflow: hidden;
        }

        .btn-neon {
            background: linear-gradient(135deg, hsl(var(--neon)), hsl(var(--accent)));
            color: hsl(160 30% 5%);
            box-shadow: 0 0 30px hsl(var(--neon) / 0.4), 0 10px 40px hsl(var(--neon) / 0.2);
        }

        .btn-neon:hover {
            transform: scale(1.05);
            box-shadow: 0 0 50px hsl(var(--neon) / 0.6), 0 15px 50px hsl(var(--neon) / 0.3);
        }

        .btn-neon::after {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            animation: shine 3s infinite;
        }

        .btn-whatsapp {
            background: linear-gradient(135deg, #25D366, #128C7E);
            color: white;
            box-shadow: 0 0 30px rgba(37, 211, 102, 0.4);
        }

        .btn-whatsapp:hover {
            transform: scale(1.05);
            box-shadow: 0 0 50px rgba(37, 211, 102, 0.6);
        }

        .glass-card {
            background: hsl(var(--card) / 0.6);
            backdrop-filter: blur(20px);
            border: 1px solid hsl(var(--border) / 0.5);
            border-radius: 1.5rem;
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
            padding: 2rem;
        }

        .hero-bg {
            position: absolute;
            inset: 0;
            background: 
                radial-gradient(ellipse 80% 50% at 50% -20%, hsl(var(--neon) / 0.15), transparent),
                radial-gradient(ellipse 60% 40% at 80% 80%, hsl(160 80% 30% / 0.1), transparent);
        }

        .hero-orb {
            position: absolute;
            border-radius: 50%;
            filter: blur(80px);
            opacity: 0.5;
        }

        .hero-orb-1 {
            width: 400px;
            height: 400px;
            background: hsl(var(--neon) / 0.2);
            top: 10%;
            left: 10%;
            animation: float 8s ease-in-out infinite;
        }

        .hero-orb-2 {
            width: 300px;
            height: 300px;
            background: hsl(160 80% 40% / 0.15);
            bottom: 20%;
            right: 10%;
            animation: float 10s ease-in-out infinite reverse;
        }

        .hero-particles {
            position: absolute;
            inset: 0;
            overflow: hidden;
            pointer-events: none;
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: hsl(var(--neon) / 0.6);
            border-radius: 50%;
            animation: particle-float 6s ease-in-out infinite;
        }

        .orbit-container {
            position: absolute;
            width: 400px;
            height: 400px;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            pointer-events: none;
        }

        .orbit-dot {
            position: absolute;
            width: 8px;
            height: 8px;
            background: hsl(var(--neon));
            border-radius: 50%;
            top: 50%;
            left: 50%;
            box-shadow: 0 0 20px hsl(var(--neon));
        }

        .orbit-dot-1 { animation: orbit 20s linear infinite; }
        .orbit-dot-2 { animation: orbit-reverse 25s linear infinite; }

        .hero-content {
            position: relative;
            z-index: 10;
            text-align: center;
            max-width: 900px;
        }

        .hero-logo {
            width: 140px;
            height: auto;
            margin-bottom: 2rem;
            animation: float 6s ease-in-out infinite;
            filter: drop-shadow(0 0 30px hsl(var(--neon) / 0.5));
        }

        .hero-title {
            font-size: clamp(2.5rem, 6vw, 4.5rem);
            font-weight: 700;
            line-height: 1.1;
            margin-bottom: 1.5rem;
            animation: fade-in-up 1s ease-out;
        }

        .hero-subtitle {
            font-size: clamp(1.1rem, 2.5vw, 1.5rem);
            color: hsl(var(--muted-foreground));
            margin-bottom: 2.5rem;
            animation: fade-in-up 1s ease-out 0.2s both;
        }

        .hero-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
            animation: fade-in-up 1s ease-out 0.4s both;
        }

        .scroll-indicator {
            position: absolute;
            bottom: 2rem;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 0.5rem;
            color: hsl(var(--muted-foreground));
            font-size: 0.875rem;
            animation: bounce 2s infinite;
        }

        .scroll-indicator-line {
            width: 1px;
            height: 40px;
            background: linear-gradient(to bottom, hsl(var(--neon)), transparent);
        }

        /* Problems Section */
        .problems {
            padding: 6rem 0;
            position: relative;
        }

        .section-title {
            font-size: clamp(2rem, 4vw, 3rem);
            text-align: center;
            margin-bottom: 1rem;
        }

        .section-subtitle {
            text-align: center;
            color: hsl(var(--muted-foreground));
            font-size: 1.1rem;
            margin-bottom: 4rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .problems-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
        }

        .problem-card {
            padding: 2rem;
            border-radius: 1.5rem;
            background: hsl(var(--card));
            border: 1px solid hsl(var(--border));
            transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
            position: relative;
            overflow: hidden;
        }

        .problem-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: linear-gradient(90deg, hsl(var(--destructive)), hsl(0 70% 50%));
            opacity: 0;
            transition: opacity 0.3s;
        }

        .problem-card:hover {
            transform: translateY(-8px);
            border-color: hsl(var(--destructive) / 0.3);
            box-shadow: 0 20px 40px hsl(var(--destructive) / 0.1);
        }

        .problem-card:hover::before {
            opacity: 1;
        }

        .problem-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .problem-card h3 {
            font-size: 1.25rem;
            margin-bottom: 0.5rem;
        }

        .problem-card p {
            color: hsl(var(--muted-foreground));
            font-size: 0.95rem;
        }

        /* Solution Section */
        .solution {
            padding: 6rem 0;
            position: relative;
        }

        .solution-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .solution-emoji {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            display: inline-block;
            animation: float 4s ease-in-out infinite;
        }

        .solution-card {
            padding: 3rem;
            margin-top: 2rem;
        }

        .solution-card p {
            font-size: 1.2rem;
            color: hsl(var(--muted-foreground));
            line-height: 1.8;
        }

        .solution-card strong {
            color: hsl(var(--neon));
        }

        /* Funnel Section */
        .funnel {
            padding: 6rem 0;
            position: relative;
        }

        .funnel-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .funnel-card {
            padding: 2rem;
            border-radius: 1.5rem;
            background: hsl(var(--card));
            border: 1px solid hsl(var(--border));
            position: relative;
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }

        .funnel-card::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: linear-gradient(90deg, hsl(var(--neon)), hsl(var(--accent)));
            transform: scaleX(0);
            transition: transform 0.4s;
        }

        .funnel-card:hover {
            transform: translateY(-8px);
            border-color: hsl(var(--neon) / 0.3);
            box-shadow: 0 20px 40px hsl(var(--neon) / 0.1);
        }

        .funnel-card:hover::after {
            transform: scaleX(1);
        }

        .funnel-number {
            position: absolute;
            top: 1rem;
            right: 1rem;
            width: 40px;
            height: 40px;
            background: linear-gradient(135deg, hsl(var(--neon)), hsl(var(--accent)));
            color: hsl(var(--background));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            font-size: 0.9rem;
        }

        .funnel-emoji {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .funnel-card h3 {
            font-size: 1.25rem;
            margin-bottom: 0.75rem;
            color: hsl(var(--neon));
        }

        .funnel-card .objective {
            font-size: 0.95rem;
            color: hsl(var(--foreground));
            margin-bottom: 0.5rem;
        }

        .funnel-card .quote {
            font-style: italic;
            color: hsl(var(--muted-foreground));
            font-size: 0.9rem;
        }

        /* Pricing Section */
        .pricing {
            padding: 6rem 0;
            position: relative;
        }

        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 1.5rem;
        }

        .plan-card {
            padding: 2.5rem;
            border-radius: 1.5rem;
            background: hsl(var(--card));
            border: 1px solid hsl(var(--border));
            position: relative;
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
        }

        .plan-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, hsl(var(--neon)), hsl(var(--accent)));
        }

        .plan-card:hover {
            transform: translateY(-10px);
            border-color: hsl(var(--neon) / 0.3);
            box-shadow: 0 25px 50px hsl(var(--neon) / 0.15);
        }

        .plan-card.featured {
            border-color: hsl(var(--neon) / 0.5);
            box-shadow: 0 0 40px hsl(var(--neon) / 0.2);
        }

        .plan-badge {
            position: absolute;
            top: 1.5rem;
            right: -2rem;
            background: linear-gradient(135deg, hsl(var(--neon)), hsl(var(--accent)));
            color: hsl(var(--background));
            padding: 0.25rem 2.5rem;
            font-size: 0.75rem;
            font-weight: 700;
            transform: rotate(45deg);
        }

        .plan-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .plan-name {
            font-size: 1.75rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
        }

        .plan-desc {
            color: hsl(var(--neon));
            font-size: 0.9rem;
            margin-bottom: 1.5rem;
        }

        .plan-price {
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
        }

        .plan-price span {
            font-size: 1rem;
            color: hsl(var(--muted-foreground));
            font-weight: 400;
        }

        .plan-features {
            list-style: none;
            margin-bottom: 2rem;
        }

        .plan-features li {
            padding: 0.5rem 0;
            display: flex;
            align-items: flex-start;
            gap: 0.75rem;
            font-size: 0.95rem;
            color: hsl(var(--muted-foreground));
        }

        .plan-features li.section-title {
            font-weight: 700;
            color: hsl(var(--foreground));
            margin-top: 1rem;
            border: none;
        }

        .plan-features .check {
            color: hsl(var(--neon));
            font-weight: bold;
        }

        .plan-features .highlight {
            color: hsl(var(--neon));
            font-weight: 600;
        }

        /* Enterprise Section */
        .enterprise {
            padding: 6rem 0;
            background: linear-gradient(180deg, hsl(var(--background)), hsl(160 30% 5%));
        }

        .enterprise-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: start;
        }

        @media (max-width: 900px) {
            .enterprise-grid {
                grid-template-columns: 1fr;
            }
        }

        .enterprise-form {
            padding: 2.5rem;
        }

        .enterprise-form h3 {
            font-size: 1.75rem;
            color: hsl(var(--neon));
            margin-bottom: 2rem;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
            color: hsl(var(--neon));
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 0.875rem 1rem;
            border: 1px solid hsl(var(--border));
            border-radius: 0.75rem;
            background: hsl(var(--muted) / 0.3);
            color: hsl(var(--foreground));
            font-size: 1rem;
            font-family: inherit;
            transition: all 0.3s;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: hsl(var(--neon));
            box-shadow: 0 0 20px hsl(var(--neon) / 0.2);
        }

        .form-group textarea {
            min-height: 100px;
            resize: vertical;
        }

        .checkbox-group {
            display: flex;
            flex-direction: column;
            gap: 0.75rem;
        }

        .checkbox-item {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            padding: 0.875rem 1rem;
            background: hsl(var(--muted) / 0.2);
            border: 1px solid hsl(var(--border));
            border-radius: 0.75rem;
            cursor: pointer;
            transition: all 0.3s;
        }

        .checkbox-item:hover {
            background: hsl(var(--neon) / 0.1);
            border-color: hsl(var(--neon) / 0.3);
        }

        .checkbox-item input[type="checkbox"] {
            width: 18px;
            height: 18px;
            accent-color: hsl(var(--neon));
            cursor: pointer;
        }

        .checkbox-item label {
            cursor: pointer;
            font-size: 0.9rem;
            color: hsl(var(--foreground));
            flex: 1;
        }

        .enterprise-preview {
            position: sticky;
            top: 2rem;
            padding: 2.5rem;
        }

        .enterprise-preview h3 {
            font-size: 1.75rem;
            color: hsl(var(--neon));
            margin-bottom: 1.5rem;
        }

        .preview-empty {
            text-align: center;
            padding: 3rem;
            color: hsl(var(--muted-foreground));
        }

        .preview-section {
            margin-bottom: 1.5rem;
            padding-bottom: 1.5rem;
            border-bottom: 1px solid hsl(var(--border));
        }

        .preview-section:last-of-type {
            border-bottom: none;
        }

        .preview-section h4 {
            color: hsl(var(--neon));
            margin-bottom: 0.75rem;
            font-size: 1.1rem;
        }

        .preview-section ul {
            list-style: none;
        }

        .preview-section li {
            padding: 0.35rem 0;
            color: hsl(var(--muted-foreground));
            font-size: 0.9rem;
        }

        .preview-section li::before {
            content: '✓';
            color: hsl(var(--neon));
            margin-right: 0.75rem;
            font-weight: bold;
        }

        .preview-total {
            font-size: 2.5rem;
            font-weight: 700;
            text-align: center;
            color: hsl(var(--neon));
            margin: 1.5rem 0;
        }

        .preview-discount {
            background: hsl(var(--neon) / 0.1);
            border: 1px solid hsl(var(--neon) / 0.3);
            border-radius: 0.75rem;
            padding: 1rem;
            text-align: center;
            margin-bottom: 1.5rem;
        }

        .preview-discount h4 {
            color: hsl(var(--neon));
            margin-bottom: 0.5rem;
        }

        .preview-discount p {
            color: hsl(var(--muted-foreground));
            font-size: 0.9rem;
        }

        .preview-note {
            background: hsl(var(--muted) / 0.3);
            padding: 1rem;
            border-radius: 0.75rem;
            font-size: 0.85rem;
            color: hsl(var(--muted-foreground));
            margin-top: 1.5rem;
        }

        /* Results Section */
        .results {
            padding: 6rem 0;
            background: linear-gradient(135deg, hsl(160 30% 5%), hsl(var(--background)));
        }

        .results-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 3rem;
        }

        .stat-card {
            padding: 2.5rem;
            text-align: center;
            border-radius: 1.5rem;
            background: hsl(var(--card) / 0.5);
            backdrop-filter: blur(10px);
            border: 1px solid hsl(var(--border));
            transition: all 0.4s;
        }

        .stat-card:hover {
            transform: scale(1.05);
            border-color: hsl(var(--neon) / 0.3);
            box-shadow: 0 20px 40px hsl(var(--neon) / 0.1);
        }

        .stat-number {
            font-size: 3rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
        }

        .stat-label {
            color: hsl(var(--muted-foreground));
            font-size: 1.1rem;
        }

        /* Final CTA */
        .final-cta {
            padding: 6rem 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .final-cta::before {
            content: '';
            position: absolute;
            inset: 0;
            background: radial-gradient(ellipse at center, hsl(var(--neon) / 0.1), transparent 70%);
        }

        .final-cta-content {
            position: relative;
            z-index: 10;
            max-width: 700px;
            margin: 0 auto;
        }

        .final-cta h2 {
            font-size: clamp(1.75rem, 4vw, 2.5rem);
            margin-bottom: 1.5rem;
        }

        .final-cta p {
            font-size: 1.25rem;
            color: hsl(var(--muted-foreground));
            margin-bottom: 2rem;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero {
                padding: 1.5rem;
            }

            .hero-logo {
                width: 100px;
            }

            .btn {
                padding: 0.875rem 1.5rem;
                font-size: 0.9rem;
            }

            .orbit-container {
                display: none;
            }

            .section-title {
                font-size: 1.75rem;
            }

            .pricing-grid,
            .funnel-grid,
            .problems-grid {
                grid-template-columns: 1fr;
            }

            .plan-card {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-bg"></div>
        <div class="hero-orb hero-orb-1"></div>
        <div class="hero-orb hero-orb-2"></div>
        
        <div class="hero-particles">
            <div class="particle" style="left: 10%; top: 20%; animation-delay: 0s;"></div>
            <div class="particle" style="left: 20%; top: 60%; animation-delay: 1s;"></div>
            <div class="particle" style="left: 80%; top: 30%; animation-delay: 2s;"></div>
            <div class="particle" style="left: 70%; top: 70%; animation-delay: 0.5s;"></div>
            <div class="particle" style="left: 40%; top: 80%; animation-delay: 1.5s;"></div>
            <div class="particle" style="left: 90%; top: 50%; animation-delay: 2.5s;"></div>
        </div>

        <div class="orbit-container">
            <div class="orbit-dot orbit-dot-1"></div>
            <div class="orbit-dot orbit-dot-2"></div>
        </div>

        <div class="hero-content">
            <img src="https://i.ibb.co/svdJg9Dp/Design-sem-nome.png" alt="Logo R9" class="hero-logo">
            <h1><span class="text-gradient">🚀 Transforme Seu Negócio</span><br>com Tráfego Pago</h1>
            <p class="hero-subtitle">Resultados reais, clientes reais, crescimento previsível</p>
            <div class="hero-buttons">
                <a href="#pricing" class="btn btn-neon">Ver Planos</a>
                <a href="https://wa.me/5548914260130?text=Olá! Quero saber mais sobre os planos de tráfego pago" class="btn btn-whatsapp" target="_blank">💬 Falar no WhatsApp</a>
            </div>
        </div>

        <div class="scroll-indicator">
            <span>Role para descobrir</span>
            <div class="scroll-indicator-line"></div>
        </div>
    </section>

    <!-- Problems Section -->
    <section class="problems">
        <div class="container">
            <h2 class="section-title animate-on-scroll">O que acontece com a maioria dos negócios?</h2>
            <p class="section-subtitle animate-on-scroll">Problemas comuns que impedem o crescimento</p>
            
            <div class="problems-grid">
                <div class="problem-card animate-on-scroll stagger-1">
                    <div class="problem-icon">❌</div>
                    <h3>Gastam sem retorno</h3>
                    <p>Investem em anúncios sem estratégia e não veem resultados reais</p>
                </div>
                <div class="problem-card animate-on-scroll stagger-2">
                    <div class="problem-icon">❌</div>
                    <h3>Origem desconhecida</h3>
                    <p>Não sabem de onde vêm os clientes nem qual canal funciona melhor</p>
                </div>
                <div class="problem-card animate-on-scroll stagger-3">
                    <div class="problem-icon">❌</div>
                    <h3>Processos manuais</h3>
                    <p>Perdem tempo valioso com tarefas que poderiam ser automatizadas</p>
                </div>
                <div class="problem-card animate-on-scroll stagger-4">
                    <div class="problem-icon">❌</div>
                    <h3>Sem previsibilidade</h3>
                    <p>Crescem de forma aleatória, sem poder planejar o futuro</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Solution Section -->
    <section class="solution">
        <div class="container">
            <div class="solution-content">
                <div class="animate-on-scroll">
                    <div class="solution-emoji">📍</div>
                    <h2 class="section-title"><span class="text-gradient">A Solução</span></h2>
                </div>
                <div class="solution-card glass-card animate-on-scroll stagger-1">
                    <p>Posicione sua empresa como um <strong>outdoor bem localizado em uma avenida movimentada</strong>. Com estratégias de tráfego pago, você atinge exatamente quem precisa dos seus serviços, no momento certo, com a mensagem certa.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Funnel Section -->
    <section class="funnel">
        <div class="container">
            <h2 class="section-title animate-on-scroll">🎯 <span class="text-gradient">Funil de Estratégia Completo</span></h2>
            <p class="section-subtitle animate-on-scroll">9 etapas para transformar desconhecidos em clientes fiéis</p>
            
            <div class="funnel-grid">
                <div class="funnel-card animate-on-scroll stagger-1">
                    <div class="funnel-number">01</div>
                    <div class="funnel-emoji">👁️</div>
                    <h3>Reconhecimento de Marca</h3>
                    <p class="objective"><strong>Objetivo:</strong> Mostrar seu negócio para quem ainda não conhece</p>
                    <p class="quote">"Quem é, onde fica, que vibe é essa?"</p>
                </div>
                <div class="funnel-card animate-on-scroll stagger-2">
                    <div class="funnel-number">02</div>
                    <div class="funnel-emoji">💬</div>
                    <h3>Engajamento</h3>
                    <p class="objective"><strong>Objetivo:</strong> Gerar afinidade e conversa</p>
                    <p class="quote">"Eu gosto desse lugar, parece minha vibe."</p>
                </div>
                <div class="funnel-card animate-on-scroll stagger-3">
                    <div class="funnel-number">03</div>
                    <div class="funnel-emoji">🎯</div>
                    <h3>Conversão</h3>
                    <p class="objective"><strong>Objetivo:</strong> Trazer o público para seu negócio</p>
                    <p class="quote">"Quero ir lá!"</p>
                </div>
                <div class="funnel-card animate-on-scroll stagger-4">
                    <div class="funnel-number">04</div>
                    <div class="funnel-emoji">🔄</div>
                    <h3>Fidelização</h3>
                    <p class="objective"><strong>Objetivo:</strong> Fazer o público voltar</p>
                    <p class="quote">"Esse é meu ponto fixo."</p>
                </div>
                <div class="funnel-card animate-on-scroll stagger-5">
                    <div class="funnel-number">05</div>
                    <div class="funnel-emoji">📣</div>
                    <h3>Advocacia</h3>
                    <p class="objective"><strong>Objetivo:</strong> Transformar clientes em promotores</p>
                    <p class="quote">"Você *tem* que conhecer esse lugar!"</p>
                </div>
                <div class="funnel-card animate-on-scroll stagger-6">
                    <div class="funnel-number">06</div>
                    <div class="funnel-emoji">💰</div>
                    <h3>Upsell</h3>
                    <p class="objective"><strong>Objetivo:</strong> Aumentar o ticket médio</p>
                    <p class="quote">"Já que estou aqui, vou levar isso também."</p>
                </div>
                <div class="funnel-card animate-on-scroll stagger-7">
                    <div class="funnel-number">07</div>
                    <div class="funnel-emoji">🔁</div>
                    <h3>Remarketing</h3>
                    <p class="objective"><strong>Objetivo:</strong> Reconquistar visitantes</p>
                    <p class="quote">"Lembrei daquele produto que eu queria..."</p>
                </div>
                <div class="funnel-card animate-on-scroll stagger-8">
                    <div class="funnel-number">08</div>
                    <div class="funnel-emoji">📊</div>
                    <h3>Análise de Dados</h3>
                    <p class="objective"><strong>Objetivo:</strong> Entender comportamento</p>
                    <p class="quote">"Os números mostram o caminho."</p>
                </div>
                <div class="funnel-card animate-on-scroll stagger-9">
                    <div class="funnel-number">09</div>
                    <div class="funnel-emoji">🧪</div>
                    <h3>Otimização Contínua</h3>
                    <p class="objective"><strong>Objetivo:</strong> Melhorar CPA e ROI</p>
                    <p class="quote">"Vamos testar A contra B."</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section class="pricing" id="pricing">
        <div class="container">
            <h2 class="section-title animate-on-scroll">💎 <span class="text-gradient">Escolha Seu Plano</span></h2>
            <p class="section-subtitle animate-on-scroll">Selecione o plano ideal para o seu negócio</p>
            
            <div class="pricing-grid">
                <!-- Starter -->
                <div class="plan-card animate-on-scroll stagger-1">
                    <div class="plan-icon">🎯</div>
                    <div class="plan-name">Starter</div>
                    <div class="plan-desc">Ideal para quem já tem conteúdo</div>
                    <div class="plan-price">R$ 990<span>/mês</span></div>
                    <ul class="plan-features">
                        <li class="section-title">❌ Audio Visual</li>
                        <li>Você fornece todo material</li>
                        <li class="section-title">✅ Gestão de Tráfego</li>
                        <li><span class="check">✓</span> 2 Campanhas</li>
                        <li><span class="check">✓</span> 3 Dias de Teste</li>
                        <li><span class="check">✓</span> 10 Dias de Otimizações</li>
                        <li><span class="check">✓</span> Suporte via E-mail</li>
                        <li><span class="check">✓</span> Relatório Semanal</li>
                    </ul>
                    <a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Starter" class="btn btn-neon" style="width: 100%;" target="_blank">Quero o Starter</a>
                </div>

                <!-- Inclusive -->
                <div class="plan-card animate-on-scroll stagger-2">
                    <div class="plan-icon">📦</div>
                    <div class="plan-name">Inclusive</div>
                    <div class="plan-desc">Para quem quer começar agora</div>
                    <div class="plan-price">R$ 1.790<span>/mês</span></div>
                    <ul class="plan-features">
                        <li class="section-title">❌ Audio Visual</li>
                        <li>Você fornece vídeos e fotos</li>
                        <li class="section-title">✅ Gestão de Tráfego</li>
                        <li><span class="check">✓</span> 3 Campanhas</li>
                        <li><span class="check">✓</span> 5 Dias de Teste</li>
                        <li><span class="check">✓</span> 15 Dias de Otimizações</li>
                        <li><span class="check">✓</span> Suporte em Horário Comercial</li>
                        <li><span class="check">✓</span> Relatório Quinzenal</li>
                        <li class="section-title">Adicionais*</li>
                        <li>Criação de Posts*</li>
                        <li>Banners* | WhatsApp Auto*</li>
                    </ul>
                    <a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Inclusive" class="btn btn-neon" style="width: 100%;" target="_blank">Quero o Inclusive</a>
                </div>

                <!-- Pro -->
                <div class="plan-card featured animate-on-scroll stagger-3">
                    <div class="plan-badge">+ Popular</div>
                    <div class="plan-icon">🚀</div>
                    <div class="plan-name">Pro</div>
                    <div class="plan-desc">Completo com produção visual</div>
                    <div class="plan-price">R$ 3.680<span>/mês</span></div>
                    <ul class="plan-features">
                        <li class="section-title">✅ Audio Visual</li>
                        <li><span class="check">✓</span> 25 Fotos Profissionais</li>
                        <li><span class="check">✓</span> 2 Vídeos Formato Reels</li>
                        <li class="section-title">✅ Gestão de Tráfego</li>
                        <li><span class="check">✓</span> 3 Campanhas</li>
                        <li><span class="check">✓</span> 5 Dias de Teste</li>
                        <li><span class="check">✓</span> 20 Dias de Otimizações</li>
                        <li><span class="check">✓</span> Suporte Prioritário</li>
                        <li><span class="check">✓</span> Relatório Semanal Detalhado</li>
                        <li class="highlight">Até 10% de desconto nos adicionais</li>
                    </ul>
                    <a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Pro" class="btn btn-neon" style="width: 100%;" target="_blank">Quero o Pro</a>
                </div>

                <!-- Master -->
                <div class="plan-card animate-on-scroll stagger-4">
                    <div class="plan-icon">👑</div>
                    <div class="plan-name">Master</div>
                    <div class="plan-desc">Máximo desempenho e conteúdo</div>
                    <div class="plan-price">R$ 4.190<span>/mês</span></div>
                    <ul class="plan-features">
                        <li class="section-title">✅ Audio Visual Premium</li>
                        <li><span class="check">✓</span> 35 Fotos Profissionais</li>
                        <li><span class="check">✓</span> 3 Vídeos Formato Reels</li>
                        <li><span class="check">✓</span> 1 Vídeo de Drone</li>
                        <li class="section-title">✅ Gestão de Tráfego</li>
                        <li><span class="check">✓</span> 5 Campanhas Simultâneas</li>
                        <li><span class="check">✓</span> 6 Dias de Teste</li>
                        <li><span class="check">✓</span> 25 Dias de Otimizações</li>
                        <li><span class="check">✓</span> Suporte 24 Horas</li>
                        <li class="highlight">Até 25% de desconto nos adicionais</li>
                    </ul>
                    <a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Master" class="btn btn-neon" style="width: 100%;" target="_blank">Quero o Master</a>
                </div>

                <!-- Growth -->
                <div class="plan-card animate-on-scroll stagger-5">
                    <div class="plan-icon">📈</div>
                    <div class="plan-name">Growth</div>
                    <div class="plan-desc">Foco total em conversão</div>
                    <div class="plan-price">R$ 2.490<span>/mês</span></div>
                    <ul class="plan-features">
                        <li class="section-title">❌ Audio Visual</li>
                        <li>Material por sua conta</li>
                        <li class="section-title">✅ Gestão Avançada</li>
                        <li><span class="check">✓</span> 4 Campanhas Simultâneas</li>
                        <li><span class="check">✓</span> 5 Dias de Teste A/B</li>
                        <li><span class="check">✓</span> 20 Dias de Otimizações</li>
                        <li><span class="check">✓</span> Remarketing Avançado</li>
                        <li><span class="check">✓</span> Análise de Concorrência</li>
                        <li><span class="check">✓</span> Dashboard Personalizado</li>
                    </ul>
                    <a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Growth" class="btn btn-neon" style="width: 100%;" target="_blank">Quero o Growth</a>
                </div>

                <!-- Complete -->
                <div class="plan-card animate-on-scroll stagger-6">
                    <div class="plan-icon">💼</div>
                    <div class="plan-name">Complete</div>
                    <div class="plan-desc">Solução 360° completa</div>
                    <div class="plan-price">R$ 5.290<span>/mês</span></div>
                    <ul class="plan-features">
                        <li class="section-title">✅ Audio Visual Completo</li>
                        <li><span class="check">✓</span> 40 Fotos Profissionais</li>
                        <li><span class="check">✓</span> 4 Vídeos Formato Reels</li>
                        <li><span class="check">✓</span> 2 Vídeos de Drone</li>
                        <li class="section-title">✅ Gestão Premium</li>
                        <li><span class="check">✓</span> 6 Campanhas Simultâneas</li>
                        <li><span class="check">✓</span> 30 Dias de Otimizações</li>
                        <li><span class="check">✓</span> Suporte 24/7 WhatsApp</li>
                        <li><span class="check">✓</span> Consultoria Mensal</li>
                        <li class="highlight">Economia de até R$ 1.500</li>
                    </ul>
                    <a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Complete" class="btn btn-neon" style="width: 100%;" target="_blank">Quero o Complete</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Enterprise Section -->
    <section class="enterprise" id="enterprise">
        <div class="container">
            <h2 class="section-title animate-on-scroll">🎨 <span class="text-gradient">Plano Enterprise Personalizado</span></h2>
            <p class="section-subtitle animate-on-scroll">Monte seu plano sob medida e receba um orçamento instantâneo</p>
            
            <div class="enterprise-grid">
                <div class="enterprise-form glass-card animate-on-scroll stagger-1">
                    <h3>📋 Configure Seu Plano</h3>
                    
                    <div class="form-group">
                        <label for="businessName">Nome do Negócio *</label>
                        <input type="text" id="businessName" placeholder="Ex: Velozes Bar Music" required>
                    </div>

                    <div class="form-group">
                        <label for="businessType">Tipo de Negócio *</label>
                        <select id="businessType">
                            <option value="">Selecione...</option>
                            <option value="bar">Bar/Restaurante</option>
                            <option value="loja">Loja/Comércio</option>
                            <option value="servicos">Serviços</option>
                            <option value="saude">Saúde/Bem-estar</option>
                            <option value="educacao">Educação</option>
                            <option value="tecnologia">Tecnologia</option>
                            <option value="outros">Outros</option>
                        </select>
                    </div>

                    <div class="form-group">
                        <label>📸 Audio Visual</label>
                        <div class="checkbox-group">
                            <div class="checkbox-item">
                                <input type="checkbox" id="av-fotos" data-price="800" data-category="audioVisual">
                                <label for="av-fotos">Sessão de Fotos (20-30 fotos) - R$ 800</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="av-fotos-extra" data-price="400" data-category="audioVisual">
                                <label for="av-fotos-extra">Fotos Extras (+15 fotos) - R$ 400</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="av-reels" data-price="600" data-category="audioVisual">
                                <label for="av-reels">Vídeos Reels (2 vídeos) - R$ 600</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="av-drone" data-price="800" data-category="audioVisual">
                                <label for="av-drone">Vídeo de Drone - R$ 800</label>
                            </div>
                        </div>
                    </div>

                    <div class="form-group">
                        <label>🎯 Gestão de Tráfego</label>
                        <div class="checkbox-group">
                            <div class="checkbox-item">
                                <input type="checkbox" id="trafego-basic" data-price="990" data-category="trafego">
                                <label for="trafego-basic">Gestão Básica (2 campanhas) - R$ 990</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="trafego-standard" data-price="1790" data-category="trafego">
                                <label for="trafego-standard">Gestão Standard (3 campanhas) - R$ 1.790</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="trafego-advanced" data-price="2490" data-category="trafego">
                                <label for="trafego-advanced">Gestão Avançada (4 campanhas) - R$ 2.490</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="trafego-premium" data-price="3500" data-category="trafego">
                                <label for="trafego-premium">Gestão Premium (6 campanhas) - R$ 3.500</label>
                            </div>
                        </div>
                    </div>

                    <div class="form-group">
                        <label>📱 Conteúdo e Automação</label>
                        <div class="checkbox-group">
                            <div class="checkbox-item">
                                <input type="checkbox" id="content-posts" data-price="800" data-category="conteudo">
                                <label for="content-posts">Criação de Posts (12/mês) - R$ 800</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="content-banners" data-price="500" data-category="conteudo">
                                <label for="content-banners">Design de Banners (10) - R$ 500</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="content-whatsapp" data-price="600" data-category="conteudo">
                                <label for="content-whatsapp">WhatsApp Automático - R$ 600</label>
                            </div>
                        </div>
                    </div>

                    <div class="form-group">
                        <label>🚀 Extras Premium</label>
                        <div class="checkbox-group">
                            <div class="checkbox-item">
                                <input type="checkbox" id="extra-consultoria" data-price="1200" data-category="extras">
                                <label for="extra-consultoria">Consultoria Mensal - R$ 1.200</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="extra-dashboard" data-price="500" data-category="extras">
                                <label for="extra-dashboard">Dashboard Personalizado - R$ 500</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="extra-landing" data-price="1500" data-category="extras">
                                <label for="extra-landing">Landing Page Profissional - R$ 1.500</label>
                            </div>
                        </div>
                    </div>

                    <div class="form-group">
                        <label for="specialRequests">Solicitações Especiais</label>
                        <textarea id="specialRequests" placeholder="Descreva qualquer necessidade específica..."></textarea>
                    </div>
                </div>

                <div class="enterprise-preview glass-card animate-on-scroll stagger-2">
                    <h3>📊 Seu Orçamento</h3>
                    
                    <div id="previewContent">
                        <p class="preview-empty">Selecione os serviços ao lado para ver seu orçamento personalizado</p>
                    </div>

                    <div class="preview-total" id="totalPrice">R$ 0</div>

                    <div class="preview-note">
                        💡 <strong>Desconto Progressivo:</strong><br>
                        • Acima de R$ 5.000: 10% de desconto<br>
                        • Acima de R$ 8.000: 15% de desconto<br>
                        • Acima de R$ 12.000: 20% de desconto
                    </div>

                    <a href="#" class="btn btn-whatsapp" id="sendQuote" style="width: 100%; margin-top: 1.5rem;">💬 Enviar Orçamento via WhatsApp</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Results Section -->
    <section class="results">
        <div class="container">
            <h2 class="section-title animate-on-scroll">📊 <span class="text-gradient">Resultados em 30 Dias</span></h2>
            
            <div class="results-grid">
                <div class="stat-card animate-on-scroll stagger-1">
                    <div class="stat-number text-gradient" data-target="5800" data-prefix="1,2k - ">5,8k</div>
                    <div class="stat-label">Alcance Diário</div>
                </div>
                <div class="stat-card animate-on-scroll stagger-2">
                    <div class="stat-number text-gradient" data-target="70" data-prefix="15 - ">70</div>
                    <div class="stat-label">Cliques por Dia</div>
                </div>
                <div class="stat-card animate-on-scroll stagger-3">
                    <div class="stat-number text-gradient" data-target="90" data-suffix="%">90%</div>
                    <div class="stat-label">Público Estratégico</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Final CTA -->
    <section class="final-cta">
        <div class="container">
            <div class="final-cta-content">
                <h2 class="animate-on-scroll">Você quer ser mais um no mercado...<br><span class="text-gradient">ou quer ser a referência na sua região?</span></h2>
                <p class="animate-on-scroll stagger-1">Sua agenda com MAIS CLIENTES todos os dias começa agora.</p>
                <a href="https://wa.me/5548914260130?text=Olá! Quero saber mais sobre os planos de tráfego pago" class="btn btn-whatsapp animate-on-scroll stagger-2" target="_blank">💬 Falar no WhatsApp</a>
            </div>
        </div>
    </section>

    <script>
        // Intersection Observer for scroll animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.animate-on-scroll').forEach(el => {
            observer.observe(el);
        });

        // Smooth scroll for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
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

        // Enterprise form calculation
        const checkboxes = document.querySelectorAll('.checkbox-item input[type="checkbox"]');
        const previewContent = document.getElementById('previewContent');
        const totalPriceEl = document.getElementById('totalPrice');
        const sendQuoteBtn = document.getElementById('sendQuote');

        function calculateTotal() {
            let total = 0;
            const selectedItems = {
                audioVisual: [],
                trafego: [],
                conteudo: [],
                extras: []
            };

            checkboxes.forEach(checkbox => {
                if (checkbox.checked) {
                    const price = parseInt(checkbox.dataset.price);
                    const category = checkbox.dataset.category;
                    total += price;
                    const label = checkbox.nextElementSibling.textContent.split(' - ')[0];
                    
                    if (category && selectedItems[category]) {
                        selectedItems[category].push(label);
                    }
                }
            });

            // Progressive discounts
            let discount = 0;
            let discountText = '';
            if (total >= 12000) {
                discount = 0.20;
                discountText = '20% de desconto aplicado!';
            } else if (total >= 8000) {
                discount = 0.15;
                discountText = '15% de desconto aplicado!';
            } else if (total >= 5000) {
                discount = 0.10;
                discountText = '10% de desconto aplicado!';
            }

            const discountAmount = total * discount;
            const finalTotal = total - discountAmount;

            updatePreview(selectedItems, total, discountAmount, finalTotal, discountText);
        }

        function updatePreview(items, subtotal, discount, total, discountText) {
            if (subtotal === 0) {
                previewContent.innerHTML = '<p class="preview-empty">Selecione os serviços ao lado para ver seu orçamento personalizado</p>';
                totalPriceEl.textContent = 'R$ 0';
                return;
            }

            let html = '';

            if (items.audioVisual.length > 0) {
                html += `<div class="preview-section"><h4>📸 Audio Visual</h4><ul>${items.audioVisual.map(item => `<li>${item}</li>`).join('')}</ul></div>`;
            }

            if (items.trafego.length > 0) {
                html += `<div class="preview-section"><h4>🎯 Gestão de Tráfego</h4><ul>${items.trafego.map(item => `<li>${item}</li>`).join('')}</ul></div>`;
            }

            if (items.conteudo.length > 0) {
                html += `<div class="preview-section"><h4>📱 Conteúdo</h4><ul>${items.conteudo.map(item => `<li>${item}</li>`).join('')}</ul></div>`;
            }

            if (items.extras.length > 0) {
                html += `<div class="preview-section"><h4>🚀 Extras</h4><ul>${items.extras.map(item => `<li>${item}</li>`).join('')}</ul></div>`;
            }

            if (discount > 0) {
                html += `<div class="preview-discount"><h4>🎉 ${discountText}</h4><p>De <s>R$ ${subtotal.toLocaleString('pt-BR')}</s> por <strong>R$ ${total.toLocaleString('pt-BR')}</strong></p><p>Economia: R$ ${discount.toLocaleString('pt-BR')}</p></div>`;
            }

            previewContent.innerHTML = html;
            totalPriceEl.textContent = `R$ ${total.toLocaleString('pt-BR')}`;
        }

        checkboxes.forEach(checkbox => {
            checkbox.addEventListener('change', calculateTotal);
        });

        // Send quote via WhatsApp
        sendQuoteBtn.addEventListener('click', function(e) {
            e.preventDefault();
            
            const businessName = document.getElementById('businessName').value;
            const businessType = document.getElementById('businessType').value;
            const specialRequests = document.getElementById('specialRequests').value;

            if (!businessName || !businessType) {
                alert('Por favor, preencha o nome e tipo do negócio');
                return;
            }

            let selectedServices = [];
            checkboxes.forEach(checkbox => {
                if (checkbox.checked) {
                    const label = checkbox.nextElementSibling.textContent;
                    selectedServices.push(label);
                }
            });

            if (selectedServices.length === 0) {
                alert('Por favor, selecione pelo menos um serviço');
                return;
            }

            const totalPrice = totalPriceEl.textContent;
            
            let message = `🎨 *ORÇAMENTO PLANO ENTERPRISE*%0A%0A`;
            message += `*Negócio:* ${businessName}%0A`;
            message += `*Tipo:* ${businessType}%0A%0A`;
            message += `*Serviços Selecionados:*%0A`;
            selectedServices.forEach(service => {
                message += `✓ ${service}%0A`;
            });
            message += `%0A*VALOR TOTAL:* ${totalPrice}%0A`;
            
            if (specialRequests) {
                message += `%0A*Solicitações Especiais:*%0A${specialRequests}`;
            }

            const whatsappUrl = `https://wa.me/5548914260130?text=${message}`;
            window.open(whatsappUrl, '_blank');
        });
    </script>
</body>
</html>

        }
