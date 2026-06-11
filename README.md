<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agro & Sustentabilidade - Laura Cristina</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }
        body {
            background: #FFF5F8;
            color: #4A2A33;
            font-size: 18px;
            transition: 0.3s;
        }
        header {
            background: linear-gradient(135deg, #C2185B, #EC407A);
            color: white;
            text-align: center;
            padding: 50px;
        }
        header h1 {
            font-size: 50px;
            margin-bottom: 10px;
        }
        header h2 {
            font-size: 24px;
            font-weight: normal;
        }
        .botoes {
            margin-top: 20px;
        }
        button {
            background: white;
            color: #C2185B;
            border: none;
            padding: 12px 20px;
            margin: 5px;
            border-radius: 30px;
            font-weight: bold;
            cursor: pointer;
        }
        button:hover {
            background: #F8BBD0;
        }
        nav {
            background: #AD1457;
            padding: 15px;
            text-align: center;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 15px;
            font-weight: bold;
        }
        section {
            width: 90%;
            max-width: 1100px;
            margin: 30px auto;
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }
        h2 {
            color: #C2185B;
            margin-bottom: 15px;
        }
        img {
            width: 100%;
            border-radius: 15px;
            margin-top: 15px;
        }
        .saiba {
            display: inline-block;
            margin-top: 15px;
            background: #EC407A;
            color: white;
            padding: 12px 25px;
            border-radius: 30px;
            text-decoration: none;
        }
        .saiba:hover {
            background: #C2185B;
        }
        footer {
            background: #AD1457;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 30px;
        }
        .contraste {
            background: black;
            color: white;
        }
        .contraste section {
            background: #111;
            color: white;
        }
        .contraste h2 {
            color: #FF80AB;
        }
    </style>
</head>
<body>

    <header>
        <h1>Agro & Sustentabilidade</h1>
        <h2>Projeto desenvolvido por Laura Cristina</h2>
        <p>Produção agrícola, tecnologia e preservação ambiental para um futuro sustentável.</p>

        <div class="botoes">
            <button onclick="aumentarTexto()">Aumentar Texto</button>
            <button onclick="diminuirTexto()">Diminuir Texto</button>
            <button onclick="contraste()">Contraste</button>
        </div>
    </header>

    <nav>
        <a href="#agro">Agro</a>
        <a href="#sustentabilidade">Sustentabilidade</a>
        <a href="#tecnologia">Tecnologia</a>
    </nav>

    <section id="agro">
        <h2>O que é o Agronegócio?</h2>
        <p>O agronegócio é um dos setores mais importantes da economia brasileira, responsável pela produção de alimentos, geração de empregos e desenvolvimento econômico.</p>
        <img src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854" alt="Agricultura sustentável">
        <a class="saiba" href="agro.html" target="_blank">Saiba Mais</a>
    </section>

    <section id="sustentabilidade">
        <h2>Sustentabilidade no Campo</h2>
        <p>A sustentabilidade busca equilibrar a produção agrícola, preservação ambiental e desenvolvimento social, garantindo recursos para as futuras gerações.</p>
        <img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399" alt="Plantação sustentável">
        <a class="saiba" href="sustentabilidade.html" target="_blank">Saiba Mais</a>
    </section>

    <section id="tecnologia">
        <h2>Tecnologia Agrícola</h2>
        <p>A tecnologia no campo inclui drones, sensores, máquinas inteligentes e agricultura de precisão, aumentando a produtividade e reduzindo impactos ambientais.</p>
        <img src="https://images.unsplash.com/photo-1586771107445-d3ca888129ff" alt="Tecnologia no campo">
        <a class="saiba" href="tecnologia.html" target="_blank">Saiba Mais</a>
    </section>

    <section id="grafico">
        <h2>Indicadores de Sustentabilidade</h2>
        <div id="grafico-container">
            <!-- Aqui você pode inserir um gráfico de uma biblioteca como Chart.js, ou outro que preferir -->
            <canvas id="grafico"></canvas>
        </div>
    </section>

    <section id="mapa">
        <h2>Mapa Interativo</h2>
        <iframe
            src="https://www.openstreetmap.org/export/embed.html?bbox=-56.0%2C-33.0%2C-34.0%2C-5.0&amp;layer=mapnik"
            width="100%" height="450" style="border:0;" allowfullscreen=""
            loading="lazy">
        </iframe>
    </section>

    <section id="video">
        <h2>Vídeo Educativo sobre Agronegócio</h2>
        <iframe width="100%" height="450" src="https://www.youtube.com/embed/5mKxQAF7r84" title="Agronegócio" allowfullscreen></iframe>
    </section>

    <footer>
        <p>Laura Cristina • Agro & Sustentabilidade</p>
    </footer>

    <script>
        let tamanho = 18;
        function aumentarTexto() {
            tamanho += 2;
            document.body.style.fontSize = tamanho + "px";
        }
        function diminuirTexto() {
            if (tamanho > 12) {
                tamanho -= 2;
                document.body.style.fontSize = tamanho + "px";
            }
        }
        function contraste() {
            document.body.classList.toggle("contraste");
        }

        // Exemplo de gráfico (usando Chart.js - você precisa adicionar a biblioteca Chart.js no projeto)
        // Caso queira um gráfico real, insira o script e configure o gráfico
        // Exemplo:
        // const ctx = document.getElementById('grafico').getContext('2d');
        // new Chart(ctx, {
        //     type: 'bar',
        //     data: {
        //         labels: ['Sustentabilidade', 'Economia de Água', 'Tecnologia'],
        //         datasets: [{
        //             label: 'Percentual',
        //             data: [90, 85, 92],
        //             backgroundColor: ['#C2185B', '#EC407A', '#F8BBD0']
        //         }]
        //     },
        //     options: {
        //         responsive: true,
        //         scales: {
        //             y: { beginAtZero: true, max: 100 }
        //         }
        //     }
        // });
    </script>
</body>
</html>