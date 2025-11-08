Certo\! Aqui está o código HTML atualizado.

Eu identifiquei a seção `<section class="funnel">` e, dentro da `div class="funnel-stages"`, mantive os 4 estágios originais e adicionei mais 5, totalizando 9 soluções, conforme solicitado.

Os novos estágios adicionados são:

  * **05: Advocacia (Indicação)**
  * **06: Aumento de Valor (Upsell)**
  * **07: Remarketing Estratégico**
  * **08: Análise de Dados**
  * **09: Otimização Contínua**

<!-- end list -->

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gestão de Tráfego Pago - Transforme Seu Negócio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            overflow-x: hidden;
        }

        .hero {
            background: linear-gradient(135deg, #1a1a1a 0%, #0d4d0d 100%);
            color: white;
            padding: 60px 20px 100px 20px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .logo-container {
            margin-bottom: 30px;
        }

        .logo {
            width: 120px;
            height: auto;
            filter: drop-shadow(0 5px 15px rgba(168, 255, 0, 0.3));
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg width="100" height="100" xmlns="http://www.w3.org/2000/svg"><circle cx="50" cy="50" r="2" fill="%23a8ff00" opacity="0.1"/></svg>');
            animation: float 20s linear infinite;
        }

        @keyframes float {
            0% { transform: translateY(0); }
            100% { transform: translateY(-100px); }
        }

        .hero h1 {
            font-size: 3.5em;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            position: relative;
            z-index: 1;
            background: linear-gradient(135deg, #a8ff00, #7cd400);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero p {
            font-size: 1.5em;
            margin-bottom: 30px;
            position: relative;
            z-index: 1;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .problems {
            background: #f8f9fa;
            padding: 80px 20px;
            text-align: center;
        }

        .problems h2 {
            font-size: 2.5em;
            margin-bottom: 50px;
            color: #2d3748;
        }

        .problem-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .problem-card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .problem-card:hover {
            transform: translateY(-10px);
        }

        .problem-card::before {
            content: '❌';
            font-size: 3em;
            display: block;
            margin-bottom: 15px;
        }

        .solution {
            padding: 80px 20px;
            text-align: center;
            background: linear-gradient(to bottom, white, #f8f9fa);
        }

        .solution h2 {
            font-size: 2.5em;
            margin-bottom: 30px;
            color: #2d3748;
        }

        .solution-text {
            font-size: 1.3em;
            max-width: 800px;
            margin: 0 auto;
            color: #4a5568;
        }

        .funnel {
            padding: 80px 20px;
            background: white;
        }

        .funnel h2 {
            text-align: center;
            font-size: 2.5em;
            margin-bottom: 60px;
            color: #2d3748;
        }

        .funnel-stages {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .stage {
            background: linear-gradient(135deg, #e8ffe8 0%, #d4ffd4 100%);
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(168, 255, 0, 0.15);
            transition: all 0.3s;
            position: relative;
        }

        .stage:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 40px rgba(168, 255, 0, 0.25);
        }

        .stage-number {
            position: absolute;
            top: -20px;
            left: 20px;
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, #a8ff00, #7cd400);
            color: #1a1a1a;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5em;
            font-weight: bold;
            box-shadow: 0 5px 15px rgba(168, 255, 0, 0.3);
        }

        .stage h3 {
            font-size: 1.5em;
            margin: 20px 0 15px 0;
            color: #2d3748;
        }

        .stage .emoji {
            font-size: 2em;
        }

        .stage p {
            margin: 10px 0;
            color: #4a5568;
        }

        .pricing {
            padding: 80px 20px;
            background: #f8f9fa;
        }

        .pricing h2 {
            text-align: center;
            font-size: 2.5em;
            margin-bottom: 30px;
            color: #2d3748;
        }

        .pricing-subtitle {
            text-align: center;
            font-size: 1.2em;
            color: #4a5568;
            margin-bottom: 60px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            max-width: 1400px;
            margin: 0 auto;
        }

        .plan {
            background: white;
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.1);
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }

        .plan::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
            background: linear-gradient(90deg, #a8ff00, #7cd400);
        }

        .plan:hover {
            transform: translateY(-15px);
            box-shadow: 0 20px 50px rgba(168, 255, 0, 0.2);
        }

        .plan.featured {
            border: 3px solid #a8ff00;
            transform: scale(1.05);
            box-shadow: 0 15px 50px rgba(168, 255, 0, 0.3);
        }

        .plan.featured .badge {
            position: absolute;
            top: 20px;
            right: -35px;
            background: #a8ff00;
            color: #333;
            padding: 5px 40px;
            transform: rotate(45deg);
            font-weight: bold;
            font-size: 0.9em;
        }

        .plan-header {
            text-align: center;
            margin-bottom: 30px;
        }

        .plan-name {
            font-size: 2em;
            font-weight: bold;
            margin-bottom: 15px;
            color: #2d3748;
        }

        .plan-icon {
            font-size: 3em;
            margin-bottom: 15px;
        }

        .plan-price {
            font-size: 3em;
            font-weight: bold;
            color: #7cd400;
            margin: 20px 0;
        }

        .plan-price span {
            font-size: 0.4em;
            color: #4a5568;
        }

        .plan-features {
            list-style: none;
            margin: 30px 0;
        }

        .plan-features li {
            padding: 12px 0;
            border-bottom: 1px solid #e2e8f0;
            text-align: left;
            color: #4a5568;
            font-size: 0.95em;
        }

        .plan-features li::before {
            content: '✓';
            color: #a8ff00;
            font-weight: bold;
            margin-right: 10px;
        }

        .section-title {
            font-weight: bold;
            color: #2d3748;
            font-size: 1.1em;
            margin-top: 20px;
        }

        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, #a8ff00 0%, #7cd400 100%);
            color: #1a1a1a;
            padding: 15px 40px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1em;
            transition: all 0.3s;
            box-shadow: 0 5px 15px rgba(168, 255, 0, 0.3);
            margin-top: 20px;
        }

        .cta-button:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 25px rgba(168, 255, 0, 0.5);
        }

        .results {
            padding: 80px 20px;
            background: linear-gradient(135deg, #1a1a1a 0%, #0d4d0d 100%);
            color: white;
            text-align: center;
        }

        .results h2 {
            font-size: 2.5em;
            margin-bottom: 50px;
        }

        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            max-width: 1000px;
            margin: 0 auto;
        }

        .stat {
            background: rgba(255,255,255,0.1);
            padding: 30px;
            border-radius: 15px;
            backdrop-filter: blur(10px);
        }

        .stat-number {
            font-size: 3em;
            font-weight: bold;
            margin-bottom: 10px;
        }

        .stat-label {
            font-size: 1.2em;
        }

        .cta-final {
            padding: 80px 20px;
            text-align: center;
            background: #2d3748;
            color: white;
        }

        .cta-final h2 {
            font-size: 2.5em;
            margin-bottom: 30px;
        }

        .cta-final p {
            font-size: 1.3em;
            margin-bottom: 40px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        .enterprise-section {
            background: linear-gradient(135deg, #1a1a1a 0%, #0d4d0d 100%);
            padding: 80px 20px;
            color: white;
        }

        .enterprise-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: start;
        }

        .enterprise-form {
            background: rgba(255, 255, 255, 0.05);
            padding: 40px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 2px solid rgba(168, 255, 0, 0.2);
        }

        .enterprise-form h3 {
            font-size: 2em;
            margin-bottom: 30px;
            color: #a8ff00;
        }

        .form-group {
            margin-bottom: 25px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: #a8ff00;
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 12px 15px;
            border: 2px solid rgba(168, 255, 0, 0.3);
            border-radius: 10px;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 1em;
            transition: all 0.3s;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #a8ff00;
            background: rgba(255, 255, 255, 0.15);
        }

        .form-group textarea {
            min-height: 120px;
            resize: vertical;
        }

        .checkbox-group {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .checkbox-item {
            display: flex;
            align-items: center;
            gap: 10px;
            padding: 12px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.3s;
        }

        .checkbox-item:hover {
            background: rgba(168, 255, 0, 0.1);
        }

        .checkbox-item input[type="checkbox"] {
            width: 20px;
            height: 20px;
            cursor: pointer;
            accent-color: #a8ff00;
        }

        .checkbox-item label {
            margin: 0;
            cursor: pointer;
            color: white;
        }

        .enterprise-preview {
            position: sticky;
            top: 100px;
            background: rgba(255, 255, 255, 0.05);
            padding: 40px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            border: 2px solid rgba(168, 255, 0, 0.2);
        }

        .enterprise-preview h3 {
            font-size: 2em;
            margin-bottom: 20px;
            color: #a8ff00;
        }

        .preview-content {
            margin-top: 20px;
        }

        .preview-section {
            margin-bottom: 25px;
            padding-bottom: 25px;
            border-bottom: 1px solid rgba(168, 255, 0, 0.2);
        }

        .preview-section:last-child {
            border-bottom: none;
        }

        .preview-section h4 {
            color: #a8ff00;
            margin-bottom: 10px;
            font-size: 1.2em;
        }

        .preview-section ul {
            list-style: none;
            padding-left: 0;
        }

        .preview-section li {
            padding: 5px 0;
            color: #e0e0e0;
        }

        .preview-section li::before {
            content: '✓';
            color: #a8ff00;
            margin-right: 10px;
            font-weight: bold;
        }

        .preview-price {
            font-size: 2.5em;
            color: #a8ff00;
            font-weight: bold;
            margin: 20px 0;
            text-align: center;
        }

        .preview-note {
            background: rgba(168, 255, 0, 0.1);
            padding: 15px;
            border-radius: 10px;
            margin-top: 20px;
            font-size: 0.9em;
            color: #e0e0e0;
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2em;
            }

            .hero p {
                font-size: 1.2em;
            }

            .plan.featured {
                transform: scale(1);
            }

            .pricing-grid {
                gap: 30px;
            }

            .enterprise-content {
                grid-template-columns: 1fr;
                gap: 30px;
            }

            .enterprise-preview {
                position: static;
            }
        }
    </style>
</head>
<body>
    <section class="hero">
        <div class="logo-container">
            <img src="https://i.ibb.co/svdJg9Dp/Design-sem-nome.png" alt="Logo R9" class="logo">
        </div>
        <h1>🚀 Transforme Seu Negócio com Tráfego Pago</h1>
        <p>Resultados reais, clientes reais, crescimento previsível</p>
    </section>

    <section class="problems">
        <div class="container">
            <h2>O que acontece com a maioria dos negócios hoje?</h2>
            <div class="problem-grid">
                <div class="problem-card">
                    <h3>Gastam com anúncios sem retorno real</h3>
                </div>
                <div class="problem-card">
                    <h3>Não sabem de onde vêm os clientes</h3>
                </div>
                <div class="problem-card">
                    <h3>Perdem tempo em processos manuais</h3>
                </div>
                <div class="problem-card">
                    <h3>Crescem sem previsibilidade</h3>
                </div>
            </div>
        </div>
    </section>

    <section class="solution">
        <div class="container">
            <h2>📍 A Solução</h2>
            <p class="solution-text">
                Posicione sua empresa como um <strong>outdoor bem localizado em uma avenida movimentada</strong>. 
                Com estratégias de tráfego pago, você atinge exatamente quem precisa dos seus serviços, 
                no momento certo, com a mensagem certa.
            </p>
        </div>
    </section>

    <section class="funnel">
        <div class="container">
            <h2>🎯 Funil de Estratégia Completo</h2>
            <div class="funnel-stages">
                <div class="stage">
                    <div class="stage-number">01</div>
                    <div class="emoji">👁️</div>
                    <h3>Reconhecimento de Marca</h3>
                    <p><strong>Objetivo:</strong> Mostrar seu negócio para quem ainda não conhece</p>
                    <p><em>"Quem é, onde fica, que vibe é essa?"</em></p>
                </div>

                <div class="stage">
                    <div class="stage-number">02</div>
                    <div class="emoji">💬</div>
                    <h3>Engajamento</h3>
                    <p><strong>Objetivo:</strong> Gerar afinidade e conversa</p>
                    <p><em>"Eu gosto desse lugar, parece minha vibe."</em></p>
                </div>

                <div class="stage">
                    <div class="stage-number">03</div>
                    <div class="emoji">🎯</div>
                    <h3>Conversão</h3>
                    <p><strong>Objetivo:</strong> Trazer o público para seu negócio</p>
                    <p><em>"Quero ir lá!"</em></p>
                </div>

                <div class="stage">
                    <div class="stage-number">04</div>
                    <div class="emoji">🔄</div>
                    <h3>Fidelização</h3>
                    <p><strong>Objetivo:</strong> Fazer o público voltar</p>
                    <p><em>"Esse é meu ponto fixo."</em></p>
                </div>
                
                <div class="stage">
                    <div class="stage-number">05</div>
                    <div class="emoji">📣</div>
                    <h3>Advocacia (Indicação)</h3>
                    <p><strong>Objetivo:</strong> Transformar clientes em promotores da marca</p>
                    <p><em>"Você *tem* que conhecer esse lugar!"</em></p>
                </div>

                <div class="stage">
                    <div class="stage-number">06</div>
                    <div class="emoji">💰</div>
                    <h3>Aumento de Valor (Upsell)</h3>
                    <p><strong>Objetivo:</strong> Aumentar o ticket médio por cliente fidelizado</p>
                    <p><em>"Já que estou aqui, vou levar isso também."</em></p>
                </div>

                <div class="stage">
                    <div class="stage-number">07</div>
                    <div class="emoji">🔁</div>
                    <h3>Remarketing Estratégico</h3>
                    <p><strong>Objetivo:</strong> Reconquistar quem visitou mas não converteu</p>
                    <p><em>"Lembrei daquele produto que eu queria..."</em></p>
                </div>

                <div class="stage">
                    <div class="stage-number">08</div>
                    <div class="emoji">📊</div>
                    <h3>Análise de Dados</h3>
                    <p><strong>Objetivo:</strong> Entender o comportamento e otimizar rotas</p>
                    <p><em>"Os números mostram que o público da 'terça' converte mais."</em></p>
                </div>

                <div class="stage">
                    <div class="stage-number">09</div>
                    <div class="emoji">🧪</div>
                    <h3>Otimização Contínua</h3>
                    <p><strong>Objetivo:</strong> Melhorar o custo por aquisição (CPA) e o ROI</p>
                    <p><em>"Vamos testar o anúncio 'A' contra o 'B'."</em></p>
                </div>
                
                </div>
        </div>
    </section>

    <section class="pricing">
        <div class="container">
            <h2>💎 Escolha Seu Plano</h2>
            <p class="pricing-subtitle">Selecione o plano ideal para o seu negócio. Todos incluem Gestão de Tráfego profissional.</p>
            <div class="pricing-grid">
                <div class="plan">
                    <div class="plan-header">
                        <div class="plan-icon">🎯</div>
                        <div class="plan-name">Starter</div>
                        <div class="plan-price">R$ 990</div>
                    </div>
                    <p style="text-align: center; color: #7cd400; font-weight: bold;">Ideal para quem já tem conteúdo</p>
                    <ul class="plan-features">
                        <li class="section-title">❌ Audio Visual</li>
                        <li style="opacity: 0.6;">Você fornece todo material</li>
                        
                        <li class="section-title">✅ Gestão de Tráfego</li>
                        <li>2 Campanhas</li>
                        <li>3 Dias de Teste</li>
                        <li>10 Dias de Otimizações</li>
                        <li>Suporte via E-mail</li>
                        <li>Relatório Semanal</li>
                    </ul>
                    <center><a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Starter" class="cta-button">Quero o Starter</a></center>
                </div>

                <div class="plan">
                    <div class="plan-header">
                        <div class="plan-icon">📦</div>
                        <div class="plan-name">Inclusive</div>
                        <div class="plan-price">R$ 1.790</div>
                    </div>
                    <p style="text-align: center; color: #7cd400; font-weight: bold;">Para quem quer começar agora</p>
                    <ul class="plan-features">
                        <li class="section-title">❌ Audio Visual</li>
                        <li style="opacity: 0.6;">Você fornece vídeos e fotos</li>
                        
                        <li class="section-title">✅ Gestão de Tráfego</li>
                        <li>3 Campanhas</li>
                        <li>5 Dias de Teste</li>
                        <li>15 Dias de Otimizações</li>
                        <li>Suporte em Horário Comercial</li>
                        <li>Relatório Quinzenal</li>
                        
                        <li class="section-title">Adicionais*</li>
                        <li>Criação de Posts*</li>
                        <li>Banners*</li>
                        <li>WhatsApp Auto*</li>
                    </ul>
                    <center><a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Inclusive" class="cta-button">Quero o Inclusive</a></center>
                </div>

                <div class="plan featured">
                    <div class="badge">+ Popular</div>
                    <div class="plan-header">
                        <div class="plan-icon">🚀</div>
                        <div class="plan-name">Pro</div>
                        <div class="plan-price">R$ 3.680</div>
                    </div>
                    <p style="text-align: center; color: #7cd400; font-weight: bold;">Completo com produção visual</p>
                    <ul class="plan-features">
                        <li class="section-title">✅ Audio Visual</li>
                        <li>25 Fotos Profissionais</li>
                        <li>2 Vídeos Formato Reels</li>
                        
                        <li class="section-title">✅ Gestão de Tráfego</li>
                        <li>3 Campanhas</li>
                        <li>5 Dias de Teste</li>
                        <li>20 Dias de Otimizações</li>
                        <li>Suporte Prioritário</li>
                        <li>Relatório Semanal Detalhado</li>
                        
                        <li class="section-title">Adicionais*</li>
                        <li>Criação de Posts*</li>
                        <li>Banners*</li>
                        <li>WhatsApp Auto*</li>
                        <li style="color: #a8ff00; font-weight: bold;">Até 10% de desconto nos adicionais</li>
                    </ul>
                    <center><a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Pro" class="cta-button">Quero o Pro</a></center>
                </div>

                <div class="plan">
                    <div class="plan-header">
                        <div class="plan-icon">👑</div>
                        <div class="plan-name">Master</div>
                        <div class="plan-price">R$ 4.190</div>
                    </div>
                    <p style="text-align: center; color: #7cd400; font-weight: bold;">Máximo desempenho e conteúdo</p>
                    <ul class="plan-features">
                        <li class="section-title">✅ Audio Visual Premium</li>
                        <li>35 Fotos Profissionais</li>
                        <li>3 Vídeos Formato Reels</li>
                        <li>1 Vídeo de Drone</li>
                        
                        <li class="section-title">✅ Gestão de Tráfego</li>
                        <li>5 Campanhas Simultâneas</li>
                        <li>6 Dias de Teste</li>
                        <li>25 Dias de Otimizações</li>
                        <li>Suporte 24 Horas</li>
                        <li>Relatório em Tempo Real</li>
                        
                        <li class="section-title">Adicionais*</li>
                        <li>Criação de Posts*</li>
                        <li>Banners*</li>
                        <li>WhatsApp Auto*</li>
                        <li style="color: #a8ff00; font-weight: bold;">Até 25% de desconto nos adicionais</li>
                    </ul>
                    <center><a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Master" class="cta-button">Quero o Master</a></center>
                </div>

                <div class="plan">
                    <div class="plan-header">
                        <div class="plan-icon">📈</div>
                        <div class="plan-name">Growth</div>
                        <div class="plan-price">R$ 2.490</div>
                    </div>
                    <p style="text-align: center; color: #7cd400; font-weight: bold;">Foco total em conversão</p>
                    <ul class="plan-features">
                        <li class="section-title">❌ Audio Visual</li>
                        <li style="opacity: 0.6;">Material por sua conta</li>
                        
                        <li class="section-title">✅ Gestão de Tráfego Avançada</li>
                        <li>4 Campanhas Simultâneas</li>
                        <li>5 Dias de Teste A/B</li>
                        <li>20 Dias de Otimizações</li>
                        <li>Remarketing Avançado</li>
                        <li>Suporte Prioritário</li>
                        <li>Análise de Concorrência</li>
                        <li>Dashboard Personalizado</li>
                    </ul>
                    <center><a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Growth" class="cta-button">Quero o Growth</a></center>
                </div>

                <div class="plan">
                    <div class="plan-header">
                        <div class="plan-icon">💼</div>
                        <div class="plan-name">Complete</div>
                        <div class="plan-price">R$ 5.290</div>
                    </div>
                    <p style="text-align: center; color: #7cd400; font-weight: bold;">Solução 360° completa</p>
                    <ul class="plan-features">
                        <li class="section-title">✅ Audio Visual Completo</li>
                        <li>40 Fotos Profissionais</li>
                        <li>4 Vídeos Formato Reels</li>
                        <li>2 Vídeos de Drone</li>
                        <li>Edição Avançada</li>
                        
                        <li class="section-title">✅ Gestão de Tráfego Premium</li>
                        <li>6 Campanhas Simultâneas</li>
                        <li>7 Dias de Teste Multi-variável</li>
                        <li>30 Dias de Otimizações</li>
                        <li>Suporte 24/7 WhatsApp</li>
                        <li>Consultoria Estratégica Mensal</li>
                        
                        <li class="section-title">✅ Inclusos</li>
                        <li>Criação de Posts</li>
                        <li>Banners</li>
                        <li>WhatsApp Auto</li>
                        <li style="color: #a8ff00; font-weight: bold;">Economia de até R$ 1.500</li>
                    </ul>
                    <center><a href="https://wa.me/5548914260130?text=Olá! Quero conhecer o plano Complete" class="cta-button">Quero o Complete</a></center>
                </div>
            </div>
        </div>
    </section>

    <section class="enterprise-section" id="enterprise">
        <div class="container">
            <h2 style="text-align: center; font-size: 2.5em; margin-bottom: 20px; color: #a8ff00;">🎨 Plano Enterprise Personalizado</h2>
            <p style="text-align: center; font-size: 1.2em; margin-bottom: 50px; max-width: 800px; margin-left: auto; margin-right: auto;">
                Monte seu plano sob medida. Selecione exatamente o que você precisa e receba um orçamento instantâneo.
            </p>
            
            <div class="enterprise-content">
                <div class="enterprise-form">
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
                                <input type="checkbox" id="av-fotos" data-price="800">
                                <label for="av-fotos">Sessão de Fotos Profissionais (20-30 fotos) - R$ 800</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="av-fotos-extra" data-price="400">
                                <label for="av-fotos-extra">Fotos Extras (+15 fotos) - R$ 400</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="av-reels" data-price="600">
                                <label for="av-reels">Vídeos Reels (2 vídeos editados) - R$ 600</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="av-reels-extra" data-price="400">
                                <label for="av-reels-extra">Reels Extras (+2 vídeos) - R$ 400</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="av-drone" data-price="800">
                                <label for="av-drone">Vídeo de Drone (1 vídeo aéreo) - R$ 800</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="av-edicao" data-price="500">
                                <label for="av-edicao">Edição Avançada com Efeitos - R$ 500</label>
                            </div>
                        </div>
                    </div>

                    <div class="form-group">
                        <label>🎯 Gestão de Tráfego</label>
                        <div class="checkbox-group">
                            <div class="checkbox-item">
                                <input type="checkbox" id="trafego-basic" data-price="990">
                                <label for="trafego-basic">Gestão Básica (2 campanhas, 10 dias) - R$ 990</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="trafego-standard" data-price="1790">
                                <label for="trafego-standard">Gestão Standard (3 campanhas, 15 dias) - R$ 1.790</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="trafego-advanced" data-price="2490">
                                <label for="trafego-advanced">Gestão Avançada (4 campanhas, 20 dias) - R$ 2.490</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="trafego-premium" data-price="3500">
                                <label for="trafego-premium">Gestão Premium (6 campanhas, 30 dias) - R$ 3.500</label>
                            </div>
                        </div>
                    </div>

                    <div class="form-group">
                        <label>📱 Conteúdo e Automação</label>
                        <div class="checkbox-group">
                            <div class="checkbox-item">
                                <input type="checkbox" id="content-posts" data-price="800">
                                <label for="content-posts">Criação de Posts (12 posts/mês) - R$ 800</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="content-banners" data-price="500">
                                <label for="content-banners">Design de Banners (10 banners) - R$ 500</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="content-whatsapp" data-price="600">
                                <label for="content-whatsapp">WhatsApp Automático (chatbot) - R$ 600</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="content-stories" data-price="400">
                                <label for="content-stories">Stories Diários (30 stories/mês) - R$ 400</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="content-copywriting" data-price="700">
                                <label for="content-copywriting">Copywriting Profissional - R$ 700</label>
                            </div>
                        </div>
                    </div>

                    <div class="form-group">
                        <label>🚀 Extras Premium</label>
                        <div class="checkbox-group">
                            <div class="checkbox-item">
                                <input type="checkbox" id="extra-consultoria" data-price="1200">
                                <label for="extra-consultoria">Consultoria Estratégica Mensal - R$ 1.200</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="extra-dashboard" data-price="500">
                                <label for="extra-dashboard">Dashboard Personalizado - R$ 500</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="extra-suporte24" data-price="800">
                                <label for="extra-suporte24">Suporte 24/7 Prioritário - R$ 800</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="extra-concorrencia" data-price="600">
                                <label for="extra-concorrencia">Análise de Concorrência - R$ 600</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="extra-landing" data-price="1500">
                                <label for="extra-landing">Landing Page Profissional - R$ 1.500</label>
                            </div>
                        </div>
                    </div>

                    <div class="form-group">
                        <label for="specialRequests">Solicitações Especiais</label>
                        <textarea id="specialRequests" placeholder="Descreva qualquer necessidade específica do seu negócio..."></textarea>
                    </div>
                </div>

                <div class="enterprise-preview">
                    <h3>📊 Seu Orçamento</h3>
                    
                    <div class="preview-content" id="previewContent">
                        <p style="text-align: center; color: #a8ff00; padding: 40px 20px;">
                            Selecione os serviços ao lado para ver seu orçamento personalizado
                        </p>
                    </div>

                    <div class="preview-price" id="totalPrice">R$ 0</div>

                    <div class="preview-note">
                        💡 <strong>Desconto Progressivo:</strong><br>
                        • Acima de R$ 5.000: 10% de desconto<br>
                        • Acima de R$ 8.000: 15% de desconto<br>
                        • Acima de R$ 12.000: 20% de desconto
                    </div>

                    <center>
                        <a href="#" class="cta-button" id="sendQuote" style="width: 100%; text-align: center; margin-top: 20px;">
                            💬 Enviar Orçamento via WhatsApp
                        </a>
                    </center>
                </div>
            </div>
        </div>
    </section>

    <section class="results">
        <div class="container">
            <h2>📊 Resultados em 30 Dias</h2>
            <div class="stats">
                <div class="stat">
                    <div class="stat-number">1,2k - 5,8k</div>
                    <div class="stat-label">Alcance Diário</div>
                </div>
                <div class="stat">
                    <div class="stat-number">15 - 70</div>
                    <div class="stat-label">Cliques por Dia</div>
                </div>
                <div class="stat">
                    <div class="stat-number">90%</div>
                    <div class="stat-label">Público Estratégico</div>
                </div>
            </div>
        </div>
    </section>

    <section class="cta-final" id="contato">
        <div class="container">
            <h2>Você quer ser mais um no mercado... ou quer ser a referência na sua região?</h2>
            <p>Sua agenda com MAIS CLIENTES todos os dias começa agora.</p>
            <a href="https://wa.me/5548914260130?text=Olá! Quero saber mais sobre os planos de tráfego pago" class="cta-button" style="background: #25d366;">
                💬 Falar no WhatsApp
            </a>
        </div>
    </section>

    <script>
        // Animação suave ao rolar
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
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

        // Animação de entrada dos elementos
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.stage, .plan, .problem-card, .stat').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(30px)';
            el.style.transition = 'all 0.6s ease-out';
            observer.observe(el);
        });

        // Sistema de cálculo do plano Enterprise
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
                    total += price;
                    const label = checkbox.nextElementSibling.textContent.split(' - ')[0];
                    
                    if (checkbox.id.startsWith('av-')) {
                        selectedItems.audioVisual.push(label);
                    } else if (checkbox.id.startsWith('trafego-')) {
                        selectedItems.trafego.push(label);
                    } else if (checkbox.id.startsWith('content-')) {
                        selectedItems.conteudo.push(label);
                    } else if (checkbox.id.startsWith('extra-')) {
                        selectedItems.extras.push(label);
                    }
                }
            });

            // Aplicar descontos progressivos
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

            // Atualizar preview
            updatePreview(selectedItems, total, discountAmount, finalTotal, discountText);
        }

        function updatePreview(items, subtotal, discount, total, discountText) {
            if (subtotal === 0) {
                previewContent.innerHTML = `
                    <p style="text-align: center; color: #a8ff00; padding: 40px 20px;">
                        Selecione os serviços ao lado para ver seu orçamento personalizado
                    </p>
                `;
                totalPriceEl.textContent = 'R$ 0';
                return;
            }

            let html = '';

            if (items.audioVisual.length > 0) {
                html += `
                    <div class="preview-section">
                        <h4>📸 Audio Visual</h4>
                        <ul>
                            ${items.audioVisual.map(item => `<li>${item}</li>`).join('')}
                        </ul>
                    </div>
                `;
            }

            if (items.trafego.length > 0) {
                html += `
                    <div class="preview-section">
                        <h4>🎯 Gestão de Tráfego</h4>
                        <ul>
                            ${items.trafego.map(item => `<li>${item}</li>`).join('')}
                        </ul>
                    </div>
                `;
            }

            if (items.conteudo.length > 0) {
                html += `
                    <div class="preview-section">
                        <h4>📱 Conteúdo e Automação</h4>
                        <ul>
                            ${items.conteudo.map(item => `<li>${item}</li>`).join('')}
                        </ul>
                    </div>
                `;
            }

            if (items.extras.length > 0) {
                html += `
                    <div class="preview-section">
                        <h4>🚀 Extras Premium</h4>
                        <ul>
                            ${items.extras.map(item => `<li>${item}</li>`).join('')}
                        </ul>
                    </div>
                `;
            }

            if (discount > 0) {
                html += `
                    <div class="preview-section" style="background: rgba(168, 255, 0, 0.1); padding: 15px; border-radius: 10px; border: 2px solid #a8ff00;">
                        <h4 style="color: #a8ff00;">🎉 ${discountText}</h4>
                        <p style="color: #e0e0e0;">Subtotal: <span style="text-decoration: line-through;">R$ ${subtotal.toFixed(2)}</span></p>
                        <p style="color: #a8ff00; font-weight: bold;">Economia: R$ ${discount.toFixed(2)}</p>
                    </div>
                `;
            }

            previewContent.innerHTML = html;
            totalPriceEl.textContent = `R$ ${total.toFixed(2)}`;
        }

        // Event listeners para checkboxes
        checkboxes.forEach(checkbox => {
            checkbox.addEventListener('change', calculateTotal);
        });

        // Enviar orçamento via WhatsApp
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
```
