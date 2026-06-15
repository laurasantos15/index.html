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


https://laurasantos15.github.io/index.html/#o-agro-move-o-brasil



<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Agro Brasil - Sustentabilidade e Tecnologia</title>

<style>
:root{
    --vermelho1:#B71C1C;
    --vermelho2:#D32F2F;
    --vermelho3:#7F0000;
    --fundo:#fff6f6;
}

/* BASE */
*{margin:0;padding:0;box-sizing:border-box;}

body{
    font-family:Arial;
    background:var(--fundo);
    color:#111;
    font-size:20px;
    transition:0.3s;
}

/* HEADER COM VÍDEO */
header{
    position:relative;
    height:70vh;
    overflow:hidden;
    color:white;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
}

video{
    position:absolute;
    width:100%;
    height:100%;
    object-fit:cover;
    z-index:-1;
    filter:brightness(40%);
}

header h1{
    font-size:3rem;
}

header p{
    max-width:700px;
    margin:auto;
}

.btn{
    background:var(--vermelho1);
    color:white;
    border:none;
    padding:10px 15px;
    margin:5px;
    border-radius:8px;
    cursor:pointer;
}

/* NAV */
nav{
    background:var(--vermelho3);
    text-align:center;
    padding:10px;
    position:sticky;
    top:0;
}

nav a{
    color:white;
    text-decoration:none;
    margin:10px;
    font-weight:bold;
}

/* CONTAINER */
.container{
    width:90%;
    max-width:1100px;
    margin:auto;
    padding:40px 0;
}

/* CARDS */
.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:20px;
}

.card{
    background:white;
    padding:20px;
    border-left:6px solid var(--vermelho2);
    border-radius:10px;
    box-shadow:0 3px 10px rgba(0,0,0,0.1);
}

/* MAPA SIMBÓLICO */
.mapa{
    background:linear-gradient(135deg,#ffdddd,#fff);
    padding:20px;
    border-radius:10px;
    text-align:center;
}

/* BARRA SIMPLES (GRÁFICO) */
.bar{
    background:#ddd;
    border-radius:20px;
    overflow:hidden;
    margin:8px 0;
}

.bar span{
    display:block;
    background:var(--vermelho2);
    color:white;
    padding:5px;
}

/* EXTRA */
.extra{display:none;margin-top:10px;}

/* CONTRASTE */
.alto-contraste{
    background:black !important;
    color:white !important;
}

.alto-contraste .card{
    background:black !important;
    border:1px solid yellow;
}

.alto-contraste h1,
.alto-contraste h2{
    color:yellow !important;
}

.alto-contraste .btn{
    background:yellow !important;
    color:black !important;
}
</style>
</head>

<body>

<header>
    <!-- VÍDEO (substitua por arquivo local se quiser) -->
    <video autoplay muted loop>
        <source src="https://cdn.pixabay.com/video/2023/03/10/154393-817302878_large.mp4" type="video/mp4">
    </video>

    <div>
        <h1>Agro Brasil</h1>
        <p>Sustentabilidade, tecnologia e produção que alimenta o mundo</p>

        <button class="btn" onclick="aumentar()">Aumentar</button>
        <button class="btn" onclick="diminuir()">Diminuir</button>
        <button class="btn" onclick="contraste()">Contraste</button>
    </div>
</header>

<nav>
    <a href="#importancia">Importância</a>
    <a href="#sustentabilidade">Sustentabilidade</a>
    <a href="#tecnologia">Tecnologia</a>
    <a href="#dados">Dados</a>
</nav>

<div class="container">

<!-- IMPORTANCIA -->
<section id="importancia">
<h2>Importância do Agro</h2>

<div class="grid">

<div class="card">
<h3>Alimentação</h3>
<p>O agro alimenta o mundo inteiro.</p>
<button class="btn" onclick="toggle('a')">Saiba mais</button>
<div id="a" class="extra">
<p>Produz arroz, soja, carne, frutas e garante segurança alimentar global.</p>
</div>
</div>

<div class="card">
<h3>Economia</h3>
<p>Fortalece o Brasil.</p>
<button class="btn" onclick="toggle('b')">Saiba mais</button>
<div id="b" class="extra">
<p>Representa grande parte do PIB e exportações brasileiras.</p>
</div>
</div>

</div>
</section>

<!-- SUSTENTABILIDADE -->
<section id="sustentabilidade">
<h2>Sustentabilidade</h2>

<div class="grid">
<div class="card">Preservação do solo e natureza</div>
<div class="card">Uso consciente da água</div>
<div class="card">Produção responsável</div>
</div>
</section>

<!-- TECNOLOGIA -->
<section id="tecnologia">
<h2>Tecnologia no Campo</h2>

<div class="grid">

<div class="card">
<h3>Drones</h3>
<p>Monitoramento aéreo das plantações</p>
</div>

<div class="card">
<h3>IA</h3>
<p>Previsão de clima e produtividade</p>
</div>

<div class="card">
<h3>Energia Solar</h3>
<p>Energia limpa nas fazendas</p>
</div>

</div>
</section>

<!-- MAPA -->
<section class="mapa">
<h2>Exportação Brasileira</h2>
<p>Brasil exporta alimentos para mais de 150 países</p>
<p>🌎 América, Europa, Ásia e África</p>
</section>

<!-- GRÁFICOS -->
<section id="dados">
<h2>Dados do Agro</h2>

<p>Exportação</p>
<div class="bar"><span style="width:90%">90%</span></div>

<p>Empregos</p>
<div class="bar"><span style="width:70%">70%</span></div>

<p>Sustentabilidade</p>
<div class="bar"><span style="width:80%">80%</span></div>

</section>

</div>

<script>

let size = 20;

function aumentar(){ size+=2; document.body.style.fontSize=size+"px"; }
function diminuir(){ if(size>14){ size-=2; document.body.style.fontSize=size+"px"; } }

function contraste(){
    document.body.classList.toggle("alto-contraste");
}

function toggle(id){
    const el=document.getElementById(id);
    el.style.display = el.style.display==="block"?"none":"block";
}

</script>

</body>
</html>
     









