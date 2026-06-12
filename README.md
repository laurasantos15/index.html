<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agro e Sua Importância | Laura Cristina</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        // Paleta de cores: Azul Marinho
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        marinho: {
                            50: '#f0f4f8',
                            100: '#d9e2ed',
                            200: '#b3c6db',
                            300: '#80a2c7',
                            400: '#4d7eb3',
                            500: '#1a5a9f', // Azul marinho principal
                            600: '#15487f',
                            700: '#10365f',
                            800: '#0b243f',
                            900: '#05121f',
                        },
                    },
                    fontFamily: {
                        sans: ['Inter', 'Roboto', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .texto-p { font-size: 1rem; line-height: 1.6; }
            .texto-m { font-size: 1.15rem; line-height: 1.7; }
            .texto-g { font-size: 1.3rem; line-height: 1.8; }
            .contraste-n { filter: contrast(100%); }
            .contraste-a { filter: contrast(160%); }
            .contraste-b { filter: contrast(70%); }
            .sombra-profissional { box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08); }
            .transicao { transition: all 0.3s ease; }
            .oculto { display: none !important; }
        }
    </style>
</head>
<body class="bg-marinho-50 text-marinho-900 font-sans transicao contraste-n texto-p" id="corpo">

    <!-- BOTÕES DE ACESSIBILIDADE (FIXO NO TOPO) -->
    <div class="bg-marinho-800 text-white py-3 px-4 sticky top-0 z-50 sombra-profissional">
        <div class="container mx-auto flex flex-wrap gap-3 justify-center items-center">
            <span class="text-sm font-medium">Acessibilidade:</span>
            <button id="btnAumentar" class="bg-marinho-500 hover:bg-marinho-400 px-3 py-1.5 rounded transicao">
                <i class="fa fa-font"></i> Aumentar
            </button>
            <button id="btnDiminuir" class="bg-marinho-500 hover:bg-marinho-400 px-3 py-1.5 rounded transicao">
                <i class="fa fa-font fa-rotate-180"></i> Diminuir
            </button>
            <button id="btnContrasteN" class="bg-marinho-500 hover:bg-marinho-400 px-3 py-1.5 rounded transicao">
                <i class="fa fa-adjust"></i> Contraste Normal
            </button>
            <button id="btnContrasteA" class="bg-marinho-500 hover:bg-marinho-400 px-3 py-1.5 rounded transicao">
                <i class="fa fa-sun-o"></i> Alto Contraste
            </button>
            <button id="btnContrasteB" class="bg-marinho-500 hover:bg-marinho-400 px-3 py-1.5 rounded transicao">
                <i class="fa fa-moon-o"></i> Baixo Contraste
            </button>
        </div>
    </div>

    <!-- ==========================================
         PÁGINA INICIAL
    ========================================== -->
    <section id="paginaInicial" class="min-h-screen">
        <!-- Cabeçalho -->
        <header class="bg-marinho-500 text-white py-16 px-4">
            <div class="container mx-auto text-center">
                <h1 class="text-[clamp(2rem,5vw,4rem)] font-bold mb-3">Agro e Sua Importância</h1>
                <p class="text-[clamp(1rem,2vw,1.3rem)] opacity-90">Por Laura Cristina</p>
            </div>
        </header>

        <!-- Conteúdo Inicial -->
        <main class="container mx-auto px-4 py-16 max-w-3xl">
            <div class="bg-white p-8 rounded-xl sombra-profissional">
                <h2 class="text-2xl font-semibold text-marinho-600 mb-5">O que é e por que é essencial?</h2>
                
                <p class="mb-4">
                    O agronegócio vai muito além do plantio e da criação de animais: ele é a base da economia, da alimentação e da vida em sociedade. É o setor que garante comida na mesa, gera empregos, movimenta o mercado e sustenta o desenvolvimento do país.
                </p>

                <p class="mb-6">
                    Além de produzir, o agro moderno se preocupa com sustentabilidade, uso consciente dos recursos naturais e preservação ambiental. Sem o agro, não há abastecimento, não há renda e não há progresso.
                </p>

                <!-- Botão Explorar Mais -->
                <button id="btnExplorar" class="w-full bg-marinho-500 hover:bg-marinho-600 text-white font-medium py-3 px-6 rounded-lg text-lg transicao sombra-profissional">
                    Explorar Mais <i class="fa fa-arrow-right ml-2"></i>
                </button>
            </div>
        </main>

        <!-- Rodapé Inicial -->
        <footer class="bg-marinho-800 text-white py-6 text-center">
            <p>© 2026 Agro e Sua Importância - Trabalho Acadêmico | Laura Cristina</p>
        </footer>
    </section>


    <!-- ==========================================
         PÁGINA EXPLORAR MAIS (DETALHADA)
    ========================================== -->
    <section id="paginaExplorar" class="min-h-screen oculto">
        <!-- Cabeçalho -->
        <header class="bg-marinho-500 text-white py-12 px-4">
            <div class="container mx-auto text-center">
                <h1 class="text-[clamp(1.8rem,4vw,3rem)] font-bold mb-2">Tudo sobre o Agro e Sua Importância</h1>
                <p class="opacity-90">Explicação Completa | Acadêmico e Detalhado</p>
                <button id="btnVoltar" class="mt-6 bg-white text-marinho-500 hover:bg-marinho-50 px-4 py-2 rounded-lg transicao">
                    <i class="fa fa-arrow-left"></i> Voltar para página inicial
                </button>
            </div>
        </header>

        <!-- Conteúdo Completo -->
        <main class="container mx-auto px-4 py-16 max-w-5xl">
            <div class="space-y-16">

                <!-- SEÇÃO 1: CONCEITO GERAL -->
                <div class="bg-white p-8 rounded-xl sombra-profissional">
                    <h2 class="text-2xl font-bold text-marinho-600 mb-6">1. Conceito e Definição</h2>
                    <p class="mb-4">
                        O agronegócio é o conjunto de todas as atividades econômicas ligadas à produção, processamento, distribuição e comercialização de produtos derivados da agricultura, pecuária, silvicultura e extrativismo. Ele envolve desde o produtor rural até a indústria, o comércio e o consumidor final.
                    </p>
                    <p class="mb-4">
                        No Brasil, o agro é um dos pilares da economia, responsável por grande parte do Produto Interno Bruto (PIB), das exportações e da geração de empregos diretos e indiretos. Não é apenas um setor, mas um sistema que conecta o campo à cidade.
                    </p>
                    <img src="https://images.unsplash.com/photo-1560493631-97b20efd53d1?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" 
                         alt="Campo produtivo representando o agronegócio" 
                         class="w-full h-[350px] object-cover rounded-lg mt-6">
                </div>


                <!-- SEÇÃO 2: IMPORTÂNCIA ECONÔMICA -->
                <div class="bg-white p-8 rounded-xl sombra-profissional">
                    <h2 class="text-2xl font-bold text-marinho-600 mb-6">2. Importância Econômica</h2>
                    <p class="mb-4">
                        O agro é o grande motor da economia brasileira. Ele é responsável por:
                    </p>
                    <ul class="list-disc pl-6 space-y-2 mb-6">
                        <li>Geração de mais de 20 milhões de empregos em todo o país;</li>
                        <li>Ser o principal setor exportador, vendendo para mais de 200 nações;</li>
                        <li>Movimentar cadeias industriais (alimentos, têxtil, energia, biocombustíveis);</li>
                        <li>Reduzir a dependência externa e fortalecer a balança comercial.</li>
                    </ul>

                    <!-- GRÁFICO PROFISSIONAL 1 -->
                    <div class="mt-8 p-6 bg-marinho-50 rounded-lg">
                        <h3 class="text-lg font-semibold text-marinho-700 mb-4">Participação do Agro no PIB Brasileiro (%)</h3>
                        <svg width="100%" height="300" viewBox="0 0 500 300">
                            <!-- Eixos -->
                            <line x1="60" y1="240" x2="460" y2="240" stroke="#1a5a9f" stroke-width="3"/>
                            <line x1="60" y1="30" x2="60" y2="240" stroke="#1a5a9f" stroke-width="3"/>
                            
                            <!-- Barras -->
                            <rect x="100" y="80" width="80" height="160" fill="#1a5a9f" opacity="0.9" rx="4"/>
                            <rect x="210" y="110" width="80" height="130" fill="#4d7eb3" opacity="0.9" rx="4"/>
                            <rect x="320" y="50" width="80" height="190" fill="#0b243f" opacity="0.9" rx="4"/>
                            
                            <!-- Rótulos -->
                            <text x="140" y="265" text-anchor="middle" font-size="14" font-weight="500">2022</text>
                            <text x="250" y="265" text-anchor="middle" font-size="14" font-weight="500">2023</text>
                            <text x="360" y="265" text-anchor="middle" font-size="14" font-weight="500">2024</text>
                            
                            <!-- Valores -->
                            <text x="140" y="70" text-anchor="middle" font-size="15" font-weight="bold" fill="#1a5a9f">24,8%</text>
                            <text x="250" y="100" text-anchor="middle" font-size="15" font-weight="bold" fill="#1a5a9f">22,3%</text>
                            <text x="360" y="40" text-anchor="middle" font-size="15" font-weight="bold" fill="#1a5a9f">27,1%</text>
                            
                            <text x="250" y="290" text-anchor="middle" font-size="13" fill="#666">Fonte: IBGE - Dados Estatísticos</text>
                        </svg>
                    </div>
                </div>


                <!-- SEÇÃO 3: SEGURANÇA ALIMENTAR -->
                <div class="bg-white p-8 rounded-xl sombra-profissional">
                    <h2 class="text-2xl font-bold text-marinho-600 mb-6">3. Segurança Alimentar</h2>
                    <p class="mb-4">
                        A função mais essencial do agro é produzir alimentos. O Brasil é um dos maiores produtores e exportadores de alimentos do mundo, ajudando a alimentar não só sua população, mas também milhões de pessoas em outros países.
                    </p>
                    <p class="mb-4">
                        Segurança alimentar significa garantir que todas as pessoas tenham acesso a comida de qualidade, em quantidade suficiente e de forma permanente. Sem uma agricultura forte, não existe soberania alimentar.
                    </p>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mt-6">
                        <img src="https://images.unsplash.com/photo-1593113616828-6f22ca0423c0?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Produção de alimentos saudáveis" class="w-full h-60 object-cover rounded-lg">
                        <img src="https://images.unsplash.com/photo-1623243505160-7b040073c78a?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" alt="Colheita de grãos e alimentos" class="w-full h-60 object-cover rounded-lg">
                    </div>
                </div>


                <!-- SEÇÃO 4: SUSTENTABILIDADE E MEIO AMBIENTE -->
                <div class="bg-white p-8 rounded-xl sombra-profissional">
                    <h2 class="text-2xl font-bold text-marinho-600 mb-6">4. Agro e Sustentabilidade</h2>
                    <p class="mb-4">
                        O agro moderno evoluiu: hoje, produzir e preservar andam juntos. A sustentabilidade no campo significa usar os recursos naturais — solo, água, biodiversidade — de forma consciente, para que não se esgotem e possam ser usados pelas gerações futuras.
                    </p>
                    <p class="mb-4">
                        Práticas como plantio direto, rotação de culturas, integração lavoura-pecuária-floresta, reúso de água e energia renovável são cada vez mais usadas. O agro é, também, guardião de florestas e áreas preservadas.
                    </p>

                    <!-- GRÁFICO PROFISSIONAL 2 -->
                    <div class="mt-8 p-6 bg-marinho-50 rounded-lg">
                        <h3 class="text-lg font-semibold text-marinho-700 mb-4">Uso de Práticas Sustentáveis no Brasil</h3>
                        <svg width="100%" height="300" viewBox="0 0 500 300">
                            <!-- Gráfico de Pizza -->
                            <circle cx="250" cy="150" r="100" fill="none" stroke="#eee" stroke-width="1"/>
                            
                            <!-- Partes -->
                            <path d="M250,150 L250,50 A100,100 0 0,1 385,100 Z" fill="#1a5a9f"/>
                            <path d="M250,150 L385,100 A100,100 0 0,1 400,200 Z" fill="#4d7eb3"/>
                            <path d="M250,150 L400,200 A100,100 0 0,1 200,240 Z" fill="#80a2c7"/>
                            <path d="M250,150 L200,240 A100,100 0 0,1 250,50 Z" fill="#0b243f"/>
                            
                            <!-- Legenda -->
                            <rect x="370" y="60" width="15" height="15" fill="#1a5a9f"/>
                            <text x="390" y="72" font-size="13">Plantio Direto (35%)</text>
                            
                            <rect x="370" y="90" width="15" height="15" fill="#4d7eb3"/>
                            <text x="390" y="102" font-size="13">Adubação Orgânica (20%)</text>
                            
                            <rect x="370" y="120" width="15" height="15" fill="#80a2c7"/>
                            <text x="390" y="132" font-size="13">Rotação de Culturas (25%)</text>
                            
                            <rect x="370" y="150" width="15" height="15" fill="#0b243f"/>
                            <text x="390" y="162" font-size="13">Preservação de Áreas (20%)</text>

                            <text x="250" y="270" text-anchor="middle" font-size="13" fill="#666">Dados: Embrapa - Pesquisa Nacional</text>
                        </svg>
                    </div>
                </div>


                <!-- SEÇÃO 5: TECNOLOGIA E FUTURO -->
                <div class="bg-white p-8 rounded-xl sombra-profissional">
                    <h2 class="text-2xl font-bold text-marinho-600 mb-6">5. Tecnologia e Futuro do Agro</h2>
                    <p class="mb-4">
                        O agro brasileiro é referência mundial em tecnologia. O uso de inteligência artificial, satélites, sensores, biotecnologia e máquinas modernas permite produzir mais, com melhor qualidade e menor impacto ambiental.
                    </p>
                    <p class="mb-4">
                        O futuro é digital e sustentável: agricultura de precisão, energia limpa, bioinsumos e cadeias produtivas inteligentes. O agro continuará sendo fundamental para o Brasil e para o mundo, evoluindo sempre.
                    </p>
                    <img src="https://images.unsplash.com/photo-1611262564516-96b7d5a3c3f6?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" 
                         alt="Tecnologia aplicada no agronegócio" 
                         class="w-full h-[300px] object-cover rounded-lg mt-6">
                </div>


                <!-- CONCLUSÃO -->
                <div class="bg-marinho-50 p-8 rounded-xl sombra-profissional border-l-4 border-marinho-500">
                    <h2 class="text-2xl font-bold text-marinho-600 mb-4">Conclusão</h2>
                    <p>
                        O agro é muito mais do que trabalho no campo: é desenvolvimento, é alimento, é renda, é tecnologia e é cuidado com o planeta. Sua importância é estratégica para o Brasil e essencial para a vida humana. Valorizar e investir no agronegócio é garantir um futuro forte, seguro e sustentável para todos.
                    </p>
                </div>

            </div>
        </main>

        <!-- Rodapé Explorar -->
        <footer class="bg-marinho-800 text-white py-8 text-center">
            <p class="mb-2">Trabalho Acadêmico: Agro e Sua Importância</p>
            <p class="text-sm opacity-75">© 2026 | Laura Cristina | Todos os direitos reservados</p>
        </footer>
    </section>


    <!-- ==========================================
         SCRIPTS DE FUNCIONALIDADES
    ========================================== -->
    <script>
        const corpo = document.getElementById('corpo');
        let tamanhoTexto = 0; // 0=padrão, 1=aumentado, 2=muito aumentado

        // === TROCA DE PÁGINAS ===
        const pagInicial = document.getElementById('paginaInicial');
        const pagExplorar = document.getElementById('paginaExplorar');
        const btnExplorar = document.getElementById('btnExplorar');
        const btnVoltar = document.getElementById('btnVoltar');

        btnExplorar.addEventListener('click', () => {
            pagInicial.classList.add('oculto');
            pagExplorar.classList.remove('oculto');
            window.scrollTo(0,0);
        });

        btnVoltar.addEventListener('click', () => {
            pagExplorar.classList.add('oculto');
            pagInicial.classList.remove('oculto');
            window.scrollTo(0,0);
        });


        // === BOTÕES DE ACESSIBILIDADE ===
        // Aumentar Texto
        document.getElementById('btnAumentar').addEventListener('click', () => {
            corpo.classList.remove('texto-p', 'texto-m', 'texto-g');
            tamanhoTexto = Math.min(tamanhoTexto + 1, 2);
            if(tamanhoTexto === 0) corpo.classList.add('texto-p');
            if(tamanhoTexto === 1) corpo.classList.add('texto-m');
            if(tamanhoTexto === 2) corpo.classList.add('texto-g');
        });

        // Diminuir Texto
        document.getElementById('btnDiminuir').addEventListener('click', () => {
            corpo.classList.remove('texto-p', 'texto-m', 'texto-g');
            tamanhoTexto = Math.max(tamanhoTexto - 1, 0);
            if(tamanhoTexto === 0) corpo.classList.add('texto-p');
            if(tamanhoTexto === 1) corpo.classList.add('texto-m');
            if(tamanhoTexto === 2) corpo.classList.add('texto-g');
        });

        // Contrastes
        document.getElementById('btnContrasteN').addEventListener('click', () => {
            corpo.classList.remove('contraste-a', 'contraste-b');
            corpo.classList.add('contraste-n');
        });

        document.getElementById('btnContrasteA').addEventListener('click', () => {
            corpo.classList.remove('contraste-n', 'contraste-b');
            corpo.classList.add('contraste-a');
        });

        document.getElementById('btnContrasteB').addEventListener('click', () => {
            corpo.classList.remove('contraste-n', 'contraste-a');
            corpo.classList.add('contraste-b');
        });
    </script>

</body>
</html>
