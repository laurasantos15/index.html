<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agro e Sustentabilidade - Laura Cristina</title>

    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

    <style>
        :root {
            --vinho: #6b0f1a;
            --vinho-claro: #8f1730;
            --fundo: #f7f7f7;
            --texto: #222;
            --branco: #fff;
            --rosa: #ff66b2;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', sans-serif;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            background: var(--fundo);
            color: var(--texto);
            font-size: 16px;
            transition: 0.4s;
        }

        body.contraste {
            background: #000;
            color: var(--rosa);
        }

        header {
            background: linear-gradient(135deg, var(--vinho), #4a0712);
            color: white;
            padding: 25px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0,0,0,0.2);
        }

        header h1 {
            font-size: 2.8rem;
        }

        header p {
            margin-top: 10px;
            font-size: 1.1rem;
        }

        nav {
            background: var(--vinho-claro);
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            padding: 15px;
            gap: 20px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: .3s;
        }

        nav a:hover {
            transform: scale(1.05);
        }

        .hero {
            height: 80vh;
            background: linear-gradient(rgba(0,0,0,.45), rgba(0,0,0,.45)), url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&w=1600&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: