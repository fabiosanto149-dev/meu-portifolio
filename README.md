

<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ruany | Account Manager Vivo Empresas</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            /* Cores com tendência feminina e profissional */
            --primary: #6600ff; /* Roxo Profundo */
            --secondary: #ff00cc; /* Magenta Vivo */
            --accent: #ffb7c5; /* Detalhe Rose Gold */
            --dark: #0a0510;
            --glass: rgba(255, 255, 255, 0.05);
            --border: rgba(255, 255, 255, 0.1);
        }

        * {
            margin: 0; padding: 0; box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--dark);
            color: white;
            overflow-x: hidden;
        }

        /* Fundo Dinâmico */
        body::before {
            content: "";
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: radial-gradient(circle at 70% 30%, #1e0a3d 0%, #0a0510 100%);
            z-index: -1;
        }

        .glow {
            position: absolute;
            width: 400px; height: 400px;
            background: var(--secondary);
            filter: blur(180px);
            border-radius: 50%;
            opacity: 0.1;
            top: 10%; left: 5%;
            animation: move 12s infinite alternate;
        }

        @keyframes move {
            from { transform: translate(0, 0); }
            to { transform: translate(100px, 50px); }
        }

        header {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 0 8%;
        }

        .container {
            max-width: 1200px;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 40px;
        }

        /* Foto com borda orgânica (Morphing) */
        .profile-area {
            position: relative;
            width: 400px;
            height: 400px;
        }

        .profile-img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
            border: 2px solid var(--border);
            box-shadow: 0 0 50px rgba(255, 0, 204, 0.2);
            animation: morph 8s ease-in-out infinite;
        }

        @keyframes morph {
            0% { border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%; }
            50% { border-radius: 30% 60% 70% 40% / 50% 60% 30% 60%; }
            100% { border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%; }
        }

        .content h2 {
            color: var(--secondary);
            letter-spacing: 4px;
            font-size: 0.8rem;
            text-transform: uppercase;
            margin-bottom: 10px;
        }

        .content h1 {
            font-size: 3.8rem;
            line-height: 1.1;
            margin-bottom: 20px;
        }

        .content h1 span {
            background: linear-gradient(to right, var(--secondary), var(--accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Botão WhatsApp */
        .cta-button {
            display: inline-block;
            margin-top: 30px;
            padding: 18px 45px;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            color: white;
            text-decoration: none;
            font-weight: 600;
            border-radius: 12px;
            transition: 0.4s;
            box-shadow: 0 10px 25px rgba(255, 0, 204, 0.3);
        }

        .cta-button:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(255, 0, 204, 0.5);
        }

        /* Seção de Excelência */
        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin: 100px 0 50px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            padding: 0 10% 100px;
        }

        .card {
            background: var(--glass);
            backdrop-filter: blur(15px);
            border: 1px solid var(--border);
            padding: 40px;
            border-radius: 25px;
            transition: 0.4s;
        }

        .card:hover {
            background: rgba(255, 255, 255, 0.08);
            border-color: var(--secondary);
            transform: translateY(-10px);
        }

        .card h3 {
            color: var(--accent);
            margin-bottom: 15px;
        }

        @media (max-width: 900px) {
            .container { flex-direction: column-reverse; text-align: center; }
            .profile-area { width: 300px; height: 300px; }
            .content h1 { font-size: 2.8rem; }
        }
    </style>
</head>
<body>
    <div class="glow"></div>

    <header>
        <div class="container">
            <div class="content">
                <h2>Vivo Empresas</h2>
                <h1>Olá, eu sou <span>Ruany</span></h1>
                <p>Gerente de Contas focada em transformar a conectividade do seu negócio com <b>eficiência</b> e <b>qualidade</b> de serviço surreal.</p>
                <a href="https://wa.me/552730619962" class="cta-button" target="_blank">Solicitar Consultoria</a>
            </div>
            <div class="profile-area">
                <img src="ruany.jpg" alt="Ruany" class="profile-img">
            </div>
        </div>
    </header>

    <h2 class="section-title">Opções de Excelência</h2>
    <div class="grid">
        <div class="card">
            <h3>Gestão Estratégica</h3>
            <p>Atendimento consultivo e personalizado para otimizar os custos e a performance da sua empresa.</p>
        </div>
        <div class="card">
            <h3>Qualidade de Serviço</h3>
            <p>Implementação das melhores soluções B2B da Vivo, garantindo estabilidade e alta tecnologia.</p>
        </div>
        <div class="card">
            <h3>Eficiência Máxima</h3>
            <p>Processos ágeis e suporte dedicado para que sua equipe nunca pare de produzir.</p>
        </div>
    </div>

    <h2 class="section-title" id="sobre">SOBRE MIM</h2>
    <div style="max-width: 800px; margin: 0 auto; text-align: center; padding: 0 20px 100px; line-height: 1.8;">
        <p>Sou especialista em soluções corporativas na Vivo Empresas, atuando como parceira estratégica de grandes e pequenos negócios. Minha missão é entregar excelência através de um olhar atento às necessidades do cliente, unindo a força da marca Vivo com um atendimento humano e eficiente.</p>
    </div>

</body>
</html>
