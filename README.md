#PORTIFOLIO!
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fábio Lourenço | Portfolio Developer</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #00f2fe;
            --secondary: #4facfe;
            --dark: #0a0a0b;
            --glass: rgba(255, 255, 255, 0.05);
            --border: rgba(255, 255, 255, 0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--dark);
            color: white;
            overflow-x: hidden;
        }

        /* Fundo Animado Surreal */
        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 50% 50%, #1a1a2e 0%, #0a0a0b 100%);
            z-index: -1;
        }

        .glow {
            position: absolute;
            width: 300px;
            height: 300px;
            background: var(--secondary);
            filter: blur(150px);
            border-radius: 50%;
            opacity: 0.2;
            top: 10%;
            right: 10%;
            animation: move 10s infinite alternate;
        }

        @keyframes move {
            from { transform: translate(0, 0); }
            to { transform: translate(-100px, 100px); }
        }

        header {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 0 5%;
        }

        .container {
            max-width: 1200px;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 50px;
        }

        /* Imagem com Efeito de Bordas Brilhantes */
        .profile-area {
            position: relative;
            width: 400px;
            height: 400px;
        }

        .profile-img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
            border: 4px solid var(--border);
            box-shadow: 0 0 40px rgba(79, 172, 254, 0.3);
            animation: morph 8s ease-in-out infinite;
        }

        @keyframes morph {
            0% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; }
            50% { border-radius: 50% 50% 20% 80% / 25% 80% 20% 75%; }
            100% { border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%; }
        }

        .content h1 {
            font-size: 3.5rem;
            line-height: 1.1;
            margin-bottom: 20px;
        }

        .content h1 span {
            background: linear-gradient(to right, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .contact-btn {
            display: inline-block;
            margin-top: 30px;
            padding: 15px 40px;
            background: linear-gradient(45deg, var(--secondary), var(--primary));
            color: #000;
            text-decoration: none;
            font-weight: bold;
            border-radius: 50px;
            transition: 0.3s;
            box-shadow: 0 10px 20px rgba(79, 172, 254, 0.4);
        }

        .contact-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(79, 172, 254, 0.6);
        }

        /* Seção de Excelência (Cards de Vidro) */
        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin: 100px 0 50px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            padding: 0 10% 100px;
        }

        .card {
            background: var(--glass);
            backdrop-filter: blur(15px);
            border: 1px solid var(--border);
            padding: 40px;
            border-radius: 20px;
            transition: 0.4s;
            cursor: default;
        }

        .card:hover {
            background: rgba(255, 255, 255, 0.1);
            transform: translateY(-10px);
            border-color: var(--primary);
        }

        .card h3 {
            color: var(--primary);
            margin-bottom: 15px;
        }

        @media (max-width: 768px) {
            .container { flex-direction: column-reverse; text-align: center; }
            .profile-area { width: 280px; height: 280px; }
            .content h1 { font-size: 2.5rem; }
        }
    </style>
</head>
<body>
    <div class="glow"></div>

    <header>
        <div class="container">
            <div class="content">
                <p>Análise e Desenvolvimento de Sistemas</p>
                <h1>Olá, eu sou o <br><span>Fábio Lourenço</span></h1>
                <p>Especialista em criar experiências digitais de alta performance e sites de excelência.</p>
                <a href="https://wa.me/27988080831" class="contact-btn">WhatsApp: 27 98808-0831</a>
            </div>
            <div class="profile-area">
                <img src="perfil.jpg" alt="Fábio Lourenço" class="profile-img">
            </div>
        </div>
    </header>

    <h2 class="section-title">Opções de Excelência</h2>
    <div class="grid">
        <div class="card">
            <h3>Desenvolvimento Web</h3>
            <p>Criação de sites modernos, responsivos e otimizados para conversão.</p>
        </div>
        <div class="card">
            <h3>Análise de Sistemas</h3>
            <p>Soluções inteligentes e arquitetura de dados pensada na escalabilidade.</p>
        </div>
        <div class="card">
            <h3>Design Surreal</h3>
            <p>Interface do usuário (UI) focada em estética moderna e usabilidade (UX).</p>
        </div>
    </div>

    <h2 class="section-title" id="sobre">Me Descreva</h2>
    <div style="max-width: 800px; margin: 0 auto; text-align: center; padding: 0 20px 100px; line-height: 1.8;">
        <p>Sou um profissional apaixonado por tecnologia e inovação, atualmente focado em Análise e Desenvolvimento de Sistemas. Minha trajetória une a visão estratégica de negócios com a precisão técnica da engenharia de software. Busco sempre entregar projetos que não apenas funcionem, mas que superem as expectativas em estética e funcionalidade.</p>
    </div>

</body>
</html>
