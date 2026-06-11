<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>A Importância do Agro - Laura</title>

<style>
:root{
    --vermelho-principal:#B71C1C;
    --vermelho-secundario:#D32F2F;
    --vermelho-claro:#FFCDD2;
    --fundo:#FFF8F8;
    --texto:#111111;
    --branco:#FFFFFF;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family: Arial, Helvetica, sans-serif;
    background: var(--fundo);
    color: var(--texto);
    line-height: 1.8;
    font-size: 20px;
}

/* ACESSIBILIDADE */
.skip-link{
    position:absolute;
    left:-9999px;
}

.skip-link:focus{
    left:20px;
    top:20px;
    background:white;
    color:black;
    padding:10px;
    border:3px solid black;
}

button,
a{
    min-height:44px;
}

a:focus,
button:focus{
    outline:4px solid #000;
    outline-offset:4px;
}

header{
    background: linear-gradient(135deg,var(--vermelho-principal),var(--vermelho-secundario));
    color:white;
    text-align:center;
    padding:60px 20px;
}

header h1{
    font-size:clamp(2.5rem,5vw,4rem);
    margin-bottom:20px;
}

header p{
    font-size:1.4rem;
    max-width:900px;
    margin:auto;
}

nav{
    background:#7F0000;
    position:sticky;
    top:0;
    z-index:1000;
}

nav ul{
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    list-style:none;
}

nav a{
    display:block;
    color:white;
    text-decoration:none;
    padding:18px;
    font-weight:bold;
    font-size:1.1rem;
}

nav a:hover{
    background:var(--vermelho-secundario);
}

.container{
    width:min(1200px,95%);
    margin:auto;
}

section{
    padding:70px 20px;
}

h2{
    font-size:2.2rem;
    margin-bottom:25px;
    color:var(--vermelho-principal);
}

.card-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

.card{
    background:white;
    border-left:8px solid var(--vermelho-secundario);
    border-radius:12px;
    padding:25px;
    box-shadow:0 4px 12px rgba(0,0,0,.15);
}

.card h3{
    margin-bottom:15px;
    color:#8B0000;
}

.destaque{
    background:var(--vermelho-principal);
    color:white;
    padding:40px;
    border-radius:15px;
    text-align:center;
}

.dados{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:25px;
    margin-top:30px;
}

.numero{
    background:white;
    color:#8B0000;
    padding:20px;
    min-width:220px;
    border-radius:12px;
    font-weight:bold;
    text-align:center;
}

.numero span{
    display:block;
    font-size:2.2rem;
}

.controles{
    text-align:center;
    margin-top:30px;
}

.btn{
    background:var(--vermelho-principal);
    color:white;
    border:none;
    padding:15px 25px;
    margin:5px;
    border-radius:8px;
    cursor:pointer;
    font-size:1rem;
    font-weight:bold;
}

.btn:hover{
    background:#7F0000;
}

footer{
    background:#4A0000;
    color:white;
    text-align:center;
    padding:30px;
}

/* MODO ALTO CONTRASTE */
.alto-contraste{
    background:black;
    color:white;
}

.alto-contraste section,
.alto-contraste .card{
    background:black;
    color:white;
}

.alto-contraste h2,
.alto-contraste h3{
    color:#FFD54F;
}

.alto-contraste .numero{
    background:#222;
    color:#FFD54F;
}

.alto-contraste nav{
    background:#111;
}

.alto-contraste .btn{
    background:#FFD54F;
    color:black;
}

@media (max-width:768px){
    body{
        font-size:18px;
    }

    h2{
        font-size:1.8rem;
    }
}
</style>
</head>

<body>

<a href="#conteudo" class="skip-link">Pular para o conteúdo principal</a>

<header>
    <h1>🌾 A Importância do Agro</h1>
    <p>
        Olá, eu sou a <strong>Laura</strong>! Este site mostra a importância do agronegócio
        para a alimentação, economia, geração de empregos e sustentabilidade.
    </p>

    <div class="controles">
        <button class="btn" onclick="aumentarFonte()">Aumentar Texto</button>
        <button class="btn" onclick="diminuirFonte()">Diminuir Texto</button>
        <button class="btn" onclick="alternarContraste()">Alto Contraste</button>
    </div>
</header>

<nav aria-label="Menu principal">
    <ul>
        <li><a href="#importancia">Importância</a></li>
        <li><a href="#beneficios">Benefícios</a></li>
        <li><a href="#sustentabilidade">Sustentabilidade</a></li>
    </ul>
</nav>

<main id="conteudo">

<section id="importancia">
<div class="container">
<h2>Por que o Agro é Fundamental?</h2>
<div class="card-grid">
<div class="card">
<h3>🍎 Alimentação</h3>
<p>O agro produz alimentos que chegam às mesas das famílias,
garantindo segurança alimentar e qualidade de vida.</p>
</div>

<div class="card">
<h3>💼 Empregos</h3>
<p>Milhões de pessoas trabalham direta ou indiretamente no setor,
desde a produção até a distribuição dos produtos.</p>
</div>

<div class="card">
<h3>📈 Economia</h3>
<p>O agronegócio contribui significativamente para a economia brasileira,
fortalecendo exportações e gerando renda.</p>
</div>
</div>
</div>
</section>

<section id="beneficios">
<div class="container">
<div class="destaque">
<h2 style="color:white;">O Agro Move o Brasil</h2>
<p>A produção agrícola e pecuária sustenta cidades, abastece mercados
e contribui para o desenvolvimento tecnológico e social do país.</p>

<div class="dados">
<div class="numero"><span>🌽</span>Produção de alimentos</div>
<div class="numero"><span>🚜</span>Inovação no campo</div>
<div class="numero"><span>🌎</span>Exportação mundial</div>
</div>
</div>
</div>
</section>

<section id="sustentabilidade">
<div class="container">
<h2>Agro e Sustentabilidade</h2>
<div class="card-grid">
<div class="card">
<h3>🌱 Preservação Ambiental</h3>
<p>Práticas modernas ajudam a preservar recursos naturais e aumentar
a eficiência da produção agrícola.</p>
</div>

<div class="card">
<h3>💧 Uso Consciente da Água</h3>
<p>Tecnologias de irrigação reduzem desperdícios e melhoram a produtividade.</p>
</div>

<div class="card">
<h3>♻️ Produção Responsável</h3>
<p>O futuro do agro depende do equilíbrio entre produtividade,
preservação ambiental e responsabilidade social.</p>
</div>
</div>
</div>
</section>

</main>

<footer>
    <p>Projeto Educacional • Desenvolvido por <strong>Laura</strong> • Acessível para pessoas com baixa visão • Valorizando a importância do Agro.</p>
</footer>

<script>
let tamanhoAtual = 20;
function aumentarFonte(){
    tamanhoAtual += 2;
    document.body.style.fontSize = tamanhoAtual + "px";
}
function diminuirFonte(){
    if(tamanhoAtual > 14){
        tamanhoAtual -= 2;
        document.body.style.fontSize = tamanhoAtual + "px";
    }
}
function alternarContraste(){
    document.body.classList.toggle("alto-contraste");
}
</script>

</body>
</html>
<section id="sustentabilidade">
<div class="container">

<h2>Agro e Sustentabilidade</h2>

<div class="tabs">
    <button class="tab-btn active" onclick="abrirAba('ambiental')">
        🌱 Preservação Ambiental
    </button>

    <button class="tab-btn" onclick="abrirAba('agua')">
        💧 Uso da Água
    </button>

    <button class="tab-btn" onclick="abrirAba('responsavel')">
        ♻️ Produção Responsável
    </button>
</div>

<!-- ABA: Preservação Ambiental -->
<div id="ambiental" class="tab-content active-tab">
    <h3>🌱 Preservação Ambiental</h3>

    <ul>
        <li><a href="#mata-ciliar">🌳 Matas Ciliares</a></li>
        <li><a href="#recuperacao">🌱 Recuperação de Áreas Degradadas</a></li>
        <li><a href="#biodiversidade">🦜 Preservação da Biodiversidade</a></li>
        <li><a href="#solo">🌾 Conservação do Solo</a></li>
    </ul>

    <!-- MATA CILIAR -->
    <div id="mata-ciliar" class="sub-section">
        <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?w=1000" 
             alt="Mata ciliar preservada com rio">
        <h4>Matas Ciliares</h4>
        <p>
            As matas ciliares são vegetações que cercam rios e córregos, protegendo a água
            contra erosão e poluição. No agro, a preservação dessas áreas evita assoreamento
            e mantém o equilíbrio ecológico.
        </p>
    </div>

    <!-- RECUPERAÇÃO DE ÁREAS DEGRADADAS -->
    <div id="recuperacao" class="sub-section">
        <img src="https://images.unsplash.com/photo-1561867993-6f4db15d2a82?w=1000" 
             alt="Área degradada sendo recuperada com plantio de árvores">
        <h4>Recuperação de Áreas Degradadas</h4>
        <p>
            Áreas degradadas podem ser recuperadas com técnicas como plantio de árvores nativas,
            controle de erosão e adubação orgânica. Isso aumenta a produtividade e protege o ambiente.
        </p>
    </div>

    <!-- PRESERVAÇÃO DA BIODIVERSIDADE -->
    <div id="biodiversidade" class="sub-section">
        <img src="https://images.unsplash.com/photo-1552089123-001a301c35d4?w=1000" 
             alt="Diversidade de espécies vegetais e animais">
        <h4>Preservação da Biodiversidade</h4>
        <p>
            Manter diferentes espécies de plantas e animais no campo garante equilíbrio
            ecológico, controle de pragas naturais e sustentabilidade da produção agrícola.
        </p>
    </div>

    <!-- CONSERVAÇÃO DO SOLO -->
    <div id="solo" class="sub-section">
        <img src="https://images.unsplash.com/photo-1605539432472-1d1f0ed2f9db?w=1000" 
             alt="Solo cultivado com técnicas de conservação">
        <h4>Conservação do Solo</h4>
        <p>
            Técnicas como plantio direto, rotação de culturas e cobertura do solo ajudam
            a evitar erosão, manter a fertilidade e proteger a água subterrânea.
        </p>
    </div>

</div>

<!-- ABA: Uso da Água -->
<div id="agua" class="tab-content">
    <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?w=1000"
         alt="Sistema de irrigação em plantação">

    <h3>💧 Uso Consciente da Água</h3>

    <p>
        Técnicas modernas de irrigação reduzem desperdícios e aumentam a eficiência.
        Sensores de umidade, irrigação localizada e planejamento da água garantem
        sustentabilidade.
    </p>
</div>

<!-- ABA: Produção Responsável -->
<div id="responsavel" class="tab-content">
    <img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?w=1000"
         alt="Produção agrícola sustentável">

    <h3>♻️ Produção Responsável</h3>

    <p>
        Produzir de forma responsável significa equilibrar produtividade, proteção
        ambiental e bem-estar social, garantindo um futuro sustentável.
    </p>
</div>

</div>
</section>
/* Abas */
.tabs{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
    margin-bottom:20px;
}

.tab-btn{
    background:#B71C1C;
    color:white;
    border:none;
    padding:15px 20px;
    cursor:pointer;
    border-radius:8px;
    font-weight:bold;
}

.tab-btn:hover{
    background:#8B0000;
}

.tab-content{
    display:none;
    background:white;
    padding:25px;
    border-radius:12px;
    box-shadow:0 4px 12px rgba(0,0,0,.15);
}

.active-tab{
    display:block;
}

.tab-content img{
    width:100%;
    max-height:400px;
    object-fit:cover;
    border-radius:12px;
    margin-bottom:15px;
}

/* Sub-seções da Preservação Ambiental */
.sub-section{
    margin-top:25px;
}

.sub-section h4{
    color:#D32F2F;
    margin-bottom:10px;
}

.sub-section p{
    font-size:1rem;
}
<script>
function abrirAba(id){
    const abas = document.querySelectorAll('.tab-content');
    abas.forEach(aba => aba.classList.remove('active-tab'));
    document.getElementById(id).classList.add('active-tab');

    const botoes = document.querySelectorAll('.tab-btn');
    botoes.forEach(btn => btn.classList.remove('active'));
    event.target.classList.add('active');
}
</script>
