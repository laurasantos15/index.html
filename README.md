<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agro e Sustentabilidade - Laura Cristina</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        // Configuração da paleta de cores vinho
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        vinho: {
                            50: '#f9f0f2',
                            100: '#f0d6dc',
                            200: '#e0adb8',
                            300: '#cc7a8f',
                            400: '#b34a66',
                            500: '#992647', // Cor principal vinho
                            600: '#7a1e39',
                            700: '#5c172b',
                            800: '#3d0f1d',
                            900: '#1f080f',
                        },
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .texto-normal { font-size: 1rem; }
            .texto-maior { font-size: 1.15rem; }
            .texto-muito-maior { font-size: 1.3rem; }
            .contraste-normal { filter: contrast(100%); }
            .contraste-alto { filter: contrast(150%); }
            .contraste-baixo { filter: contrast(70%); }
        }
    </style>
</head>
<body class="bg-vinho-50 text-vinho-900 font-sans transition-all duration-300" id="corpo">
    <!-- Cabeçalho -->
    <header class="bg-vinho-500 text-white py-8 px-4 shadow-lg">
        <div class="container mx-auto text-center">
            <h1 class="text-[clamp(1.8rem,4vw,3.2rem)] font-bold">Agro e Sustentabilidade</h1>
            <p class="text-[clamp(1rem,2vw,1.4rem)] mt-2">Por Laura Cristina</p>
        </div>

        <!-- Botões de acessibilidade -->
        <div class="container mx-auto mt-6 flex flex-wrap gap-3 justify-center">
            <button id="aumentarTexto" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-font"></i> Aumentar texto
            </button>
            <button id="diminuirTexto" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-font fa-rotate-180"></i> Diminuir texto
            </button>
            <button id="contrasteNormal" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-adjust"></i> Contraste normal
            </button>
            <button id="contrasteAlto" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-sun-o"></i> Alto contraste
            </button>
            <button id="contrasteBaixo" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-moon-o"></i> Baixo contraste
            </button>
        </div>
    </header>

    <!-- Conteúdo Principal -->
    <main class="container mx-auto px-4 py-10">
        <!-- Texto breve sobre sustentabilidade -->
        <section class="mb-12 max-w-3xl mx-auto text-center">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-4">O que é agro e sustentabilidade?</h2>
            <p class="texto-normal leading-relaxed">
                A agropecuária sustentável é um modelo de produção que busca aliar a criação de alimentos, fibras e energia com a preservação do meio ambiente, o uso consciente dos recursos naturais e o bem-estar das pessoas e comunidades rurais. Ela não esgota o solo, não polui a água e garante que as gerações futuras também possam produzir e viver bem. Quer saber tudo detalhadamente? Clique no botão abaixo!
            </p>
            <a href="explorar.html" class="inline-block mt-6 bg-vinho-500 text-white px-8 py-3 rounded-lg font-medium hover:bg-vinho-600 transition shadow-md">
                Explorar Mais
            </a>
        </section>

        <!-- Seção de Fotos -->
        <section class="mb-16">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-6 text-center">Imagens do Campo Sustentável</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
                <img src="https://picsum.photos/id/1072/600/400" alt="Plantação com manejo sustentável" class="rounded-lg shadow-md w-full h-60 object-cover hover:scale-[1.02] transition">
                <img src="https://picsum.photos/id/1084/600/400" alt="Preservação de nascentes na propriedade" class="rounded-lg shadow-md w-full h-60 object-cover hover:scale-[1.02] transition">
                <img src="https://picsum.photos/id/1023/600/400" alt="Criação de animais em sistema integrado" class="rounded-lg shadow-md w-full h-60 object-cover hover:scale-[1.02] transition">
            </div>
        </section>

        <!-- Seção de Vídeos -->
        <section class="mb-16">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-6 text-center">Vídeos Explicativos</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 max-w-4xl mx-auto">
                <div class="aspect-video rounded-lg overflow-hidden shadow-md">
                    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/8yH7wO8wX7s" title="Agricultura Sustentável" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
                <div class="aspect-video rounded-lg overflow-hidden shadow-md">
                    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/9Xa3rF5eR8c" title="Agro e Meio Ambiente" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>
        </section>

        <!-- Seção de Gráficos -->
        <section class="mb-10">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-6 text-center">Dados e Gráficos</h2>
            <div class="bg-white p-6 rounded-lg shadow-md max-w-2xl mx-auto">
                <h3 class="text-lg font-medium text-vinho-500 mb-4">Uso de Práticas Sustentáveis no Brasil</h3>
                <svg width="100%" height="250" viewBox="0 0 400 250">
                    <!-- Eixos -->
                    <line x1="50" y1="200" x2="350" y2="200" stroke="#992647" stroke-width="2"/>
                    <line x1="50" y1="20" x2="50" y2="200" stroke="#992647" stroke-width="2"/>
                    
                    <!-- Barras -->
                    <rect x="80" y="80" width="60" height="120" fill="#992647" opacity="0.8"/>
                    <rect x="170" y="110" width="60" height="90" fill="#b34a66" opacity="0.8"/>
                    <rect x="260" y="50" width="60" height="150" fill="#7a1e39" opacity="0.8"/>
                    
                    <!-- Rótulos -->
                    <text x="110" y="220" text-anchor="middle" font-size="12">Rotação de Culturas</text>
                    <text x="200" y="220" text-anchor="middle" font-size="12">Adubação Orgânica</text>
                    <text x="290" y="220" text-anchor="middle" font-size="12">Preservação de Áreas</text>
                    
                    <!-- Valores -->
                    <text x="110" y="75" text-anchor="middle" font-size="12" fill="#992647">60%</text>
                    <text x="200" y="105" text-anchor="middle" font-size="12" fill="#992647">45%</text>
                    <text x="290" y="45" text-anchor="middle" font-size="12" fill="#992647">75%</text>
                </svg>
                <p class="text-center text-sm text-gray-600 mt-2">Fonte: Dados IBGE - 2025</p>
            </div>
        </section>
    </main>

    <!-- Rodapé -->
    <footer class="bg-vinho-700 text-white py-6 px-4 text-center">
        <p>© 2026 Agro e Sustentabilidade - Criado por Laura Cristina</p>
    </footer>

    <!-- Script dos botões funcionais -->
    <script>
        const corpo = document.getElementById('corpo');
        let tamanhoAtual = 0; // 0 = normal, 1 = maior, 2 = muito maior

        // Aumentar texto
        document.getElementById('aumentarTexto').addEventListener('click', () => {
            corpo.classList.remove('texto-normal', 'texto-maior', 'texto-muito-maior');
            tamanhoAtual = Math.min(tamanhoAtual + 1, 2);
            if(tamanhoAtual === 0) corpo.classList.add('texto-normal');
            if(tamanhoAtual === 1) corpo.classList.add('texto-maior');
            if(tamanhoAtual === 2) corpo.classList.add('texto-muito-maior');
        });

        // Diminuir texto
        document.getElementById('diminuirTexto').addEventListener('click', () => {
            corpo.classList.remove('texto-normal', 'texto-maior', 'texto-muito-maior');
            tamanhoAtual = Math.max(tamanhoAtual - 1, 0);
            if(tamanhoAtual === 0) corpo.classList.add('texto-normal');
            if(tamanhoAtual === 1) corpo.classList.add('texto-maior');
            if(tamanhoAtual === 2) corpo.classList.add('texto-muito-maior');
        });

        // Contrastes
        document.getElementById('contrasteNormal').addEventListener('click', () => {
            corpo.classList.remove('contraste-alto', 'contraste-baixo');
            corpo.classList.add('contraste-normal');
        });

        document.getElementById('contrasteAlto').addEventListener('click', () => {
            corpo.classList.remove('contraste-normal', 'contraste-baixo');
            corpo.classList.add('contraste-alto');
        });

        document.getElementById('contrasteBaixo').addEventListener('click', () => {
            corpo.classList.remove('contraste-normal', 'contraste-alto');
            corpo.classList.add('contraste-baixo');
        });
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Explorar | Agro e Sustentabilidade - Laura Cristina</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        vinho: {
                            50: '#f9f0f2',
                            100: '#f0d6dc',
                            200: '#e0adb8',
                            300: '#cc7a8f',
                            400: '#b34a66',
                            500: '#992647',
                            600: '#7a1e39',
                            700: '#5c172b',
                            800: '#3d0f1d',
                            900: '#1f080f',
                        },
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .texto-normal { font-size: 1rem; }
            .texto-maior { font-size: 1.15rem; }
            .texto-muito-maior { font-size: 1.3rem; }
            .contraste-normal { filter: contrast(100%); }
            .contraste-alto { filter: contrast(150%); }
            .contraste-baixo { filter: contrast(70%); }
        }
    </style>
</head>
<body class="bg-vinho-50 text-vinho-900 font-sans transition-all duration-300" id="corpo">
    <!-- Cabeçalho -->
    <header class="bg-vinho-500 text-white py-8 px-4 shadow-lg">
        <div class="container mx-auto text-center">
            <h1 class="text-[clamp(1.8rem,4vw,3.2rem)] font-bold">Tudo sobre Agro e Sustentabilidade</h1>
            <p class="text-[clamp(1rem,2vw,1.4rem)] mt-2">Por Laura Cristina</p>
        </div>

        <!-- Botões de acessibilidade -->
        <div class="container mx-auto mt-6 flex flex-wrap gap-3 justify-center">
            <button id="aumentarTexto" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-font"></i> Aumentar texto
            </button>
            <button id="diminuirTexto" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-font fa-rotate-180"></i> Diminuir texto
            </button>
            <button id="contrasteNormal" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-adjust"></i> Contraste normal
            </button>
            <button id="contrasteAlto" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-sun-o"></i> Alto contraste
            </button>
            <button id="contrasteBaixo" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-moon-o"></i> Baixo contraste
            </button>
        </div>

        <!-- Botão voltar -->
        <div class="container mx-auto mt-4 text-center">
            <a href="index.html" class="inline-block bg-vinho-700 text-white px-4 py-2 rounded-lg hover:bg-vinho-800 transition">
                <i class="fa fa-arrow-left"></i> Voltar para página inicial
            </a>
        </div>
    </header>

    <!-- Conteúdo detalhado -->
    <main class="container mx-auto px-4 py-10 max-w-4xl">
        <section class="mb-10">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-4">O que é Agro e Sustentabilidade?</h2>
            <p class="texto-normal leading-relaxed mb-4">
                A agropecuária sustentável, ou simplesmente agro sustentável, é um sistema de produção agrícola e pecuário que tem como princípio principal atender às necessidades atuais de alimentos, matérias-primas e renda, sem comprometer a capacidade das gerações futuras de também usufruir dos recursos naturais. Ela une a produção econômica com a preservação ambiental e a justiça social.
            </p>
            <p class="texto-normal leading-relaxed">
                Diferente da agricultura convencional que muitas vezes explora o solo e usa muitos produtos químicos, a sustentabilidade no agro busca equilíbrio: produzir bem, cuidar da terra, da água, da biodiversidade e valorizar quem trabalha no campo.
            </p>
        </section>

        <section class="mb-10">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-4">Princípios Fundamentais</h2>
            <ul class="list-disc pl-6 space-y-2 leading-relaxed">
                <li><strong>Preservação dos recursos naturais:</strong> Uso consciente da água, proteção do solo contra erosão e manutenção de matas ciliares e nascentes.</li>
                <li><strong>Boa saúde do solo:</strong> Práticas como rotação de culturas, adubação orgânica e plantio direto para manter a fertilidade sem esgotar.</li>
                <li><strong>Uso moderado de insumos:</strong> Redução de agrotóxicos e fertilizantes químicos, usando alternativas naturais e controle biológico de pragas.</li>
                <li><strong>Bem-estar animal:</strong> Criação de animais em condições adequadas, respeitando seu comportamento natural e saúde.</li>
                <li><strong>Valorização das pessoas:</strong> Condições dignas de trabalho, geração de renda para o produtor e respeito às comunidades rurais e tradicionais.</li>
                <li><strong>Biodiversidade:</strong> Manter diferentes espécies de plantas e animais, pois isso fortalece o ecossistema e reduz riscos de pragas e doenças.</li>
            </ul>
        </section>

        <section class="mb-10">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-4">Práticas Comuns de Sustentabilidade</h2>
            <p class="texto-normal leading-relaxed mb-3">Algumas das técnicas mais usadas no Brasil e no mundo:</p>
            <ul class="list-circle pl-6 space-y-2 leading-relaxed">
                <li><strong>Plantio Direto:</strong> Não revolve o solo, mantém os restos de culturas anteriores na superfície — protege contra erosão e retém água.</li>
                <li><strong>Integração Lavoura-Pecuária-Floresta (ILPF):</strong> Combina cultivo de grãos, criação de animais e árvores na mesma área, aproveitando melhor o espaço e os recursos.</li>
                <li><strong>Agrofloresta:</strong> Cultivo de plantas agrícolas junto com espécies florestais, imitando a estrutura da floresta natural — ótimo para biodiversidade.</li>
                <li><strong>Captação e reúso de água:</strong> Construção de barragens, cisternas e sistemas para aproveitar água da chuva.</li>
                <li><strong>Energia renovável:</strong> Uso de energia solar, eólica ou biomassa nas propriedades, reduzindo impacto ambiental.</li>
            </ul>
        </section>

        <section class="mb-10">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-4">Por que isso é tão importante?</h2>
            <p class="texto-normal leading-relaxed mb-3">
                O Brasil é um dos maiores produtores de alimentos do mundo, e o agro é uma das bases da nossa economia. Mas produzir sem sustentabilidade traz riscos sérios:
            </p>
            <ul class="list-disc pl-6 space-y-1 mb-4">
                <li>Desgaste e perda de fertilidade do solo</li>
                <li>Escassez e poluição da água</li>
                <li>Perda de espécies animais e vegetais</li>
                <li>Danos à saúde de quem trabalha e de quem consome os alimentos</li>
            </ul>
            <p class="texto-normal leading-relaxed">
                Já a agricultura sustentável garante que possamos continuar produzindo alimentos de qualidade, preservando o meio ambiente, gerando emprego e renda, e cumprindo nosso papel de cuidar do planeta. Além disso, produtos vindos de sistemas sustentáveis são cada vez mais valorizados no mercado nacional e internacional.
            </p>
        </section>

        <section>
            <h2 class="text-2xl font-semibold text-vinho-600 mb-4">O Futuro é Agro + Sustentabilidade</h2>
            <p class="texto-normal leading-relaxed">
                A tecnologia também ajuda: hoje temos sensores no solo, satélites, sementes mais resistentes e softwares que ajudam o produtor a usar apenas o necessário de água e insumos. O agro moderno é inovador, eficiente e consciente. E o principal: ele mostra que é possível sim produzir muito e bem, ao mesmo tempo em que cuida da natureza.
            </p>
        </section>
    </main>

    <!-- Rodapé -->
    <footer class="bg-vinho-700 text-white py-6 px-4 text-center">
        <p>© 2026 Agro e Sustentabilidade - Criado por Laura Cristina</p>
    </footer>

    <!-- Script dos botões funcionais (mesmo da página inicial) -->
    <script>
        const corpo = document.getElementById('corpo');
        let tamanhoAtual = 0;

        document.getElementById('aumentarTexto').addEventListener('click', () => {
            corpo.classList.remove('texto-normal', 'texto-maior', 'texto-muito-maior');
            tamanhoAtual = Math.min(tamanhoAtual + 1, 2);
            if(tamanhoAtual === 0) corpo.classList.add('texto-normal');
            if(tamanhoAtual === 1) corpo.classList.add('texto-maior');
            if(tamanhoAtual === 2) corpo.classList.add('texto-muito-maior');
        });

        document.getElementById('diminuirTexto').addEventListener('click', () => {
            corpo.classList.remove('texto-normal', 'texto-maior', 'texto-muito-maior');
            tamanhoAtual = Math.max(tamanhoAtual - 1, 0);
            if(tamanhoAtual === 0) corpo.classList.add('texto-normal');
            if(tamanhoAtual === 1) corpo.classList.add('texto-maior');
            if(tamanhoAtual === 2) corpo.classList.add('texto-muito-maior');
        });

        document.getElementById('contrasteNormal').addEventListener('click', () => {
            corpo.classList.remove('contraste-alto', 'contraste-baixo');
            corpo.classList.add('contraste-normal');
        });

        document.getElementById('contrasteAlto').addEventListener('click', () => {
            corpo.classList.remove('contraste-normal', 'contraste-baixo');
            corpo.classList.add('contraste-alto');
        });

        document.getElementById('contrasteBaixo').addEventListener('click', () => {
            corpo.classList.remove('contraste-normal', 'contraste-alto');
            corpo.classList.add('contraste-baixo');
        });
    </script>
</body>
</html>
