<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>LAURO VAZ DESPACHANTE | 45 anos de experiência</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        html, body {
            width: 100%;
            overflow-x: hidden;
        }
        
        body {
            background-color: #fffef7;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 100%;
            width: 100%;
            padding: 0 15px;
            margin: 0 auto;
        }
        
        /* Header */
        header {
            background: linear-gradient(135deg, #e6b400, #ffcc00);
            color: #333;
            padding: 12px 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
            width: 100%;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            width: 100%;
        }
        
        .logo {
            display: flex;
            align-items: center;
            flex-shrink: 0;
        }
        
        .logo h1 {
            font-size: 1.2rem;
            margin-left: 8px;
            white-space: nowrap;
        }
        
        .logo-icon {
            font-size: 1.5rem;
            color: #333;
        }
        
        /* Menu mobile */
        .menu-toggle {
            display: block;
            flex-direction: column;
            cursor: pointer;
            background: transparent;
            border: none;
            padding: 5px;
        }
        
        .menu-toggle span {
            height: 2px;
            width: 20px;
            background: #333;
            margin-bottom: 4px;
            border-radius: 2px;
            transition: all 0.3s;
            display: block;
        }
        
        nav {
            width: 100%;
            display: none;
        }
        
        nav.active {
            display: block;
        }
        
        nav ul {
            display: flex;
            flex-direction: column;
            list-style: none;
            width: 100%;
            background: #ffcc00;
            margin-top: 10px;
            border-radius: 5px;
            padding: 10px 0;
        }
        
        nav ul li {
            margin: 0;
            text-align: center;
            width: 100%;
        }
        
        nav ul li a {
            color: #333;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9rem;
            transition: color 0.3s;
            display: block;
            padding: 8px 15px;
            width: 100%;
        }
        
        nav ul li a:hover {
            color: #fff;
            background: #e6b400;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://images.unsplash.com/photo-1603712610494-73e22f155c0e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 40px 15px;
            width: 100%;
        }
        
        .hero-content {
            width: 100%;
            max-width: 100%;
        }
        
        .hero h2 {
            font-size: 1.6rem;
            margin-bottom: 15px;
            line-height: 1.3;
        }
        
        .hero p {
            font-size: 0.95rem;
            margin: 0 auto 20px;
            max-width: 100%;
        }
        
        .experience-badge {
            background-color: #ffcc00;
            color: #333;
            display: inline-block;
            padding: 8px 15px;
            border-radius: 20px;
            font-weight: bold;
            margin-bottom: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            font-size: 0.9rem;
            width: 100%;
            max-width: 100%;
            box-sizing: border-box;
        }
        
        .btn {
            display: inline-block;
            background-color: #333;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: background-color 0.3s;
            margin: 8px 5px;
            font-size: 0.9rem;
            width: 90%;
            max-width: 200px;
        }
        
        .btn:hover {
            background-color: #555;
        }
        
        /* Services */
        .services {
            padding: 40px 0;
            background-color: white;
            width: 100%;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 30px;
            width: 100%;
            padding: 0 10px;
        }
        
        .section-title h2 {
            font-size: 1.6rem;
            color: #333;
            margin-bottom: 10px;
        }
        
        .section-title p {
            color: #666;
            max-width: 100%;
            margin: 0 auto;
            font-size: 0.9rem;
        }
        
        .services-grid {
            display: flex;
            flex-direction: column;
            gap: 15px;
            width: 100%;
        }
        
        .service-card {
            background-color: #fffef7;
            border-radius: 8px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
            border: 1px solid #ffcc00;
            width: 100%;
            box-sizing: border-box;
        }
        
        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(230, 180, 0, 0.2);
        }
        
        .service-icon {
            font-size: 1.8rem;
            color: #333;
            margin-bottom: 12px;
        }
        
        .service-card h3 {
            font-size: 1.1rem;
            margin-bottom: 8px;
            color: #333;
        }
        
        .service-card p {
            font-size: 0.85rem;
        }
        
        /* About */
        .about {
            padding: 40px 0;
            background-color: #fffef7;
            width: 100%;
        }
        
        .about-content {
            display: flex;
            flex-direction: column;
            gap: 20px;
            width: 100%;
        }
        
        .about-text {
            width: 100%;
        }
        
        .about-text h2 {
            font-size: 1.6rem;
            color: #333;
            margin-bottom: 15px;
        }
        
        .about-text p {
            font-size: 0.9rem;
            margin-bottom: 15px;
        }
        
        .about-image {
            width: 100%;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 8px;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
        }
        
        /* Importance Section */
        .importance {
            padding: 40px 0;
            background: linear-gradient(135deg, #e6b400, #ffcc00);
            color: #333;
            width: 100%;
        }
        
        .importance-content {
            display: flex;
            flex-direction: column;
            gap: 20px;
            width: 100%;
        }
        
        .importance-text {
            width: 100%;
        }
        
        .importance-text h2 {
            font-size: 1.6rem;
            margin-bottom: 15px;
            color: #333;
        }
        
        .importance-text p {
            font-size: 0.9rem;
            margin-bottom: 15px;
        }
        
        .importance-list {
            width: 100%;
        }
        
        .importance-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 15px;
        }
        
        .importance-icon {
            font-size: 1.2rem;
            color: #333;
            margin-right: 12px;
            margin-top: 3px;
            flex-shrink: 0;
        }
        
        .importance-item div h3 {
            font-size: 1.1rem;
            margin-bottom: 5px;
        }
        
        .importance-item div p {
            font-size: 0.85rem;
        }
        
        /* Contact */
        .contact {
            padding: 40px 0;
            background-color: white;
            width: 100%;
        }
        
        .contact-grid {
            display: flex;
            flex-direction: column;
            gap: 15px;
            width: 100%;
        }
        
        .contact-card {
            background-color: #fffef7;
            border-radius: 8px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.05);
            border: 1px solid #ffcc00;
            width: 100%;
            box-sizing: border-box;
        }
        
        .contact-icon {
            font-size: 1.8rem;
            color: #333;
            margin-bottom: 12px;
        }
        
        .contact-card h3 {
            font-size: 1.1rem;
            margin-bottom: 8px;
            color: #333;
        }
        
        .contact-card p {
            font-size: 0.9rem;
            margin-bottom: 10px;
        }
        
        .whatsapp-btn {
            display: inline-block;
            background-color: #25D366;
            color: white;
            padding: 8px 16px;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            margin-top: 10px;
            transition: background-color 0.3s;
            font-size: 0.9rem;
        }
        
        .whatsapp-btn:hover {
            background-color: #128C7E;
        }
        
        /* Footer */
        footer {
            background-color: #333;
            color: white;
            padding: 25px 0 12px;
            text-align: center;
            width: 100%;
        }
        
        .footer-content {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-bottom: 20px;
            width: 100%;
        }
        
        .footer-section {
            width: 100%;
        }
        
        .footer-section h3 {
            font-size: 1.1rem;
            margin-bottom: 12px;
            color: #ffcc00;
        }
        
        .footer-section p {
            font-size: 0.9rem;
        }
        
        .social-links {
            margin-top: 10px;
        }
        
        .social-links a {
            display: inline-block;
            color: white;
            font-size: 1.2rem;
            margin: 0 8px;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: #ffcc00;
        }
        
        .copyright {
            margin-top: 20px;
            padding-top: 12px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.85rem;
        }
        
        /* Media Query para telas maiores */
        @media (min-width: 768px) {
            .container {
                max-width: 720px;
                padding: 0 15px;
            }
            
            .header-content {
                flex-wrap: nowrap;
            }
            
            .menu-toggle {
                display: none;
            }
            
            nav {
                display: block;
                width: auto;
            }
            
            nav ul {
                flex-direction: row;
                background: transparent;
                margin-top: 0;
                padding: 0;
                width: auto;
            }
            
            nav ul li {
                width: auto;
            }
            
            nav ul li a {
                padding: 5px 10px;
                width: auto;
            }
            
            .hero {
                padding: 80px 15px;
            }
            
            .hero h2 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1.1rem;
            }
            
            .experience-badge {
                font-size: 1rem;
                padding: 10px 20px;
                width: auto;
            }
            
            .btn {
                width: auto;
            }
            
            .services-grid {
                flex-direction: row;
                flex-wrap: wrap;
            }
            
            .service-card {
                width: calc(50% - 10px);
            }
            
            .about-content {
                flex-direction: row;
            }
            
            .about-text, .about-image {
                width: 50%;
            }
            
            .importance-content {
                flex-direction: row;
            }
            
            .importance-text, .importance-list {
                width: 50%;
            }
            
            .contact-grid {
                flex-direction: row;
                flex-wrap: wrap;
            }
            
            .contact-card {
                width: calc(50% - 10px);
            }
            
            .footer-content {
                flex-direction: row;
            }
            
            .footer-section {
                width: 33.33%;
                padding: 0 10px;
            }
        }
        
        @media (min-width: 992px) {
            .container {
                max-width: 960px;
            }
            
            .service-card {
                width: calc(33.333% - 15px);
            }
            
            .contact-card {
                width: calc(33.333% - 15px);
            }
            
            nav ul li {
                margin-left: 15px;
            }
            
            nav ul li a {
                padding: 5px 15px;
            }
        }
        
        @media (min-width: 1200px) {
            .container {
                max-width: 1140px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-content">
            <div class="logo">
                <i class="fas fa-car logo-icon"></i>
                <h1>LAURO VAZ DESPACHANTE</h1>
            </div>
            <button class="menu-toggle" id="mobile-menu">
                <span></span>
                <span></span>
                <span></span>
            </button>
            <nav id="main-nav">
                <ul>
                    <li><a href="#services">Serviços</a></li>
                    <li><a href="#importance">Importância</a></li>
                    <li><a href="#about">Sobre</a></li>
                    <li><a href="#contact">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container hero-content">
            <div class="experience-badge">
                <i class="fas fa-award"></i> Lauro Vaz e Ednelza Medeiros - 45 anos de experiência e comprometimento!
            </div>
            <h2>Soluções completas para seus documentos veiculares</h2>
            <p>Oferecemos serviços especializados com agilidade, segurança e preços justos. Atendimento personalizado para facilitar sua vida.</p>
            <a href="#contact" class="btn">Fale Conosco</a>
            <a href="#services" class="btn">Nossos Serviços</a>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Nossos Serviços</h2>
                <p>Oferecemos uma gama completa de serviços para atender todas as suas necessidades documentais veiculares</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-car-side"></i>
                    </div>
                    <h3>ATPV</h3>
                    <p>Autorização para Transferência de Propriedade de Veículo</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-id-card"></i>
                    </div>
                    <h3>Emplacamento</h3>
                    <p>Processo completo de emplacamento do seu veículo</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-file-alt"></i>
                    </div>
                    <h3>Licenciamento</h3>
                    <p>Regularização do licenciamento anual do seu veículo</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-exchange-alt"></i>
                    </div>
                    <h3>Transferência</h3>
                    <p>Transferência de propriedade de veículos</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-money-bill-wave"></i>
                    </div>
                    <h3>Baixa Tributária</h3>
                    <p>Processamento de baixa tributária de veículos</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-copy"></i>
                    </div>
                    <h3>2ª Via de DUT/CRV</h3>
                    <p>Emissão de segunda via de documentos veiculares</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-map-marked-alt"></i>
                    </div>
                    <h3>Mudança de UF/Município</h3>
                    <p>Alteração de endereço entre unidades federativas ou municípios</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-id-badge"></i>
                    </div>
                    <h3>Renovação de CNH</h3>
                    <p>Renovação da Carteira Nacional de Habilitação</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-cog"></i>
                    </div>
                    <h3>Remarcação de Chassi/Motor</h3>
                    <p>Serviço especializado de remarcação</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-gavel"></i>
                    </div>
                    <h3>Veículos de Leilão</h3>
                    <p>Regularização de veículos adquiridos em leilão</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-unlock"></i>
                    </div>
                    <h3>Liberação de Veículos</h3>
                    <p>Liberação de veículos apreendidos ou com restrições</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Importance Section -->
    <section class="importance" id="importance">
        <div class="container">
            <div class="section-title">
                <h2>Importância de Manter Seu Veículo em Dia</h2>
                <p>Documentação regularizada evita problemas e garante sua tranquilidade</p>
            </div>
            <div class="importance-content">
                <div class="importance-text">
                    <h2>Por que é essencial regularizar sua situação?</h2>
                    <p>Manter a documentação do seu veículo em dia não é apenas uma obrigação legal, mas também uma forma de proteger seu patrimônio e garantir sua liberdade de locomoção sem preocupações.</p>
                    <p>Veículos com documentação irregular podem causar transtornos como multas, apreensões e dificuldades na venda ou transferência.</p>
                </div>
                <div class="importance-list">
                    <div class="importance-item">
                        <div class="importance-icon">
                            <i class="fas fa-shield-alt"></i>
                        </div>
                        <div>
                            <h3>Proteção Legal</h3>
                            <p>Evite multas, penalidades e apreensões do veículo</p>
                        </div>
                    </div>
                    <div class="importance-item">
                        <div class="importance-icon">
                            <i class="fas fa-lock"></i>
                        </div>
                        <div>
                            <h3>Segurança Patrimonial</h3>
                            <p>Proteja seu investimento e valor de revenda</p>
                        </div>
                    </div>
                    <div class="importance-item">
                        <div class="importance-icon">
                            <i class="fas fa-truck-loading"></i>
                        </div>
                        <div>
                            <h3>Mobilidade Garantida</h3>
                            <p>Circule sem preocupações por qualquer via do país</p>
                        </div>
                    </div>
                    <div class="importance-item">
                        <div class="importance-icon">
                            <i class="fas fa-handshake"></i>
                        </div>
                        <div>
                            <h3>Facilidade na Transferência</h3>
                            <p>Documentos em dia facilitam a venda do veículo</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2>45 Anos de Experiência e Comprometimento</h2>
                    <p>Lauro Vaz e Ednelza Medeiros são referência em serviços de despachante documentalista em Manaus e região. Com mais de quatro décadas de atuação no mercado, oferecemos serviços especializados com agilidade, transparência e preços justos.</p>
                    <p>Nossa missão é simplificar os processos burocráticos relacionados a veículos, proporcionando tranquilidade e segurança para nossos clientes. Trabalhamos com ética, profissionalismo e dedicação para superar expectativas.</p>
                    <p>Venha conhecer nosso atendimento personalizado e comprove a qualidade dos nossos serviços!</p>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1580273916550-e323be2ae537?ixlib=rb-4.0.3&auto=format&fit=crop&w=700&q=80" alt="Escritório Lauro Vaz Despachante">
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Entre em Contato</h2>
                <p>Estamos à disposição para esclarecer dúvidas e oferecer o melhor atendimento</p>
            </div>
            <div class="contact-grid">
                <div class="contact-card">
                    <div class="contact-icon">
                        <i class="fas fa-map-marker-alt"></i>
                    </div>
                    <h3>Endereço</h3>
                    <p>Travessa São Judas Tadeu, 175A<br>Adrianópolis, Manaus - AM</p>
                </div>
                <div class="contact-card">
                    <div class="contact-icon">
                        <i class="fab fa-whatsapp"></i>
                    </div>
                    <h3>WhatsApp</h3>
                    <p>(92) 99368-7009</p>
                    <a href="https://wa.me/5592993687009" class="whatsapp-btn">
                        <i class="fab fa-whatsapp"></i> Enviar Mensagem
                    </a>
                </div>
                <div class="contact-card">
                    <div class="contact-icon">
                        <i class="far fa-clock"></i>
                    </div>
                    <h3>Horário de Funcionamento</h3>
                    <p>Segunda a Sexta: 8h às 15:30h</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>LAURO VAZ DESPACHANTE</h3>
                    <p>Soluções documentais veiculares com excelência há 45 anos.</p>
                </div>
                <div class="footer-section">
                    <h3>Horário de Atendimento</h3>
                    <p>Segunda a Sexta: 8h às 15:30h</p>
                </div>
                <div class="footer-section">
                    <h3>Redes Sociais</h3>
                    <div class="social-links">
                        <a href="https://www.instagram.com/laurovazdespachante" target="_blank">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#"><i class="fab fa-facebook"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                    </div>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2025 LAURO VAZ DESPACHANTE - Todos os direitos reservados</p>
            </div>
        </div>
    </footer>

    <script>
        // Menu mobile toggle
        document.getElementById('mobile-menu').addEventListener('click', function() {
            document.getElementById('main-nav').classList.toggle('active');
        });
        
        // Fechar menu ao clicar em um link
        document.querySelectorAll('nav a').forEach(link => {
            link.addEventListener('click', function() {
                document.getElementById('main-nav').classList.remove('active');
            });
        });
        
        // Smooth scroll para links internos
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 70,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
