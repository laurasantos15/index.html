<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agro e Sustentabilidade - Laura Cristina</title>
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
            .t1 { font-size: 1rem; }
            .t2 { font-size: 1.15rem; }
            .t3 { font-size: 1.3rem; }
            .contraste-normal { filter: contrast(100%); }
            .contraste-alto { filter: contrast(150%); }
            .contraste-baixo { filter: contrast(70%); }
        }
    </style>
</head>
<body class="bg-vinho-50 text-vinho-900 font-sans transition-all duration-300" id="pagina">
    <!-- Cabeçalho -->
    <header class="bg-vinho-500 text-white py-8 px-4 shadow-lg">
        <div class="container mx-auto text-center">
            <h1 class="text-[clamp(1.8rem,4vw,3.2rem)] font-bold">Agro e Sustentabilidade</h1>
            <p class="text-[clamp(1rem,2vw,1.4rem)] mt-2">Por Laura Cristina</p>
        </div>

        <!-- Botões de acessibilidade -->
        <div class="container mx-auto mt-6 flex flex-wrap gap-3 justify-center">
            <button id="aumentar" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-font"></i> Aumentar texto
            </button>
            <button id="diminuir" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-font fa-rotate-180"></i> Diminuir texto
            </button>
            <button id="cNormal" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-adjust"></i> Contraste normal
            </button>
            <button id="cAlto" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-sun-o"></i> Alto contraste
            </button>
            <button id="cBaixo" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-moon-o"></i> Baixo contraste
            </button>
        </div>
    </header>

    <!-- Conteúdo Principal -->
    <main class="container mx-auto px-4 py-10">
        <!-- Explicação Básica -->
        <section class="mb-12 max-w-3xl mx-auto text-center">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-4">O que é?</h2>
            <p class="t1 leading-relaxed">
                Agro e sustentabilidade significa produzir alimentos, criar animais e cultivar a terra cuidando do meio ambiente. É usar os recursos naturais — como água, solo e árvores — de forma equilibrada, para não esgotar nada e garantir que as pessoas de hoje e do futuro tenham o que comer e viver bem.
            </p>
            <a href="explorar.html" class="inline-block mt-6 bg-vinho-500 text-white px-8 py-3 rounded-lg font-medium hover:bg-vinho-600 transition shadow-md">
                Explorar Mais
            </a>
        </section>

        <!-- Fotos - TODAS SÓ DE AGRO -->
        <section class="mb-16">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-6 text-center">Imagens do Campo</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
                <img src="https://images.unsplash.com/photo-1574943320262-61d4c886b493?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Plantação sustentável" class="rounded-lg shadow-md w-full h-60 object-cover">
                <img src="https://images.unsplash.com/photo-1623243505160-7b040073c78a?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Cuidado com o solo" class="rounded-lg shadow-md w-full h-60 object-cover">
                <img src="https://images.unsplash.com/photo-1593113616828-6f22ca0423c0?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Árvore e produção rural" class="rounded-lg shadow-md w-full h-60 object-cover">
            </div>
        </section>

        <!-- Vídeos -->
        <section class="mb-16">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-6 text-center">Vídeos</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 max-w-4xl mx-auto">
                <div class="aspect-video rounded-lg overflow-hidden shadow-md">
                    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/8yH7wO8wX7s" title="Agricultura Sustentável" frameborder="0" allowfullscreen></iframe>
                </div>
                <div class="aspect-video rounded-lg overflow-hidden shadow-md">
                    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/9Xa3rF5eR8c" title="Agro e Meio Ambiente" frameborder="0" allowfullscreen></iframe>
                </div>
            </div>
        </section>

        <!-- Gráfico -->
        <section class="mb-10">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-6 text-center">Dados</h2>
            <div class="bg-white p-6 rounded-lg shadow-md max-w-2xl mx-auto">
                <h3 class="text-lg font-medium text-vinho-500 mb-4">Uso de Práticas Sustentáveis</h3>
                <svg width="100%" height="250" viewBox="0 0 400 250">
                    <line x1="50" y1="200" x2="350" y2="200" stroke="#992647" stroke-width="2"/>
                    <line x1="50" y1="20" x2="50" y2="200" stroke="#992647" stroke-width="2"/>
                    <rect x="80" y="80" width="60" height="120" fill="#992647" opacity="0.8"/>
                    <rect x="170" y="110" width="60" height="90" fill="#b34a66" opacity="0.8"/>
                    <rect x="260" y="50" width="60" height="150" fill="#7a1e39" opacity="0.8"/>
                    <text x="110" y="220" text-anchor="middle" font-size="12">Rotação de Culturas</text>
                    <text x="200" y="220" text-anchor="middle" font-size="12">Adubação Orgânica</text>
                    <text x="290" y="220" text-anchor="middle" font-size="12">Preservação de Áreas</text>
                    <text x="110" y="75" text-anchor="middle" font-size="12" fill="#992647">60%</text>
                    <text x="200" y="105" text-anchor="middle" font-size="12" fill="#992647">45%</text>
                    <text x="290" y="45" text-anchor="middle" font-size="12" fill="#992647">75%</text>
                </svg>
            </div>
        </section>
    </main>

    <!-- Rodapé -->
    <footer class="bg-vinho-700 text-white py-6 px-4 text-center">
        <p>© 2026 Agro e Sustentabilidade - Laura Cristina</p>
    </footer>

    <!-- Script dos botões -->
    <script>
        const pagina = document.getElementById('pagina');
        let tamanho = 0; // 0 = normal, 1 = maior, 2 = muito maior

        // Aumentar texto
        document.getElementById('aumentar').addEventListener('click', () => {
            pagina.classList.remove('t1','t2','t3');
            tamanho = Math.min(tamanho+1, 2);
            if(tamanho===0) pagina.classList.add('t1');
            if(tamanho===1) pagina.classList.add('t2');
            if(tamanho===2) pagina.classList.add('t3');
        });

        // Diminuir texto
        document.getElementById('diminuir').addEventListener('click', () => {
            pagina.classList.remove('t1','t2','t3');
            tamanho = Math.max(tamanho-1, 0);
            if(tamanho===0) pagina.classList.add('t1');
            if(tamanho===1) pagina.classList.add('t2');
            if(tamanho===2) pagina.classList.add('t3');
        });

        // Contrastes
        document.getElementById('cNormal').addEventListener('click', ()=>{pagina.className='bg-vinho-50 text-vinho-900 font-sans transition-all duration-300 contraste-normal';});
        document.getElementById('cAlto').addEventListener('click', ()=>{pagina.className='bg-vinho-50 text-vinho-900 font-sans transition-all duration-300 contraste-alto';});
        document.getElementById('cBaixo').addEventListener('click', ()=>{pagina.className='bg-vinho-50 text-vinho-900 font-sans transition-all duration-300 contraste-baixo';});
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
            .t1 { font-size: 1rem; }
            .t2 { font-size: 1.15rem; }
            .t3 { font-size: 1.3rem; }
            .contraste-normal { filter: contrast(100%); }
            .contraste-alto { filter: contrast(150%); }
            .contraste-baixo { filter: contrast(70%); }
        }
    </style>
</head>
<body class="bg-vinho-50 text-vinho-900 font-sans transition-all duration-300" id="pagina">
    <!-- Cabeçalho -->
    <header class="bg-vinho-500 text-white py-8 px-4 shadow-lg">
        <div class="container mx-auto text-center">
            <h1 class="text-[clamp(1.8rem,4vw,3.2rem)] font-bold">Tudo Sobre Agro e Sustentabilidade</h1>
            <p class="text-[clamp(1rem,2vw,1.4rem)] mt-2">Por Laura Cristina</p>
        </div>

        <!-- Botões de acessibilidade -->
        <div class="container mx-auto mt-6 flex flex-wrap gap-3 justify-center">
            <button id="aumentar" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-font"></i> Aumentar texto
            </button>
            <button id="diminuir" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-font fa-rotate-180"></i> Diminuir texto
            </button>
            <button id="cNormal" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-adjust"></i> Contraste normal
            </button>
            <button id="cAlto" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-sun-o"></i> Alto contraste
            </button>
            <button id="cBaixo" class="bg-white text-vinho-500 px-3 py-2 rounded-lg flex items-center gap-2 hover:bg-vinho-50 transition">
                <i class="fa fa-moon-o"></i> Baixo contraste
            </button>
        </div>

        <div class="container mx-auto mt-4 text-center">
            <a href="index.html" class="inline-block bg-vinho-700 text-white px-4 py-2 rounded-lg hover:bg-vinho-800 transition">
                <i class="fa fa-arrow-left"></i> Voltar
            </a>
        </div>
    </header>

    <!-- Conteúdo DETALHADO -->
    <main class="container mx-auto px-4 py-10 max-w-4xl">
        <section class="mb-12">
            <h2 class="text-2xl font-semibold text-vinho-600 mb-4">📘 Explicação Completa e Específica</h2>
            
            <h3 class="text-xl font-medium text-vinho-500 mt-6 mb-2">1. O que é Agro e Sustentabilidade?</h3>
            <p class="t1 leading-relaxed mb-3">
                Agro e sustentabilidade é um modelo de produção agrícola, pecuária e florestal que busca produzir alimentos, fibras, energia e matérias-primas, ao mesmo tempo que preserva o meio ambiente, protege os recursos naturais (solo, água, ar, biodiversidade) e garante condições dignas de vida e trabalho para as pessoas do campo.
            </p>
            <p class="t1 leading-relaxed mb-4">
                Diferente da agricultura convencional que pode usar muitos produtos químicos e explorar a terra até esgotá-la, a sustentabilidade no agro trabalha com o equilíbrio: produzir bem hoje, sem acabar com o que é necessário para o futuro.
            </p>

            <img src="https://images.unsplash.com/photo-1560493631-97b20efd53d1?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Produção sustentável" class="rounded-lg shadow-md w-full h-64 object-cover mb-6">


            <h3 class="text-xl font-medium text-vinho-500 mt-6 mb-2">2. Princípios Fundamentais</h3>
            <ul class="list-disc pl-6 space-y-2 mb-6 t1">
                <li><strong>Preservação dos recursos naturais:</strong> Proteger nascentes, matas ciliares, florestas e usar água com moderação.</li>
                <li><strong>Conservação do solo:</strong> Evitar erosão, manter a matéria orgânica e não deixar a terra "nua" sem proteção.</li>
                <li><strong>Uso racional de insumos:</strong> Reduzir agrotóxicos, usar adubos naturais e controle biológico de pragas.</li>
                <li><strong>Biodiversidade:</strong> Plantar diferentes culturas, manter árvores e espécies animais — isso deixa o sistema mais forte.</li>
                <li><strong>Justiça social:</strong> Respeitar o trabalhador rural, pagar justo e valorizar a cultura do campo.</li>
                <li><strong>Economia de baixo carbono:</strong> Diminuir emissões e usar energia renovável (sol, vento, biomassa).</li>
            </ul>


            <h3 class="text-xl font-medium text-vinho-500 mt-6 mb-2">3. Principais Práticas Sustentáveis</h3>
            <p class="t1 mb-3">Essas são as técnicas mais usadas no Brasil e no mundo:</p>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mb-6">
                <div class="bg-white p-4 rounded-lg shadow">
                    <strong>🌱 Plantio Direto</strong>
                    <p>Não revolve o solo, deixa restos da planta anterior cobrindo a terra. Evita erosão e segura água.</p>
                </div>
                <div class="bg-white p-4 rounded-lg shadow">
                    <strong>🌳 ILPF</strong>
                    <p>Integração Lavoura-Pecuária-Floresta: juntar plantio, criação de animais e árvores na mesma área.</p>
                </div>
                <div class="bg-white p-4 rounded-lg shadow">
                    <strong>🍀 Agrofloresta</strong>
                    <p>Imita a floresta natural: plantas de diferentes alturas, frutas, madeira e alimentos juntos.</p>
                </div>
                <div class="bg-white p-4 rounded-lg shadow">
                    <strong>💧 Captação de água</strong>
                    <p>Armazenar água da chuva em cisternas, barragens e bacias para usar na seca.</p>
                </div>
            </div>

            <img src="https://images.unsplash.com/photo-1611262564516-96b7d5a3c3f6?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Práticas sustentáveis" class="rounded-lg shadow-md w-full h-64 object-cover mb-6">


            <h3 class="text-xl font-medium text-vinho-500 mt-6 mb-2">4. Por que isso é importante?</h3>
            <p class="t1 leading-relaxed mb-3">
                O Brasil é um dos maiores produtores de alimentos do planeta. Se produzirmos sem cuidado, corremos risco de:
            </p>
            <ul class="list-disc pl-6 space-y-1 mb-4 t1">
                <li>Acabar com a água potável</li>
                <li>Deixar o solo infértil e improdutivo</li>
                <li>Perder espécies de plantas e animais</li>
                <li>Poluir rios, ar e alimentos</li>
                <li>Prejudicar a saúde de quem trabalha e de quem come</li>
            </ul>
            <p class="t1 leading-relaxed mb-6">
                Já o agro sustentável garante produção contínua, alimentos mais saudáveis, renda melhor para o produtor e um planeta preservado para todos.
            </p>


            <h3 class="text-xl font-medium text-vinho-500 mt-6 mb-2">5. Tecnologia e Sustentabilidade</h3>
            <p class="t1 leading-relaxed mb-4">
                Hoje, tecnologia ajuda muito: sensores no solo que medem umidade, satélites que monitoram o crescimento das plantas, sementes mais resistentes ao clima, energia solar nas fazendas e softwares que ensinam o produtor a usar só o que precisa. O agro moderno é inteligente, eficiente e amigo da natureza.
            </p>


            <h3 class="text-xl font-medium text-vinho-500 mt-6 mb-4">📺 Vídeos Explicativos Completos</h3>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
                <div class="aspect-video rounded-lg overflow-hidden shadow-md">
                    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/8yH7wO8wX7s" title="Explicação Agricultura Sustentável" frameborder="0" allowfullscreen></iframe>
                </div>
                <div class="aspect-video rounded-lg overflow-hidden shadow-md">
                    <iframe width="100%" height="100%" src="https://www.youtube.com/embed/9Xa3rF5eR8c" title="Agro e Preservação Ambiental" frameborder="0" allowfullscreen></iframe>
                </div>
            </div>


            <h3 class="text-xl font-medium text-vinho-500 mt-6 mb-2">✅ Conclusão</h3>
            <p class="t1 leading-relaxed">
                Agro e sustentabilidade não é só uma moda, é uma necessidade. É mostrar que podemos sim ter muita produção, desenvolvimento econômico e qualidade de vida, tudo isso cuidando da natureza. O futuro do Brasil e do mundo passa por um agro forte, limpo e sustentável.
            </p>
        </section>
    </main>

    <!-- Rodapé -->
    <footer class="bg-vinho-700 text-white py-6 px-4 text-center">
        <p>© 2026 Agro e Sustentabilidade - Laura Cristina</p>
    </footer>

    <!-- Script dos botões -->
    <script>
        const pagina = document.getElementById('pagina');
        let tamanho = 0;

        document.getElementById('aumentar').addEventListener('click', () => {
            pagina.classList.remove('t1','t2','t3');
            tamanho = Math.min(tamanho+1, 2);
            if(tamanho===0) pagina.classList.add('t1');
            if(tamanho===1) pagina.classList.add('t2');
            if(tamanho===2) pagina.classList.add('t3');
        });

        document.getElementById('diminuir').addEventListener('click', () => {
            pagina.classList.remove('t1','t2','t3');
            tamanho = Math.max(tamanho-1, 0);
            if(tamanho===0) pagina.classList.add('t1');
            if(tamanho===1) pagina.classList.add('t2');
            if(tamanho===2) pagina.classList.add('t3');
        });

        document.getElementById('cNormal').addEventListener('click', ()=>{pagina.className='bg-vinho-50 text-vinho-900 font-sans transition-all duration-300 contraste-normal';});
        document.getElementById('cAlto').addEventListener('click', ()=>{pagina.className='bg-vinho-50 text-vinho-900 font-sans transition-all duration-300 contraste-alto';});
        document.getElementById('cBaixo').addEventListener('click', ()=>{pagina.className='bg-vinho-50 text-vinho-900 font-sans transition-all duration-300 contraste-baixo';});
    </script>
</body>
</html>
