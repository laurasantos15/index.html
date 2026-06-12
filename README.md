<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agro e Sustentabilidade - Laura Cristina</title>
    <style>
        :root {
            --vinho: #6b0f1a;
            --vinho2: #8f1730;
            --fundo: #f5f5f5;
            --texto: #222;
            --rosa: #ff4fa3;
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
            scroll-behavior: smooth;
        }
        body {
            background: var(--fundo);
            color: var(--texto);
            font-size: 16px;
            transition: 0.3s;
        }
        body.contraste {
            background: #000;
            color: var(--rosa);
        }
        header {
            background: linear-gradient(135deg, var(--vinho), #3a0610);
            color: white;
            text-align: center;
            padding: 30px 20px;
        }
        header h1 {
            font-size: 2.6rem;
        }
        header p {
            opacity: 0.9;
        }
        nav {
            background: var(--vinho2);
            display: flex;
            justify-content: center;
            gap: 25px;
            padding: 14px;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
            cursor: pointer;
        }
        nav a:hover {
            opacity: 0.7;
        }
        .hero {
            height: 85vh;
            background: linear-gradient(rgba(0,0,0,.55), rgba(0,0,0,.55)), 
                        url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&w=1600&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            padding: 20px;
        }
        .hero h2 {
            font-size: 3rem;
            margin-bottom: 15px;
        }
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 20px;
        }
        .btn {
            display: inline-block;
            padding: 12px 22px;
            background: var(--vinho);
            color: white;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            cursor: pointer;
            transition: 0.3s;
        }
        .btn:hover {
            transform: scale(1.05);
        }
        section {
            padding: 70px 10%;
            display: none;
        }
        section.ativo {
            display: block;
        }
        .titulo {
            text-align: center;
            font-size: 2.2rem;
            color: var(--vinho);
            margin-bottom: 35px;
        }
        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .card {
            background: white;
            padding: 22px;
            border-radius: 12px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.08);
            transition: 0.3s;
        }
        .card:hover {
            transform: translateY(-5px);
        }
        .video {
            display: flex;
            justify-content: center;
        }
        iframe {
            width: 100%;
            max-width: 800px;
            height: 450px;
            border: none;
            border-radius: 12px;
        }
        .saiba {
            max-height: 0;
            overflow: hidden;
            opacity: 0;
            transition: 0.6s ease;
            background: white;
            border-left: 6px solid var(--vinho);
            padding: 0 20px;
            border-radius: 10px;
        }
        .saiba.ativo {
            max-height: 900px;
            opacity: 1;
            padding: 25px;
        }
        .acessibilidade {
            position: fixed;
            right: 15px;
            bottom: 15px;
            display: flex;
            flex-direction: column;
            gap: 10px;
            z-index: 999;
        }
        .acessibilidade button {
            background: var(--vinho);
            color: white;
            border: none;
            padding: 12px 14px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.3s;
        }
        .acessibilidade button:hover {
            transform: scale(1.05);
        }
        footer {
            background: var(--vinho);
            color: white;
            text-align: center;
            padding: 25px;
            margin-top: 40px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Agro e Sustentabilidade</h1>
        <p>Projeto Acadêmico - Laura Cristina</p>
    </header>

    <nav>
        <a onclick="mostrar('home')">Início</a>
        <a onclick="mostrar('sobre')">Saiba Mais</a>
    </nav>

    <!-- HOME -->
    <section id="home" class="ativo">
        <div class="hero">
            <h2>O Futuro do Agro é Sustentável</h2>
            <p>Produzir mais com menos impacto ambiental</p>
            <a class="btn" onclick="mostrar('sobre')">Explorar Mais</a>
        </div>
        <div style="padding: 50px; text-align: center;">
            <h3>O que é Agro Sustentável?</h3>
            <p>
                O agronegócio sustentável busca aliar produtividade e preservação ambiental, 
                garantindo recursos para as próximas gerações.
            </p>
            <div class="cards">
                <div class="card">
                    <h3>🌱 Sustentabilidade</h3>
                    <p>Uso consciente dos recursos naturais e proteção da biodiversidade.</p>
                </div>
                <div class="card">
                    <h3>🚜 Tecnologia</h3>
                    <p>Agricultura de precisão, drones e sensores no campo.</p>
                </div>
                <div class="card">
                    <h3>🌍 Futuro</h3>
                    <p>Garantir a segurança alimentar com menor impacto no planeta.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SOBRE (SAIBA MAIS) -->
    <section id="sobre">
        <h2 class="titulo">Saiba Mais</h2>
        <div style="max-width: 900px; margin: auto;">
            <p>
                O agronegócio sustentável é uma abordagem que busca equilibrar a produção