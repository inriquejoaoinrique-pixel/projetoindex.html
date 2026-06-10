<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JotaPe Marketing | Inteligência Digital e Escala de Vendas</title>
    <meta name="description" content="Estratégias de marketing digital para transformar cliques em lucro real. Tráfego pago, branding, copywriting e crescimento para empresas.">
    <meta name="keywords" content="marketing digital, tráfego pago, branding, copywriting, crescimento de empresas, JotaPe Marketing">
    <meta name="author" content="JotaPe Marketing">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" integrity="sha512-iecdLmaskl7CVkqkXNQ/ZH/XLlvWZOJyj7Yy7tcenmpD1ypASozpmT/E0iPtmFIB46ZmdtAc9eNBvH0H/ZpiBw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <style>
        /* CONFIGURAÇÕES GERAIS E PALETA MULTI-AZUL */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            scroll-behavior: smooth;
        }

        :root {
            --bg-deep: #030914;       /* Azul Espacial Ultra Escuro */
            --bg-card: #0a1326;       /* Azul Sólido para Blocos */
            --blue-main: #0052d4;     /* Azul Royal - Autoridade */
            --blue-electric: #00d2ff; /* Azul Ciano - Destaque */
            --text-muted: #94a3b8;    /* Cinza Azulado */
            --white: #ffffff;
        }

        body {
            background-color: var(--bg-deep);
            color: var(--white);
            overflow-x: hidden;
            line-height: 1.6;
        }

        a { text-decoration: none; color: inherit; }

        /* HEADER FLUTUANTE */
        header {
            background-color: rgba(3, 9, 20, 0.95);
            backdrop-filter: blur(12px);
            padding: 15px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(0, 210, 255, 0.12);
        }

        /* LOGO */
        .logo-container {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-circulo {
            width: 48px;
            height: 48px;
            background-color: #070d19;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 900;
            font-size: 20px;
            letter-spacing: -1px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 0 15px rgba(0, 210, 255, 0.2);
        }

        .logo-circulo .letra-j {
            color: var(--blue-electric);
            text-shadow: 0 0 8px rgba(0, 210, 255, 0.6);
        }

        .logo-circulo .letra-p {
            color: var(--white);
        }

        .logo-texto {
            font-size: 18px;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            line-height: 1;
        }

        .logo-texto span {
            display: block;
            font-size: 11px;
            color: var(--blue-electric);
            font-weight: 600;
            margin-top: 3px;
            letter-spacing: 1px;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 35px;
        }

        nav ul li a {
            font-weight: 600;
            font-size: 15px;
            color: var(--white);
            transition: color 0.3s ease;
        }

        nav ul li a:hover { color: var(--blue-electric); }

        /* SEÇÃO HERO */
        .hero {
            min-height: 100vh;
            background: radial-gradient(circle at top right, #091e3d 0%, var(--bg-deep) 75%);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 140px 8% 80px 8%;
            text-align: center;
        }

        .hero-emblema-logo {
            width: 90px;
            height: 90px;
            background-color: #070d19;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 900;
            font-size: 38px;
            letter-spacing: -2px;
            border: 2px solid var(--blue-electric);
            box-shadow: 0 0 30px rgba(0, 210, 255, 0.3);
            margin-bottom: 25px;
        }
        .hero-emblema-logo .letra-j { color: var(--blue-electric); text-shadow: 0 0 10px rgba(0, 210, 255, 0.6); }
        .hero-emblema-logo .letra-p { color: var(--white); }

        .badge-tag {
            background: rgba(0, 210, 255, 0.08);
            border: 1px solid var(--blue-electric);
            color: var(--blue-electric);
            padding: 8px 22px;
            border-radius: 50px;
            font-size: 13px;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            margin-bottom: 30px;
            animation: pulse-glow 2.5s infinite;
        }

        .hero h1 {
            font-size: 54px;
            font-weight: 900;
            line-height: 1.15;
            max-width: 950px;
            margin-bottom: 25px;
            letter-spacing: -1px;
        }

        .hero h1 span {
            background: linear-gradient(45deg, var(--blue-electric), #3b82f6);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero p {
            font-size: 20px;
            color: var(--text-muted);
            max-width: 720px;
            margin-bottom: 45px;
        }

        /* BOTÕES */
        .botoes-grupo {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
            justify-content: center;
        }

        .btn {
            padding: 16px 36px;
            border-radius: 8px;
            font-weight: 700;
            font-size: 16px;
            display: inline-flex;
            align-items: center;
            gap: 12px;
            transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
            cursor: pointer;
            border: none;
        }

        .btn-principal {
            background-color: #25d366;
            color: var(--white);
            box-shadow: 0 10px 25px rgba(37, 211, 102, 0.25);
        }

        .btn-principal:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 30px rgba(37, 211, 102, 0.4);
        }

        .btn-secundario {
            background: linear-gradient(135deg, var(--blue-main), #1d4ed8);
            color: var(--white);
            border: 1px solid rgba(0, 210, 255, 0.25);
            box-shadow: 0 10px 25px rgba(0, 82, 212, 0.25);
        }

        .btn-secundario:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 30px rgba(0, 82, 212, 0.4);
        }

        /* SEÇÕES */
        section { padding: 110px 8%; }

        .header-secao {
            text-align: center;
            max-width: 800px;
            margin: 0 auto 65px auto;
        }

        .header-secao h2 {
            font-size: 40px;
            font-weight: 800;
            margin-bottom: 15px;
            letter-spacing: -0.5px;
        }

        .header-secao h2 span { color: var(--blue-electric); }

        .header-secao p { font-size: 18px; color: var(--text-muted); }

        /* QUEM SOMOS */
        .quem-somos { background-color: var(--bg-card); }

        .bloco-grid {
            display: grid;
            grid-template-columns: 1.2fr 0.8fr;
            gap: 60px;
            align-items: center;
        }

        .conteudo-texto h3 {
            font-size: 28px;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .conteudo-texto p {
            font-size: 16px;
            color: #cbd5e1;
            margin-bottom: 20px;
            text-align: justify;
        }

        .grid-status {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .card-status {
            background-color: var(--bg-deep);
            padding: 30px 20px;
            border-radius: 12px;
            border: 1px solid rgba(255, 255, 255, 0.04);
            text-align: center;
        }

        .card-status h4 { font-size: 38px; color: var(--blue-electric); font-weight: 800; }
        .card-status p { font-size: 14px; color: var(--text-muted); font-weight: 600; }

        /* ALAVANCAGEM */
        .alavancagem {
            background: linear-gradient(180deg, var(--bg-deep) 0%, #051124 100%);
        }

        .texto-propaganda {
            background: linear-gradient(135deg, rgba(0, 82, 212, 0.15), rgba(10, 19, 38, 0.8));
            border: 1px solid rgba(0, 210, 255, 0.25);
            padding: 50px;
            border-radius: 16px;
            margin-bottom: 50px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }

        .texto-propaganda h3 { font-size: 26px; margin-bottom: 20px; color: var(--white); }
        .texto-propaganda p { color: #e2e8f0; font-size: 17px; line-height: 1.8; margin-bottom: 20px; }
        .texto-propaganda p strong { color: var(--blue-electric); }

        .pilares-estrategicos {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .pilar-card {
            background-color: var(--bg-card);
            padding: 35px 30px;
            border-radius: 12px;
            border-top: 4px solid var(--blue-main);
            transition: transform 0.3s ease;
        }

        .pilar-card:hover { transform: translateY(-5px); }
        .pilar-card i { font-size: 32px; color: var(--blue-electric); margin-bottom: 20px; }
        .pilar-card h4 { font-size: 19px; margin-bottom: 12px; font-weight: 700; }
        .pilar-card p { font-size: 15px; color: var(--text-muted); }

        /* SERVIÇOS */
        .servicos { background-color: var(--bg-card); }

        .grid-servicos {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
            gap: 30px;
        }

        .card-servico {
            background-color: var(--bg-deep);
            padding: 45px 35px;
            border-radius: 16px;
            border: 1px solid rgba(255,255,255,0.02);
            transition: all 0.3s ease;
        }

        .card-servico:hover {
            border-color: var(--blue-electric);
            box-shadow: 0 15px 35px rgba(0, 210, 255, 0.08);
            transform: translateY(-5px);
        }

        .card-servico .icone-caixa {
            width: 65px;
            height: 65px;
            background: rgba(0, 82, 212, 0.15);
            border-radius: 14px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 25px;
            color: var(--blue-electric);
            font-size: 26px;
            border: 1px solid rgba(0, 210, 255, 0.2);
        }

        .card-servico h3 { font-size: 23px; margin-bottom: 15px; font-weight: 700; }
        .card-servico p { font-size: 15px; color: #cbd5e1; margin-bottom: 25px; }

        .card-servico ul { list-style: none; }
        .card-servico ul li {
            font-size: 14px;
            color: var(--text-muted);
            margin-bottom: 12px;
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .card-servico ul li i { color: var(--blue-electric); font-size: 12px; }

        /* CTA FINAL */
        .cta-final {
            background: linear-gradient(135deg, var(--bg-deep) 0%, #041229 100%);
            text-align: center;
            border-top: 1px solid rgba(0, 210, 255, 0.08);
        }

        .cta-container { max-width: 780px; margin: 0 auto; }
        .cta-container h3 { font-size: 40px; font-weight: 850; margin-bottom: 25px; }
        .cta-container p { color: #cbd5e1; font-size: 18px; margin-bottom: 45px; }

        /* MODAL WHATSAPP */
        .modal-container {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(3, 9, 20, 0.88);
            backdrop-filter: blur(8px);
            z-index: 2000;
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            background-color: var(--bg-card);
            border: 2px solid var(--blue-electric);
            border-radius: 16px;
            padding: 45px 35px;
            max-width: 500px;
            width: 90%;
            text-align: center;
            position: relative;
            box-shadow: 0 25px 60px rgba(0, 210, 255, 0.15);
        }

        .modal-content h4 { font-size: 24px; margin-bottom: 12px; font-weight: 800; }
        .modal-content p { color: var(--text-muted); font-size: 15px; margin-bottom: 35px; }

        .botoes-modal { display: flex; flex-direction: column; gap: 16px; }

        .btn-whats-opcao {
            background-color: #25d366;
            color: var(--white);
            padding: 15px;
            border-radius: 8px;
            font-weight: 700;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            transition: all 0.2s ease;
        }

        .btn-whats-opcao:hover {
            transform: scale(1.02);
            background-color: #1ebd54;
        }

        .fechar-modal {
            position: absolute;
            top: 15px;
            right: 22px;
            font-size: 26px;
            color: var(--text-muted);
            cursor: pointer;
            transition: color 0.2s;
        }

        .fechar-modal:hover { color: var(--white); }

        /* FOOTER */
        footer {
            background-color: #02050d;
            padding: 45px 8%;
            text-align: center;
            font-size: 14px;
            color: var(--text-muted);
            border-top: 1px solid rgba(255,255,255,0.04);
        }

        /* ANIMAÇÃO */
        @keyframes pulse-glow {
            0% { transform: scale(1); box-shadow: 0 0 0 0 rgba(0, 210, 255, 0.4); }
            70% { transform: scale(1.02); box-shadow: 0 0 0 10px rgba(0, 210, 255, 0); }
            100% { transform: scale(1); box-shadow: 0 0 0 0 rgba(0, 210, 255, 0); }
        }

        /* RESPONSIVIDADE */
        @media (max-width: 968px) {
            .bloco-grid { grid-template-columns: 1fr; gap: 40px; }
            .hero h1 { font-size: 35px; }
            .hero p { font-size: 16px; }
            header { padding: 15px 5%; }
            nav { display: none; }
            section { padding: 75px 5%; }
            .btn { width: 100%; justify-content: center; }
            .header-secao h2 { font-size: 32px; }
            .texto-propaganda { padding: 30px 20px; }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo-container">
            <div class="logo-circulo">
                <span class="letra-j">J</span><span class="letra-p">P</span>
            </div>
            <div class="logo-texto">
                JotaPe Marketing
                <span>MARKETING DIGITAL</span>
            </div>
        </div>
        <nav>
            <ul>
                <li><a href="#inicio">Início</a></li>
                <li><a href="#quem-somos">Quem Somos</a></li>
                <li><a href="#alavancar">Como Alavancamos</a></li>
                <li><a href="#servicos">Nossos Serviços</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="inicio">
        <div class="hero-emblema-logo">
            <span class="letra-j">J</span><span class="letra-p">P</span>
        </div>
        
        <div class="badge-tag"><i class="fas fa-rocket"></i> Crescimento Exponencial</div>
        <h1>Construindo Estratégias Digitais que Convertem Cliques em <span>Lucro Real</span></h1>
        <p>Pare de gastar tempo com publicações genéricas que não geram negócios. Na JotaPe Marketing, desenvolvemos ecossistemas magnéticos focados em atrair clientes qualificados prontos para comprar de você.</p>
        
        <div class="botoes-grupo">
            <button onclick="abrirAtendimento()" class="btn btn-principal">
                <i class="fab fa-whatsapp"></i> Iniciar Escala de Vendas
            </button>
            <a href="https://www.instagram.com/jp.marketing.oficial" target="_blank" rel="noopener noreferrer" class="btn btn-secundario">
                <i class="fab fa-instagram"></i> Conhecer Nosso Instagram
            </a>
        </div>
    </section>

    <section class="quem-somos" id="quem-somos">
        <div class="header-secao">
            <h2>Quem Somos <span>Nós?</span></h2>
            <p>Conheça a estrutura focada em gerar tração comercial para o seu negócio.</p>
        </div>

        <div class="bloco-grid">
            <div class="conteudo-texto">
                <h3>Uma Operação de Elite Voltada à Performance</h3>
                <p>A <strong>JotaPe Marketing</strong> nasceu da necessidade de entregar resultados palpáveis no mercado digital. Não somos uma agência tradicional focada apenas em curtidas ou métricas estéticas. Somos estrategistas comerciais que utilizam a internet como uma ferramenta de multiplicação de receita.</p>
                <p>Nossa equipe une inteligência analítica e excelência criativa para desenhar funis de conversão automatizados, tráfego pago de alta performance e design sofisticado. Cuidamos do posicionamento da sua empresa para que você transmita credibilidade e consiga cobrar o valor justo pelo seu produto ou serviço.</p>
            </div>
            
            <div class="grid-status">
                <div class="card-status">
                    <h4>ROI</h4>
                    <p>Foco em Retorno</p>
                </div>
                <div class="card-status">
                    <h4>100%</h4>
                    <p>Estratégico</p>
                </div>
                <div class="card-status">
                    <h4>Vendas</h4>
                    <p>Objetivo Central</p>
                </div>
                <div class="card-status">
                    <h4>Elite</h4>
                    <p>Posicionamento</p>
                </div>
            </div>
        </div>
    </section>

    <section class="alavancagem" id="alavancar">
        <div class="header-secao">
            <h2>Como Podemos Alavancar Sua <span>Empresa?</span></h2>
            <p>Acelere o crescimento e pare de perder faturamento para concorrentes menos qualificados.</p>
        </div>

        <div class="texto-propaganda">
            <h3>🔥 O Seu Próximo Nível Comercial Começa Aqui:</h3>
            <p>A verdade é que se a sua empresa não aparece com relevância no digital, ela simplesmente não existe para quem busca os seus produtos ou serviços. Estar na internet de forma amadora é pior do que estar fora dela — afasta clientes com alto poder de compra.</p>
            <p>A <strong>JotaPe Marketing</strong> alavanca o seu negócio através de estratégias personalizadas. Analisamos o seu mercado, identificamos brechas deixadas pelos concorrentes e implementamos campanhas direcionadas. Colocamos a sua marca na frente de pessoas qualificadas no momento exato em que elas precisam da sua solução.</p>
            <p>Blindamos a sua comunicação, otimizamos a captação de clientes e direcionamos leads prontos para o seu atendimento — economizando tempo e aumentando o seu faturamento.</p>
        </div>

        <div class="pilares-estrategicos">
            <div class="pilar-card">
                <i class="fas fa-search-dollar"></i>
                <h4>Análise de Mercado</h4>
                <p>Estudamos os pontos fracos dos concorrentes para posicionar sua marca como a escolha óbvia e dominante.</p>
            </div>
            <div class="pilar-card">
                <i class="fas fa-funnel-dollar"></i>
                <h4>Funis de Conversão</h4>
                <p>Estruturamos caminhos digitais inteligentes para que o cliente conheça, confie e entre em contato rápido.</p>
            </div>
            <div class="pilar-card">
                <i class="fas fa-chart-line"></i>
                <h4>Escala Sustentável</h4>
                <p>Criamos campanhas otimizadas para crescer conforme a capacidade de atendimento e demanda aumentam.</p>
            </div>
        </div>
    </section>

    <section class="servicos" id="servicos">
        <div class="header-secao">
            <h2>Nossos <span>Serviços Principais</span></h2>
            <p>Foco máximo naquilo que traz resultado para o caixa. Sem excessos, sem distrações.</p>
        </div>

        <div class="grid-servicos">
            <div class="card-servico">
                <div class="icone-caixa"><i class="fas fa-ad"></i></div>
                <h3>Gestão de Tráfego Pago</h3>
                <p>Criamos, configuramos e gerenciamos campanhas no Meta Ads e Google Ads direcionadas para o público-alvo ideal.</p>
                <ul>
                    <li><i class="fas fa-check"></i> Segmentação avançada por localização e perfil</li>
                    <li><i class="fas fa-check"></i> Criação de materiais focados em conversão</li>
                    <li><i class="fas fa-check"></i> Acompanhamento de métricas e retorno sobre investimento</li>
                </ul>
            </div>

            <div class="card-servico">
                <div class="icone-caixa"><i class="fas fa-crown"></i></div>
                <h3>Branding & Design Premium</h3>
                <p>Elevamos a percepção visual da marca nas redes sociais, transmitindo credibilidade e gerando desejo de compra.</p>
                <ul>
                    <li><i class="fas fa-check"></i> Identidade visual exclusiva e alinhada ao mercado</li>
                    <li><i class="fas fa-check"></i> Materiais gráficos e conteúdo visual profissional</li>
                    <li><i class="fas fa-check"></i> Padronização que gera reconhecimento e confiança</li>
                </ul>
            </div>

            <div class="card-servico">
                <div class="icone-caixa"><i class="fas fa-feather-alt"></i></div>
                <h3>Copywriting Persuasivo</h3>
                <p>Desenvolvemos textos, roteiros e legendas que quebram objeções e levam o cliente à ação.</p>
                <ul>
                    <li><i class="fas fa-check"></i> Roteiros dinâmicos para Reels e Stories</li>
                    <li><i class="fas fa-check"></i> Redação com chamadas claras para ação</li>
                    <li><i class="fas fa-check"></i> Comunicação alinhada com o perfil do seu cliente ideal</li>
                </ul>
            </div>
        </div>
    </section>

    <section class="cta-final">
        <div class="cta-container">
            <h3>Preparado para Liderar o Seu Mercado?</h3>
            <p>Não continue deixando oportunidades passar. Fale com um especialista e descubra a estratégia ideal para o crescimento do seu negócio.</p>
            
            <div class="botoes-grupo">
                <button onclick="abrirAtendimento()" class="btn btn-principal">
                    <i class="fab fa-whatsapp"></i> Falar com um Consultor
                </button>
                <a href="https://www.instagram.com/jp.marketing.oficial" target="_blank" rel="noopener noreferrer" class="btn btn-secundario">
                    <i class="fab fa-instagram"></i> Ver Nosso Trabalho
                </a>
            </div>
        </div>
    </section>

    <div id="modalWhats" class="modal-container">
        <div class="modal-content">
            <span onclick="fecharAtendimento()" class="fechar-modal">&times;</span>
            <h4>Selecione um Canal de Atendimento</h4>
            <p>Para agilizar o contato, clique abaixo e fale diretamente com nosso time:</p>
            <div class="botoes-modal">
                <a href="https://wa.me/558193774327?text=Olá! Vim pelo site da JotaPe Marketing e gostaria de saber mais sobre as estratégias para minha empresa." target="_blank" rel="noopener noreferrer" class="btn-whats-opcao">
                    <i class="fab fa-whatsapp"></i> Atendimento Comercial 01
                </a>
                <a href="https://wa.me/558196572994?text=Olá! Conheci a JotaPe Marketing e quero alinhar uma consultoria estratégica." target="_blank" rel="noopener noreferrer" class="btn-whats-opcao">
                    <i class="fab fa-whatsapp"></i> Atendimento Comercial 02
                </a>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2026 JotaPe Marketing. Todos os direitos reservados.</p>
    </footer>

    <script>
        function abrirAtendimento() {
            document.getElementById('modalWhats').style.display = 'flex';
        }
        function fecharAtendimento() {
            document.getElementById('modalWhats').style.display = 'none';
        }
        window.onclick = function(event) {
            const modal = document.getElementById('modalWhats');
            if (event.target === modal) {
                modal.style.display = 'none';
            }
        }
    </script>

</body>
</html>

