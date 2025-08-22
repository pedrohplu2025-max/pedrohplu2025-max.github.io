<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Impressione Designs - Estúdio criativo especializado em identidade visual, social media, web e materiais promocionais. Design que gera conexão e resultados.">
    <meta name="keywords" content="design gráfico, identidade visual, social media, branding, São Paulo">
    <meta name="author" content="Impressione Designs">
    
    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://impressione.designs/">
    <meta property="og:title" content="Impressione Designs - Design que gera conexão e resultados">
    <meta property="og:description" content="Estúdio criativo especializado em identidade visual, social media, web e materiais promocionais.">
    <meta property="og:image" content="https://placehold.co/1200x630/6366f1/white?text=Impressione+Designs">

    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://impressione.designs/">
    <meta property="twitter:title" content="Impressione Designs - Design que gera conexão e resultados">
    <meta property="twitter:description" content="Estúdio criativo especializado em identidade visual, social media, web e materiais promocionais.">
    <meta property="twitter:image" content="https://placehold.co/1200x630/6366f1/white?text=Impressione+Designs">

    <title>Impressione Designs - Design que gera conexão e resultados</title>
    
    <!-- Favicon placeholder -->
    <link rel="icon" type="image/x-icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>🎨</text></svg>">
    
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <style>
        /* ========== CSS RESET E VARIÁVEIS ========== */
        :root {
            --primary: #6366f1;
            --primary-dark: #4f46e5;
            --secondary: #f97316;
            --accent: #06b6d4;
            --text-primary: #1f2937;
            --text-secondary: #6b7280;
            --bg-primary: #ffffff;
            --bg-secondary: #f9fafb;
            --bg-card: #ffffff;
            --border: #e5e7eb;
            --shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
            --shadow-lg: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
            --radius: 8px;
            --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        [data-theme="dark"] {
            --text-primary: #f9fafb;
            --text-secondary: #d1d5db;
            --bg-primary: #111827;
            --bg-secondary: #1f2937;
            --bg-card: #1f2937;
            --border: #374151;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
            scroll-padding-top: 80px;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            line-height: 1.6;
            color: var(--text-primary);
            background: var(--bg-primary);
            transition: var(--transition);
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        a {
            text-decoration: none;
            color: inherit;
            transition: var(--transition);
        }

        button {
            border: none;
            background: none;
            font-family: inherit;
            cursor: pointer;
            transition: var(--transition);
        }

        /* ========== UTILITÁRIOS ========== */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1rem;
        }

        .section {
            padding: 5rem 0;
        }

        .section-title {
            font-size: 2.5rem;
            font-weight: 700;
            text-align: center;
            margin-bottom: 1rem;
            color: var(--text-primary);
        }

        .section-subtitle {
            font-size: 1.125rem;
            color: var(--text-secondary);
            text-align: center;
            margin-bottom: 3rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 0.75rem 1.5rem;
            font-weight: 500;
            border-radius: var(--radius);
            transition: var(--transition);
            text-decoration: none;
            cursor: pointer;
            border: 2px solid transparent;
            font-size: 1rem;
        }

        .btn-primary {
            background: var(--primary);
            color: white;
            border-color: var(--primary);
        }

        .btn-primary:hover {
            background: var(--primary-dark);
            border-color: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: var(--shadow-lg);
        }

        .btn-secondary {
            background: transparent;
            color: var(--primary);
            border-color: var(--primary);
        }

        .btn-secondary:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-2px);
        }

        .btn:focus {
            outline: none;
            ring: 2px solid var(--primary);
            ring-offset: 2px;
        }

        /* ========== HEADER E NAVEGAÇÃO ========== */
        .header {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            background: var(--bg-card);
            border-bottom: 1px solid var(--border);
            backdrop-filter: blur(10px);
            z-index: 1000;
            transition: var(--transition);
        }

        .header.scrolled {
            box-shadow: var(--shadow);
        }

        .nav {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 1rem 0;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-link {
            color: var(--text-secondary);
            font-weight: 500;
            padding: 0.5rem 0;
            position: relative;
        }

        .nav-link:hover,
        .nav-link.active {
            color: var(--primary);
        }

        .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary);
            transition: var(--transition);
        }

        .nav-link:hover::after,
        .nav-link.active::after {
            width: 100%;
        }

        .nav-controls {
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .theme-toggle {
            padding: 0.5rem;
            border-radius: 50%;
            background: var(--bg-secondary);
            color: var(--text-primary);
            font-size: 1.2rem;
        }

        .theme-toggle:hover {
            background: var(--primary);
            color: white;
        }

        .mobile-menu-btn {
            display: none;
            padding: 0.5rem;
            font-size: 1.5rem;
        }

        /* ========== HERO SECTION ========== */
        .hero {
            padding: 8rem 0 5rem;
            background: linear-gradient(135deg, var(--bg-primary) 0%, var(--bg-secondary) 100%);
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, var(--primary) 0%, transparent 70%);
            opacity: 0.03;
            animation: float 20s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
        }

        .hero-content {
            position: relative;
            z-index: 1;
        }

        .hero-title {
            font-size: clamp(3rem, 8vw, 5rem);
            font-weight: 700;
            margin-bottom: 1.5rem;
            background: linear-gradient(135deg, var(--primary), var(--accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-subtitle {
            font-size: 1.25rem;
            color: var(--text-secondary);
            margin-bottom: 1rem;
            font-weight: 500;
        }

        .hero-description {
            font-size: 1.125rem;
            color: var(--text-secondary);
            max-width: 700px;
            margin: 0 auto 2.5rem;
            line-height: 1.7;
        }

        .hero-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        /* ========== PORTFÓLIOS SECTION ========== */
        .portfolios {
            background: var(--bg-secondary);
        }

        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .portfolio-card {
            background: var(--bg-card);
            border-radius: var(--radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            cursor: pointer;
            border: 1px solid var(--border);
        }

        .portfolio-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-lg);
        }

        .portfolio-image {
            width: 100%;
            height: 250px;
            object-fit: cover;
            transition: var(--transition);
        }

        .portfolio-card:hover .portfolio-image {
            transform: scale(1.05);
        }

        .portfolio-content {
            padding: 1.5rem;
        }

        .portfolio-title {
            font-size: 1.25rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: var(--text-primary);
        }

        .portfolio-description {
            color: var(--text-secondary);
            margin-bottom: 1rem;
            line-height: 1.6;
        }

        .portfolio-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .portfolio-tag {
            padding: 0.25rem 0.75rem;
            background: var(--primary);
            color: white;
            border-radius: 100px;
            font-size: 0.875rem;
            font-weight: 500;
        }

        /* ========== MODAL ========== */
        .modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            display: none;
            align-items: center;
            justify-content: center;
            z-index: 2000;
            padding: 2rem;
        }

        .modal.active {
            display: flex;
        }

        .modal-content {
            background: var(--bg-card);
            border-radius: var(--radius);
            max-width: 800px;
            width: 100%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
            animation: modalSlideIn 0.3s ease-out;
        }

        @keyframes modalSlideIn {
            from {
                opacity: 0;
                transform: translateY(50px) scale(0.9);
            }
            to {
                opacity: 1;
                transform: translateY(0) scale(1);
            }
        }

        .modal-close {
            position: absolute;
            top: 1rem;
            right: 1rem;
            width: 2rem;
            height: 2rem;
            background: var(--bg-secondary);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            z-index: 1;
        }

        .modal-close:hover {
            background: var(--primary);
            color: white;
        }

        .modal-image {
            width: 100%;
            height: 300px;
            object-fit: cover;
        }

        .modal-body {
            padding: 2rem;
        }

        .modal-title {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 1rem;
        }

        .modal-description {
            color: var(--text-secondary);
            line-height: 1.7;
            margin-bottom: 1.5rem;
        }

        /* ========== PLANOS SECTION ========== */
        .plans-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .plan-card {
            background: var(--bg-card);
            border: 2px solid var(--border);
            border-radius: var(--radius);
            padding: 2rem;
            text-align: center;
            transition: var(--transition);
            position: relative;
        }

        .plan-card:hover {
            border-color: var(--primary);
            transform: translateY(-4px);
            box-shadow: var(--shadow-lg);
        }

        .plan-card.featured {
            border-color: var(--primary);
            transform: scale(1.05);
        }

        .plan-badge {
            position: absolute;
            top: -12px;
            left: 50%;
            transform: translateX(-50%);
            background: var(--primary);
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 100px;
            font-size: 0.875rem;
            font-weight: 600;
        }

        .plan-name {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: var(--text-primary);
        }

        .plan-price {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .plan-price span {
            font-size: 1rem;
            font-weight: 400;
            color: var(--text-secondary);
        }

        .plan-features {
            list-style: none;
            margin-bottom: 2rem;
        }

        .plan-features li {
            padding: 0.5rem 0;
            border-bottom: 1px solid var(--border);
            color: var(--text-secondary);
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .plan-features li:before {
            content: '✓';
            color: var(--primary);
            font-weight: bold;
        }

        .plan-features li:last-child {
            border-bottom: none;
        }

        .plan-note {
            font-size: 0.875rem;
            color: var(--text-secondary);
            margin-top: 2rem;
            padding-top: 1rem;
            border-top: 1px solid var(--border);
            font-style: italic;
        }

        /* ========== CONTATO SECTION ========== */
        .contact {
            background: var(--bg-secondary);
        }

        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: start;
        }

        .contact-form {
            background: var(--bg-card);
            padding: 2rem;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
            color: var(--text-primary);
        }

        .form-input,
        .form-textarea {
            width: 100%;
            padding: 0.75rem;
            border: 2px solid var(--border);
            border-radius: var(--radius);
            font-family: inherit;
            font-size: 1rem;
            background: var(--bg-primary);
            color: var(--text-primary);
            transition: var(--transition);
        }

        .form-input:focus,
        .form-textarea:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(99, 102, 241, 0.1);
        }

        .form-textarea {
            resize: vertical;
            min-height: 120px;
        }

        .contact-info {
            padding-top: 1rem;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 2rem;
            padding: 1.5rem;
            background: var(--bg-card);
            border-radius: var(--radius);
            border: 1px solid var(--border);
            transition: var(--transition);
        }

        .contact-item:hover {
            border-color: var(--primary);
            transform: translateX(4px);
        }

        .contact-icon {
            width: 3rem;
            height: 3rem;
            background: var(--primary);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            flex-shrink: 0;
        }

        .contact-details h3 {
            font-weight: 600;
            margin-bottom: 0.25rem;
            color: var(--text-primary);
        }

        .contact-details p {
            color: var(--text-secondary);
        }

        /* ========== FOOTER ========== */
        .footer {
            background: var(--text-primary);
            color: var(--bg-primary);
            padding: 3rem 0 2rem;
            text-align: center;
        }

        .footer-content {
            margin-bottom: 2rem;
        }

        .social-link {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            padding: 0.75rem 1.5rem;
            background: var(--primary);
            border-radius: 100px;
            color: white;
            font-weight: 500;
            transition: var(--transition);
        }

        .social-link:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
        }

        .footer-text {
            color: #9ca3af;
            font-size: 0.875rem;
        }

        /* ========== RESPONSIVE DESIGN ========== */
        @media (max-width: 768px) {
            .nav-menu {
                position: absolute;
                top: 100%;
                left: 0;
                right: 0;
                background: var(--bg-card);
                flex-direction: column;
                padding: 1rem;
                border-top: 1px solid var(--border);
                transform: translateY(-100%);
                opacity: 0;
                visibility: hidden;
                transition: var(--transition);
            }

            .nav-menu.active {
                transform: translateY(0);
                opacity: 1;
                visibility: visible;
            }

            .mobile-menu-btn {
                display: block;
            }

            .hero-buttons {
                flex-direction: column;
                align-items: center;
            }

            .contact-content {
                grid-template-columns: 1fr;
                gap: 2rem;
            }

            .section-title {
                font-size: 2rem;
            }

            .portfolio-grid {
                grid-template-columns: 1fr;
            }

            .plans-grid {
                grid-template-columns: 1fr;
            }

            .plan-card.featured {
                transform: none;
            }

            .modal {
                padding: 1rem;
            }

            .modal-body {
                padding: 1.5rem;
            }
        }

        @media (max-width: 480px) {
            .container {
                padding: 0 0.75rem;
            }

            .section {
                padding: 3rem 0;
            }

            .hero {
                padding: 6rem 0 3rem;
            }

            .portfolio-grid {
                grid-template-columns: 1fr;
                gap: 1.5rem;
            }

            .portfolio-card {
                min-width: unset;
            }

            .btn {
                width: 100%;
                max-width: 300px;
            }
        }

        /* ========== ANIMAÇÕES E EFEITOS ========== */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease-out;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Carregamento lazy das imagens */
        img[loading="lazy"] {
            opacity: 0;
            transition: opacity 0.3s;
        }

        img[loading="lazy"].loaded {
            opacity: 1;
        }
    </style>
</head>

<body>
    <!-- ========== HEADER ========== -->
    <header class="header" id="header">
        <nav class="nav container">
            <a href="#home" class="logo" aria-label="Impressione Designs - Página inicial">
                Impressione Designs
            </a>
            
            <ul class="nav-menu" id="nav-menu">
                <li><a href="#home" class="nav-link active" aria-label="Ir para seção Home">HOME</a></li>
                <li><a href="#portfolios" class="nav-link" aria-label="Ir para seção Portfólios">PORTFÓLIOS</a></li>
                <li><a href="#planos" class="nav-link" aria-label="Ir para seção Planos">PLANOS</a></li>
                <li><a href="#contatar" class="nav-link" aria-label="Ir para seção Contatar">CONTATAR</a></li>
            </ul>

            <div class="nav-controls">
                <button class="theme-toggle" id="theme-toggle" aria-label="Alternar modo escuro">
                    🌙
                </button>
                <button class="mobile-menu-btn" id="mobile-menu-btn" aria-label="Abrir menu mobile">
                    ☰
                </button>
            </div>
        </nav>
    </header>

    <!-- ========== MAIN CONTENT ========== -->
    <main>
        <!-- ========== HOME/HERO SECTION ========== -->
        <section id="home" class="hero">
            <div class="container">
                <div class="hero-content">
                    <h1 class="hero-title">Impressione Designs</h1>
                    <p class="hero-subtitle">Design que gera conexão e resultados</p>
                    <p class="hero-description">
                        A Impressione Designs é um estúdio criativo especializado em identidade visual, 
                        social media, web e materiais promocionais. Transformamos ideias em marcas 
                        memoráveis e experiências que impressionam.
                    </p>
                    <div class="hero-buttons">
                        <a href="#portfolios" class="btn btn-primary" aria-label="Ver nossos portfólios">
                            Ver Portfólios
                        </a>
                        <a href="#contatar" class="btn btn-secondary" aria-label="Entrar em contato">
                            Fale Conosco
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- ========== PORTFÓLIOS SECTION ========== -->
        <section id="portfolios" class="section portfolios">
            <div class="container">
                <h2 class="section-title">Nossos Portfólios</h2>
                <p class="section-subtitle">
                    Conheça alguns dos projetos que desenvolvemos com muito carinho e dedicação 
                    para nossos clientes.
                </p>

                <div class="portfolio-grid">
                    <!-- Portfolio Item 1 -->
                    <article class="portfolio-card" data-modal="modal1">
                        <img src="https://picsum.photos/400/250?random=1" 
                             alt="Identidade Visual Café Aroma" 
                             class="portfolio-image"
                             loading="lazy">
                        <div class="portfolio-content">
                            <h3 class="portfolio-title">Identidade Visual Café Aroma</h3>
                            <p class="portfolio-description">
                                Desenvolvimento completo da identidade visual para uma cafeteria artesanal, 
                                incluindo logo, paleta de cores e aplicações.
                            </p>
                            <div class="portfolio-tags">
                                <span class="portfolio-tag">Branding</span>
                                <span class="portfolio-tag">Logo</span>
                                <span class="portfolio-tag">Identidade</span>
                            </div>
                        </div>
                    </article>

                    <!-- Portfolio Item 2 -->
                    <article class="portfolio-card" data-modal="modal2">
                        <img src="https://picsum.photos/400/250?random=2" 
                             alt="Social Media TechStart" 
                             class="portfolio-image"
                             loading="lazy">
                        <div class="portfolio-content">
                            <h3 class="portfolio-title">Social Media TechStart</h3>
                            <p class="portfolio-description">
                                Criação de templates e conteúdo visual para redes sociais de uma 
                                startup de tecnologia, aumentando o engajamento em 300%.
                            </p>
                            <div class="portfolio-tags">
                                <span class="portfolio-tag">Social Media</span>
                                <span class="portfolio-tag">Templates</span>
                                <span class="portfolio-tag">Instagram</span>
                            </div>
                        </div>
                    </article>

                    <!-- Portfolio Item 3 -->
                    <article class="portfolio-card" data-modal="modal3">
                        <img src="https://picsum.photos/400/250?random=3" 
                             alt="Website Clínica Bem-Estar" 
                             class="portfolio-image"
                             loading="lazy">
                        <div class="portfolio-content">
                            <h3 class="portfolio-title">Website Clínica Bem-Estar</h3>
                            <p class="portfolio-description">
                                Design e desenvolvimento de website responsivo para clínica de saúde, 
                                com foco na experiência do usuário e conversões.
                            </p>
                            <div class="portfolio-tags">
                                <span class="portfolio-tag">Web Design</span>
                                <span class="portfolio-tag">UX/UI</span>
                                <span class="portfolio-tag">Responsivo</span>
                            </div>
                        </div>
                    </article>

                    <!-- Portfolio Item 4 -->
                    <article class="portfolio-card" data-modal="modal4">
                        <img src="https://picsum.photos/400/250?random=4" 
                             alt="Material Promocional Evento Fashion" 
                             class="portfolio-image"
                             loading="lazy">
                        <div class="portfolio-content">
                            <h3 class="portfolio-title">Material Promocional Evento Fashion</h3>
                            <p class="portfolio-description">
                                Criação de materiais gráficos para evento de moda, incluindo cartazes, 
                                flyers, convites e sinalização.
                            </p>
                            <div class="portfolio-tags">
                                <span class="portfolio-tag">Print</span>
                                <span class="portfolio-tag">Evento</span>
                                <span class="portfolio-tag">Promocional</span>
                            </div>
                        </div>
                    </article>

                    <!-- Portfolio Item 5 -->
                    <article class="portfolio-card" data-modal="modal5">
                        <img src="https://picsum.photos/400/250?random=5" 
                             alt="E-commerce Loja Natureza" 
                             class="portfolio-image"
                             loading="lazy">
                        <div class="portfolio-content">
                            <h3 class="portfolio-title">E-commerce Loja Natureza</h3>
                            <p class="portfolio-description">
                                Interface completa para e-commerce de produtos naturais, com design 
                                clean e foco na conversão de vendas.
                            </p>
                            <div class="portfolio-tags">
                                <span class="portfolio-tag">E-commerce</span>
                                <span class="portfolio-tag">UI Design</span>
                                <span class="portfolio-tag">Conversão</span>
                            </div>
                        </div>
                    </article>

                    <!-- Portfolio Item 6 -->
                    <article class="portfolio-card" data-modal="modal6">
                        <img src="https://picsum.photos/400/250?random=6" 
                             alt="Rebranding Empresa Logística" 
                             class="portfolio-image"
                             loading="lazy">
                        <div class="portfolio-content">
                            <h3 class="portfolio-title">Rebranding Empresa Logística</h3>
                            <p class="portfolio-description">
                                Renovação completa da marca de uma empresa de logística, modernizando 
                                a identidade visual e comunicação.
                            </p>
                            <div class="portfolio-tags">
                                <span class="portfolio-tag">Rebranding</span>
                                <span class="portfolio-tag">Logística</span>
                                <span class="portfolio-tag">Modernização</span>
                            </div>
                        </div>
                    </article>

                    <!-- Portfolio Item 7 -->
                    <article class="portfolio-card" data-modal="modal7">
                        <img src="https://picsum.photos/400/250?random=7" 
                             alt="App Mobile FitnessTracker" 
                             class="portfolio-image"
                             loading="lazy">
                        <div class="portfolio-content">
                            <h3 class="portfolio-title">App Mobile FitnessTracker</h3>
                            <p class="portfolio-description">
                                Design de interface para aplicativo mobile de fitness, priorizando 
                                usabilidade e motivação dos usuários.
                            </p>
                            <div class="portfolio-tags">
                                <span class="portfolio-tag">Mobile</span>
                                <span class="portfolio-tag">App Design</span>
                                <span class="portfolio-tag">Fitness</span>
                            </div>
                        </div>
                    </article>

                    <!-- Portfolio Item 8 -->
                    <article class="portfolio-card" data-modal="modal8">
                        <img src="https://picsum.photos/400/250?random=8" 
                             alt="Catálogo Digital Móveis Designer" 
                             class="portfolio-image"
                             loading="lazy">
                        <div class="portfolio-content">
                            <h3 class="portfolio-title">Catálogo Digital Móveis Designer</h3>
                            <p class="portfolio-description">
                                Criação de catálogo digital interativo para loja de móveis de design, 
                                com foco na apresentação elegante dos produtos.
                            </p>
                            <div class="portfolio-tags">
                                <span class="portfolio-tag">Catálogo</span>
                                <span class="portfolio-tag">Digital</span>
                                <span class="portfolio-tag">Interativo</span>
                            </div>
                        </div>
                    </article>
                </div>
            </div>
        </section>

        <!-- ========== PLANOS SECTION ========== -->
        <section id="planos" class="section">
            <div class="container">
                <h2 class="section-title">Nossos Planos</h2>
                <p class="section-subtitle">
                    Escolha o plano ideal para o seu projeto. Todos incluem nossa garantia de qualidade 
                    e suporte especializado.
                </p>

                <div class="plans-grid">
                    <!-- Plano Start -->
                    <div class="plan-card">
                        <h3 class="plan-name">Start</h3>
                        <div class="plan-price">
                            R$ 299
                            <span>/projeto</span>
                        </div>
                        <ul class="plan-features">
                            <li>1 peça gráfica personalizada</li>
                            <li>1 revisão incluída</li>
                            <li>Entrega em 3 dias úteis</li>
                            <li>Arquivos em alta resolução</li>
                            <li>Suporte via WhatsApp</li>
                        </ul>
                        <a href="#contatar" class="btn btn-primary">Contratar agora</a>
                    </div>

                    <!-- Plano Pro -->
                    <div class="plan-card featured">
                        <div class="plan-badge">Mais Popular</div>
                        <h3 class="plan-name">Pro</h3>
                        <div class="plan-price">
                            R$ 799
                            <span>/pacote</span>
                        </div>
                        <ul class="plan-features">
                            <li>5 peças gráficas ou kit social</li>
                            <li>2 revisões incluídas</li>
                            <li>Entrega em 5 dias úteis</li>
                            <li>Guia rápido de uso</li>
                            <li>Arquivos editáveis</li>
                            <li>Suporte prioritário</li>
                        </ul>
                        <a href="#contatar" class="btn btn-primary">Contratar agora</a>
                    </div>

                    <!-- Plano Premium -->
                    <div class="plan-card">
                        <h3 class="plan-name">Premium</h3>
                        <div class="plan-price">
                            R$ 1.499
                            <span>/pacote</span>
                        </div>
                        <ul class="plan-features">
                            <li>Identidade visual básica</li>
                            <li>Logo + paleta + tipografia</li>
                            <li>3 revisões incluídas</li>
                            <li>Mockups profissionais</li>
                            <li>Manual da marca</li>
                            <li>Suporte por 30 dias</li>
                        </ul>
                        <a href="#contatar" class="btn btn-primary">Contratar agora</a>
                    </div>

                    <!-- Plano Enterprise -->
                    <div class="plan-card">
                        <h3 class="plan-name">Enterprise</h3>
                        <div class="plan-price">
                            Sob consulta
                            <span>/projeto</span>
                        </div>
                        <ul class="plan-features">
                            <li>Pacote personalizado</li>
                            <li>Reunião de briefing</li>
                            <li>Revisões ilimitadas*</li>
                            <li>Entrega conforme acordado</li>
                            <li>Suporte dedicado</li>
                            <li>Consultoria estratégica</li>
                        </ul>
                        <a href="#contatar" class="btn btn-primary">Solicitar orçamento</a>
                    </div>
                </div>

                <div class="plan-note">
                    <p><strong>Condições:</strong> Os prazos começam a contar após aprovação do briefing. 
                    Revisões adicionais podem ter custo extra. *Revisões ilimitadas no plano Enterprise 
                    respeitam o escopo inicial do projeto.</p>
                </div>
            </div>
        </section>

        <!-- ========== CONTATO SECTION ========== -->
        <section id="contatar" class="section contact">
            <div class="container">
                <h2 class="section-title">Entre em Contato</h2>
                <p class="section-subtitle">
                    Pronto para começar seu projeto? Entre em contato conosco e vamos criar algo incrível juntos!
                </p>

                <div class="contact-content">
                    <!-- Formulário de Contato -->
                    <div class="contact-form">
                        <form id="contact-form" action="mailto:contato@impressione.designs" method="post" enctype="text/plain">
                            <div class="form-group">
                                <label for="name" class="form-label">Nome Completo *</label>
                                <input 
                                    type="text" 
                                    id="name" 
                                    name="name" 
                                    class="form-input" 
                                    required
                                    aria-describedby="name-error">
                                <div id="name-error" class="error-message" role="alert"></div>
                            </div>

                            <div class="form-group">
                                <label for="email" class="form-label">E-mail *</label>
                                <input 
                                    type="email" 
                                    id="email" 
                                    name="email" 
                                    class="form-input" 
                                    required
                                    aria-describedby="email-error">
                                <div id="email-error" class="error-message" role="alert"></div>
                            </div>

                            <div class="form-group">
                                <label for="message" class="form-label">Mensagem *</label>
                                <textarea 
                                    id="message" 
                                    name="message" 
                                    class="form-textarea" 
                                    placeholder="Conte-nos sobre seu projeto, objetivos e prazos..."
                                    required
                                    aria-describedby="message-error"></textarea>
                                <div id="message-error" class="error-message" role="alert"></div>
                            </div>

                            <button type="submit" class="btn btn-primary" style="width: 100%;">
                                Enviar Mensagem
                            </button>
                        </form>
                    </div>

                    <!-- Informações de Contato -->
                    <div class="contact-info">
                        <div class="contact-item">
                            <div class="contact-icon" aria-hidden="true">
                                ✉️
                            </div>
                            <div class="contact-details">
                                <h3>E-mail</h3>
                                <p>contato@impressione.designs</p>
                            </div>
                        </div>

                        <div class="contact-item">
                            <div class="contact-icon" aria-hidden="true">
                                📱
                            </div>
                            <div class="contact-details">
                                <h3>WhatsApp</h3>
                                <p>(00) 00000-0000</p>
                            </div>
                        </div>

                        <div class="contact-item">
                            <div class="contact-icon" aria-hidden="true">
                                🕒
                            </div>
                            <div class="contact-details">
                                <h3>Horário de Atendimento</h3>
                                <p>Segunda à Sexta: 9h às 18h<br>
                                Sábados: 9h às 14h</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- ========== FOOTER ========== -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <a href="https://instagram.com/impressione.designs" 
                   class="social-link" 
                   target="_blank" 
                   rel="noopener noreferrer"
                   aria-label="Seguir @impressione.designs no Instagram">
                    📷 @impressione.designs
                </a>
            </div>
            <p class="footer-text">
                © <span id="current-year">2024</span> Impressione Designs. Todos os direitos reservados.
            </p>
        </div>
    </footer>

    <!-- ========== MODAIS DOS PORTFÓLIOS ========== -->
    <!-- Modal 1 -->
    <div class="modal" id="modal1">
        <div class="modal-content">
            <button class="modal-close" aria-label="Fechar modal">&times;</button>
            <img src="https://picsum.photos/800/400?random=1" alt="Identidade Visual Café Aroma - Imagem ampliada" class="modal-image">
            <div class="modal-body">
                <h3 class="modal-title">Identidade Visual Café Aroma</h3>
                <p class="modal-description">
                    Projeto completo de identidade visual para a cafeteria artesanal "Café Aroma". 
                    O trabalho incluiu a criação do logotipo, definição da paleta de cores, 
                    tipografia institucional e aplicações em diversos materiais como cartões de visita, 
                    cardápio, uniformes e sinalização interna. O conceito desenvolvido transmite 
                    aconchego e qualidade, refletindo os valores da marca e criando uma conexão 
                    emocional com o público-alvo.
                </p>
                <div class="portfolio-tags">
                    <span class="portfolio-tag">Branding</span>
                    <span class="portfolio-tag">Logo</span>
                    <span class="portfolio-tag">Identidade</span>
                    <span class="portfolio-tag">Aplicações</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal 2 -->
    <div class="modal" id="modal2">
        <div class="modal-content">
            <button class="modal-close" aria-label="Fechar modal">&times;</button>
            <img src="https://picsum.photos/800/400?random=2" alt="Social Media TechStart - Imagem ampliada" class="modal-image">
            <div class="modal-body">
                <h3 class="modal-title">Social Media TechStart</h3>
                <p class="modal-description">
                    Desenvolvimento de estratégia visual e criação de templates personalizados para as 
                    redes sociais da startup TechStart. O projeto resultou em um aumento de 300% no 
                    engajamento e 150% no número de seguidores em 6 meses. Foram criados mais de 50 
                    templates diferentes para posts, stories, carrosséis e campanhas publicitárias, 
                    mantendo sempre a consistência visual da marca.
                </p>
                <div class="portfolio-tags">
                    <span class="portfolio-tag">Social Media</span>
                    <span class="portfolio-tag">Templates</span>
                    <span class="portfolio-tag">Instagram</span>
                    <span class="portfolio-tag">Estratégia</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal 3 -->
    <div class="modal" id="modal3">
        <div class="modal-content">
            <button class="modal-close" aria-label="Fechar modal">&times;</button>
            <img src="https://picsum.photos/800/400?random=3" alt="Website Clínica Bem-Estar - Imagem ampliada" class="modal-image">
            <div class="modal-body">
                <h3 class="modal-title">Website Clínica Bem-Estar</h3>
                <p class="modal-description">
                    Design e desenvolvimento completo do website responsivo para a Clínica Bem-Estar. 
                    O projeto focou na criação de uma experiência de usuário intuitiva e acessível, 
                    com agendamento online, área do paciente e sistema de teleconsulta. O resultado 
                    foi um aumento de 250% nas conversões e 40% na retenção de pacientes. 
                    O site é totalmente otimizado para SEO e carregamento rápido.
                </p>
                <div class="portfolio-tags">
                    <span class="portfolio-tag">Web Design</span>
                    <span class="portfolio-tag">UX/UI</span>
                    <span class="portfolio-tag">Responsivo</span>
                    <span class="portfolio-tag">Saúde</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal 4 -->
    <div class="modal" id="modal4">
        <div class="modal-content">
            <button class="modal-close" aria-label="Fechar modal">&times;</button>
            <img src="https://picsum.photos/800/400?random=4" alt="Material Promocional Evento Fashion - Imagem ampliada" class="modal-image">
            <div class="modal-body">
                <h3 class="modal-title">Material Promocional Evento Fashion</h3>
                <p class="modal-description">
                    Criação de toda a comunicação visual para o evento "Fashion Week Local", incluindo 
                    cartazes, flyers, convites VIP, sinalização, credenciais e materiais digitais. 
                    O conceito visual desenvolvido transmitiu elegância e modernidade, contribuindo 
                    para o sucesso do evento que recebeu mais de 5.000 visitantes e grande repercussão 
                    na mídia local.
                </p>
                <div class="portfolio-tags">
                    <span class="portfolio-tag">Print</span>
                    <span class="portfolio-tag">Evento</span>
                    <span class="portfolio-tag">Promocional</span>
                    <span class="portfolio-tag">Fashion</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal 5 -->
    <div class="modal" id="modal5">
        <div class="modal-content">
            <button class="modal-close" aria-label="Fechar modal">&times;</button>
            <img src="https://picsum.photos/800/400?random=5" alt="E-commerce Loja Natureza - Imagem ampliada" class="modal-image">
            <div class="modal-body">
                <h3 class="modal-title">E-commerce Loja Natureza</h3>
                <p class="modal-description">
                    Desenvolvimento da interface completa para e-commerce especializado em produtos 
                    naturais e orgânicos. O design clean e intuitivo, combinado com fotografias 
                    profissionais dos produtos, resultou em uma taxa de conversão 35% acima da média 
                    do setor. O projeto incluiu também a criação de ícones personalizados, 
                    sistema de avaliações e checkout otimizado.
                </p>
                <div class="portfolio-tags">
                    <span class="portfolio-tag">E-commerce</span>
                    <span class="portfolio-tag">UI Design</span>
                    <span class="portfolio-tag">Conversão</span>
                    <span class="portfolio-tag">Natural</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal 6 -->
    <div class="modal" id="modal6">
        <div class="modal-content">
            <button class="modal-close" aria-label="Fechar modal">&times;</button>
            <img src="https://picsum.photos/800/400?random=6" alt="Rebranding Empresa Logística - Imagem ampliada" class="modal-image">
            <div class="modal-body">
                <h3 class="modal-title">Rebranding Empresa Logística</h3>
                <p class="modal-description">
                    Renovação completa da marca da empresa LogiMove, incluindo novo logotipo, 
                    identidade visual, frotas de veículos, uniformes e materiais corporativos. 
                    O rebranding modernizou a percepção da empresa no mercado, transmitindo 
                    confiabilidade, eficiência e tecnologia. O projeto foi implementado em 
                    mais de 200 pontos de contato da marca em todo o país.
                </p>
                <div class="portfolio-tags">
                    <span class="portfolio-tag">Rebranding</span>
                    <span class="portfolio-tag">Logística</span>
                    <span class="portfolio-tag">Modernização</span>
                    <span class="portfolio-tag">Corporativo</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal 7 -->
    <div class="modal" id="modal7">
        <div class="modal-content">
            <button class="modal-close" aria-label="Fechar modal">&times;</button>
            <img src="https://picsum.photos/800/400?random=7" alt="App Mobile FitnessTracker - Imagem ampliada" class="modal-image">
            <div class="modal-body">
                <h3 class="modal-title">App Mobile FitnessTracker</h3>
                <p class="modal-description">
                    Design de interface para aplicativo mobile de acompanhamento fitness, com foco 
                    na motivação e facilidade de uso. O app inclui dashboard personalizado, 
                    tracking de exercícios, metas gamificadas e integração com dispositivos wearables. 
                    A interface intuitiva e as micro-interações contribuíram para uma alta taxa de 
                    retenção de usuários e avaliação 4.8 estrelas nas lojas de aplicativos.
                </p>
                <div class="portfolio-tags">
                    <span class="portfolio-tag">Mobile</span>
                    <span class="portfolio-tag">App Design</span>
                    <span class="portfolio-tag">Fitness</span>
                    <span class="portfolio-tag">UX</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal 8 -->
    <div class="modal" id="modal8">
        <div class="modal-content">
            <button class="modal-close" aria-label="Fechar modal">&times;</button>
            <img src="https://picsum.photos/800/400?random=8" alt="Catálogo Digital Móveis Designer - Imagem ampliada" class="modal-image">
            <div class="modal-body">
                <h3 class="modal-title">Catálogo Digital Móveis Designer</h3>
                <p class="modal-description">
                    Criação de catálogo digital interativo para loja de móveis de design de alto padrão. 
                    O projeto incluiu fotografia profissional, animações suaves, visualização 360°, 
                    configurador de ambientes e realidade aumentada. O catálogo digital aumentou as 
                    vendas online em 180% e reduziu significativamente os custos de impressão de 
                    materiais promocionais.
                </p>
                <div class="portfolio-tags">
                    <span class="portfolio-tag">Catálogo</span>
                    <span class="portfolio-tag">Digital</span>
                    <span class="portfolio-tag">Interativo</span>
                    <span class="portfolio-tag">Móveis</span>
                </div>
            </div>
        </div>
    </div>

    <!-- ========== JAVASCRIPT ========== -->
    <script>
        // ========== VARIÁVEIS GLOBAIS ==========
        const header = document.getElementById('header');
        const navLinks = document.querySelectorAll('.nav-link');
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const navMenu = document.getElementById('nav-menu');
        const themeToggle = document.getElementById('theme-toggle');
        const portfolioCards = document.querySelectorAll('.portfolio-card');
        const modals = document.querySelectorAll('.modal');
        const contactForm = document.getElementById('contact-form');
        const currentYearSpan = document.getElementById('current-year');

        // ========== INICIALIZAÇÃO ==========
        document.addEventListener('DOMContentLoaded', function() {
            initializeApp();
        });

        function initializeApp() {
            // Atualizar ano atual no footer
            if (currentYearSpan) {
                currentYearSpan.textContent = new Date().getFullYear();
            }

            // Configurar tema inicial
            initializeTheme();
            
            // Configurar navegação
            setupNavigation();
            
            // Configurar menu mobile
            setupMobileMenu();
            
            // Configurar modais do portfólio
            setupPortfolioModals();
            
            // Configurar formulário de contato
            setupContactForm();
            
            // Configurar animações de scroll
            setupScrollAnimations();
            
            // Configurar carregamento lazy de imagens
            setupLazyLoading();

            // Configurar eventos de teclado para acessibilidade
            setupKeyboardNavigation();
        }

        // ========== TEMA ESCURO/CLARO ==========
        function initializeTheme() {
            const savedTheme = localStorage.getItem('theme') || 'light';
            document.documentElement.setAttribute('data-theme', savedTheme);
            updateThemeToggle(savedTheme);

            if (themeToggle) {
                themeToggle.addEventListener('click', toggleTheme);
            }
        }

        function toggleTheme() {
            const currentTheme = document.documentElement.getAttribute('data-theme');
            const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
            
            document.documentElement.setAttribute('data-theme', newTheme);
            localStorage.setItem('theme', newTheme);
            updateThemeToggle(newTheme);
        }

        function updateThemeToggle(theme) {
            if (themeToggle) {
                themeToggle.textContent = theme === 'dark' ? '☀️' : '🌙';
                themeToggle.setAttribute('aria-label', 
                    theme === 'dark' ? 'Alternar para modo claro' : 'Alternar para modo escuro'
                );
            }
        }

        // ========== NAVEGAÇÃO ==========
        function setupNavigation() {
            // Rolagem suave para seções
            navLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    const targetId = this.getAttribute('href');
                    const targetSection = document.querySelector(targetId);
                    
                    if (targetSection) {
                        targetSection.scrollIntoView({
                            behavior: 'smooth',
                            block: 'start'
                        });
                        
                        // Fechar menu mobile se estiver aberto
                        if (navMenu.classList.contains('active')) {
                            toggleMobileMenu();
                        }
                    }
                });
            });

            // Destacar seção ativa no scroll
            window.addEventListener('scroll', handleScroll);
        }

        function handleScroll() {
            // Adicionar classe scrolled ao header
            if (window.scrollY > 100) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }

            // Atualizar link ativo da navegação
            const sections = document.querySelectorAll('section[id]');
            const scrollPosition = window.scrollY + 150;

            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.offsetHeight;
                const sectionId = section.getAttribute('id');
                const correspondingLink = document.querySelector(`.nav-link[href="#${sectionId}"]`);

                if (correspondingLink && 
                    scrollPosition >= sectionTop && 
                    scrollPosition < sectionTop + sectionHeight) {
                    
                    // Remover classe active de todos os links
                    navLinks.forEach(link => link.classList.remove('active'));
                    
                    // Adicionar classe active ao link atual
                    correspondingLink.classList.add('active');
                }
            });
        }

        // ========== MENU MOBILE ==========
        function setupMobileMenu() {
            if (mobileMenuBtn) {
                mobileMenuBtn.addEventListener('click', toggleMobileMenu);
            }

            // Fechar menu ao clicar fora
            document.addEventListener('click', function(e) {
                if (!mobileMenuBtn.contains(e.target) && 
                    !navMenu.contains(e.target) && 
                    navMenu.classList.contains('active')) {
                    toggleMobileMenu();
                }
            });

            // Fechar menu ao redimensionar janela
            window.addEventListener('resize', function() {
                if (window.innerWidth > 768 && navMenu.classList.contains('active')) {
                    toggleMobileMenu();
                }
            });
        }

        function toggleMobileMenu() {
            navMenu.classList.toggle('active');
            const isOpen = navMenu.classList.contains('active');
            
            // Atualizar acessibilidade
            mobileMenuBtn.setAttribute('aria-expanded', isOpen);
            mobileMenuBtn.setAttribute('aria-label', 
                isOpen ? 'Fechar menu mobile' : 'Abrir menu mobile'
            );
            
            // Atualizar ícone
            mobileMenuBtn.textContent = isOpen ? '✕' : '☰';
        }

        // ========== PORTFÓLIO E MODAIS ==========
        function setupPortfolioModals() {
            portfolioCards.forEach(card => {
                card.addEventListener('click', function() {
                    const modalId = this.getAttribute('data-modal');
                    const modal = document.getElementById(modalId);
                    
                    if (modal) {
                        openModal(modal);
                    }
                });

                // Acessibilidade via teclado
                card.addEventListener('keydown', function(e) {
                    if (e.key === 'Enter' || e.key === ' ') {
                        e.preventDefault();
                        this.click();
                    }
                });

                // Tornar focável
                card.setAttribute('tabindex', '0');
                card.setAttribute('role', 'button');
                card.setAttribute('aria-label', 'Abrir detalhes do projeto');
            });

            // Configurar botões de fechar e eventos de modal
            modals.forEach(modal => {
                const closeBtn = modal.querySelector('.modal-close');
                
                if (closeBtn) {
                    closeBtn.addEventListener('click', function() {
                        closeModal(modal);
                    });
                }

                // Fechar modal ao clicar no overlay
                modal.addEventListener('click', function(e) {
                    if (e.target === modal) {
                        closeModal(modal);
                    }
                });

                // Fechar modal com tecla ESC
                document.addEventListener('keydown', function(e) {
                    if (e.key === 'Escape' && modal.classList.contains('active')) {
                        closeModal(modal);
                    }
                });
            });
        }

        function openModal(modal) {
            modal.classList.add('active');
            document.body.style.overflow = 'hidden';
            
            // Focar no botão de fechar para acessibilidade
            const closeBtn = modal.querySelector('.modal-close');
            if (closeBtn) {
                closeBtn.focus();
            }
        }

        function closeModal(modal) {
            modal.classList.remove('active');
            document.body.style.overflow = '';
        }

        // ========== FORMULÁRIO DE CONTATO ==========
        function setupContactForm() {
            if (!contactForm) return;

            contactForm.addEventListener('submit', function(e) {
                e.preventDefault();
                
                if (validateForm()) {
                    // Simular envio (já que não temos backend)
                    showFormSuccess();
                    
                    // Limpar formulário após sucesso
                    setTimeout(() => {
                        this.reset();
                        clearFormErrors();
                    }, 2000);
                }
            });

            // Validação em tempo real
            const inputs = contactForm.querySelectorAll('input, textarea');
            inputs.forEach(input => {
                input.addEventListener('blur', function() {
                    validateField(this);
                });

                input.addEventListener('input', function() {
                    // Limpar erros enquanto digita
                    clearFieldError(this);
                });
            });
        }

        function validateForm() {
            let isValid = true;
            const requiredFields = contactForm.querySelectorAll('[required]');

            requiredFields.forEach(field => {
                if (!validateField(field)) {
                    isValid = false;
                }
            });

            return isValid;
        }

        function validateField(field) {
            const value = field.value.trim();
            const fieldName = field.name;
            let errorMessage = '';

            // Limpar erro anterior
            clearFieldError(field);

            // Validação por tipo de campo
            switch (fieldName) {
                case 'name':
                    if (!value) {
                        errorMessage = 'Nome é obrigatório';
                    } else if (value.length < 2) {
                        errorMessage = 'Nome deve ter pelo menos 2 caracteres';
                    }
                    break;

                case 'email':
                    if (!value) {
                        errorMessage = 'E-mail é obrigatório';
                    } else if (!isValidEmail(value)) {
                        errorMessage = 'E-mail inválido';
                    }
                    break;

                case 'message':
                    if (!value) {
                        errorMessage = 'Mensagem é obrigatória';
                    } else if (value.length < 10) {
                        errorMessage = 'Mensagem deve ter pelo menos 10 caracteres';
                    }
                    break;
            }

            if (errorMessage) {
                showFieldError(field, errorMessage);
                return false;
            }

            return true;
        }

        function isValidEmail(email) {
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            return emailRegex.test(email);
        }

        function showFieldError(field, message) {
            const errorElement = document.getElementById(field.name + '-error');
            if (errorElement) {
                errorElement.textContent = message;
                errorElement.style.color = '#ef4444';
                errorElement.style.fontSize = '0.875rem';
                errorElement.style.marginTop = '0.25rem';
            }
            
            field.style.borderColor = '#ef4444';
            field.setAttribute('aria-invalid', 'true');
        }

        function clearFieldError(field) {
            const errorElement = document.getElementById(field.name + '-error');
            if (errorElement) {
                errorElement.textContent = '';
            }
            
            field.style.borderColor = '';
            field.removeAttribute('aria-invalid');
        }

        function clearFormErrors() {
            const errorElements = contactForm.querySelectorAll('.error-message');
            errorElements.forEach(element => {
                element.textContent = '';
            });

            const inputs = contactForm.querySelectorAll('input, textarea');
            inputs.forEach(input => {
                input.style.borderColor = '';
                input.removeAttribute('aria-invalid');
            });
        }

        function showFormSuccess() {
            // Criar elemento de sucesso temporário
            const successMessage = document.createElement('div');
            successMessage.textContent = 'Mensagem enviada com sucesso! Em breve entraremos em contato.';
            successMessage.style.cssText = `
                position: fixed;
                top: 20px;
                right: 20px;
                background: #10b981;
                color: white;
                padding: 1rem 1.5rem;
                border-radius: 8px;
                box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1);
                z-index: 3000;
                font-weight: 500;
                animation: slideInRight 0.3s ease-out;
            `;

            document.body.appendChild(successMessage);

            // Remover após 5 segundos
            setTimeout(() => {
                successMessage.style.animation = 'slideOutRight 0.3s ease-out';
                setTimeout(() => {
                    document.body.removeChild(successMessage);
                }, 300);
            }, 5000);
        }

        // ========== ANIMAÇÕES DE SCROLL ==========
        function setupScrollAnimations() {
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };

            const observer = new IntersectionObserver(function(entries) {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            }, observerOptions);

            // Observar elementos para animação
            const animatedElements = document.querySelectorAll(
                '.portfolio-card, .plan-card, .contact-item'
            );
            
            animatedElements.forEach(element => {
                element.classList.add('fade-in');
                observer.observe(element);
            });
        }

        // ========== CARREGAMENTO LAZY DE IMAGENS ==========
        function setupLazyLoading() {
            const images = document.querySelectorAll('img[loading="lazy"]');
            
            const imageObserver = new IntersectionObserver(function(entries) {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        const img = entry.target;
                        
                        img.addEventListener('load', function() {
                            img.classList.add('loaded');
                        });

                        // Se a imagem já foi carregada
                        if (img.complete) {
                            img.classList.add('loaded');
                        }

                        imageObserver.unobserve(img);
                    }
                });
            });

            images.forEach(img => {
                imageObserver.observe(img);
            });
        }

        // ========== NAVEGAÇÃO POR TECLADO ==========
        function setupKeyboardNavigation() {
            // Melhorar navegação por Tab
            const focusableElements = document.querySelectorAll(
                'a, button, input, textarea, select, [tabindex]:not([tabindex="-1"])'
            );

            // Adicionar indicadores visuais de foco personalizados
            focusableElements.forEach(element => {
                element.addEventListener('focus', function() {
                    this.style.outline = '2px solid var(--primary)';
                    this.style.outlineOffset = '2px';
                });

                element.addEventListener('blur', function() {
                    this.style.outline = '';
                    this.style.outlineOffset = '';
                });
            });

            // Navegação por teclado nos cards de portfólio
            portfolioCards.forEach((card, index) => {
                card.addEventListener('keydown', function(e) {
                    switch (e.key) {
                        case 'ArrowRight':
                        case 'ArrowDown':
                            e.preventDefault();
                            const nextCard = portfolioCards[index + 1] || portfolioCards[0];
                            nextCard.focus();
                            break;

                        case 'ArrowLeft':
                        case 'ArrowUp':
                            e.preventDefault();
                            const prevCard = portfolioCards[index - 1] || portfolioCards[portfolioCards.length - 1];
                            prevCard.focus();
                            break;
                    }
                });
            });
        }

        // ========== UTILITÁRIOS ==========
        
        // Debounce para otimizar eventos de scroll
        function debounce(func, wait) {
            let timeout;
            return function executedFunction(...args) {
                const later = () => {
                    clearTimeout(timeout);
                    func(...args);
                };
                clearTimeout(timeout);
                timeout = setTimeout(later, wait);
            };
        }

        // Otimizar evento de scroll
        window.addEventListener('scroll', debounce(handleScroll, 10));

        // ========== ANIMAÇÕES CSS ADICIONAIS ==========
        const style = document.createElement('style');
        style.textContent = `
            @keyframes slideInRight {
                from {
                    transform: translateX(100%);
                    opacity: 0;
                }
                to {
                    transform: translateX(0);
                    opacity: 1;
                }
            }

            @keyframes slideOutRight {
                from {
                    transform: translateX(0);
                    opacity: 1;
                }
                to {
                    transform: translateX(100%);
                    opacity: 0;
                }
            }

            .error-message {
                display: block;
                min-height: 1.25rem;
                transition: all 0.3s ease;
            }

            /* Melhor indicação de foco */
            *:focus-visible {
                outline: 2px solid var(--primary) !important;
                outline-offset: 2px !important;
            }

            /* Animação suave para mudança de tema */
            * {
                transition: background-color 0.3s ease, 
                           color 0.3s ease, 
                           border-color 0.3s ease;
            }

            /* Estados de hover mais suaves */
            .portfolio-card:hover {
                transform: translateY(-8px) scale(1.02);
            }

            .plan-card:hover {
                transform: translateY(-8px) scale(1.02);
            }

            /* Indicador de carregamento para imagens */
            img[loading="lazy"]:not(.loaded) {
                background: linear-gradient(90deg, 
                    var(--bg-secondary) 25%, 
                    var(--border) 50%, 
                    var(--bg-secondary) 75%);
                background-size: 200% 100%;
                animation: loading 1.5s infinite;
            }

            @keyframes loading {
                0% { background-position: 200% 0; }
                100% { background-position: -200% 0; }
            }

            /* Melhor responsividade para tablets */
            @media (max-width: 1024px) and (min-width: 769px) {
                .portfolio-grid {
                    grid-template-columns: repeat(2, 1fr);
                }
                
                .plans-grid {
                    grid-template-columns: repeat(2, 1fr);
                }
                
                .plan-card.featured {
                    transform: translateY(-20px);
                }
            }

            /* Animações mais suaves para elementos interativos */
            .btn, .portfolio-card, .plan-card, .contact-item {
                transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            }

            /* Melhor legibilidade no modo escuro */
            [data-theme="dark"] .hero-title {
                background: linear-gradient(135deg, #818cf8, #06b6d4);
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
                background-clip: text;
            }

            /* Scroll bar personalizada */
            ::-webkit-scrollbar {
                width: 8px;
            }

            ::-webkit-scrollbar-track {
                background: var(--bg-secondary);
            }

            ::-webkit-scrollbar-thumb {
                background: var(--primary);
                border-radius: 4px;
            }

            ::-webkit-scrollbar-thumb:hover {
                background: var(--primary-dark);
            }
        `;
        
        document.head.appendChild(style);

        // ========== PERFORMANCE E SEO ==========
        
        // Preload de imagens críticas
        function preloadCriticalImages() {
            const criticalImages = [
                'https://picsum.photos/400/250?random=1',
                'https://picsum.photos/400/250?random=2',
                'https://picsum.photos/400/250?random=3'
            ];

            criticalImages.forEach(src => {
                const link = document.createElement('link');
                link.rel = 'preload';
                link.as = 'image';
                link.href = src;
                document.head.appendChild(link);
            });
        }

        // Chamar preload após carregamento da página
        window.addEventListener('load', preloadCriticalImages);

        // ========== ANALYTICS E TRACKING (PLACEHOLDER) ==========
        
        // Placeholder para Google Analytics ou outras ferramentas
        function trackEvent(action, category, label) {
            // Implementar tracking de eventos aqui
            console.log('Track Event:', { action, category, label });
        }

        // Rastrear cliques em portfólio
        portfolioCards.forEach((card, index) => {
            card.addEventListener('click', () => {
                trackEvent('portfolio_click', 'engagement', `portfolio_${index + 1}`);
            });
        });

        // Rastrear cliques em planos
        document.querySelectorAll('.plan-card .btn').forEach((btn, index) => {
            btn.addEventListener('click', () => {
                trackEvent('plan_click', 'conversion', `plan_${index + 1}`);
            });
        });

        // Rastrear envio de formulário
        if (contactForm) {
            contactForm.addEventListener('submit', () => {
                trackEvent('form_submit', 'lead', 'contact_form');
            });
        }

        console.log('🎨 Impressione Designs - Site carregado com sucesso!');
    </script>
</body>
</html>
