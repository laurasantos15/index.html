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
    <h1> A Importância do Agro</h1>
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
<h3> Alimentação</h3>
<p>O agro produz alimentos que chegam às mesas das famílias,
garantindo segurança alimentar e qualidade de vida.</p>
</div>

<div class="card">
<h3> Empregos</h3>
<p>Milhões de pessoas trabalham direta ou indiretamente no setor,
desde a produção até a distribuição dos produtos.</p>
</div>

<div class="card">
<h3> Economia</h3>
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
<div class="numero"><span> </span>Produção de alimentos</div>
<div class="numero"><span> </span>Inovação no campo</div>
<div class="numero"><span> </span>Exportação mundial</div>
</div>
</div>
</div>
</section>

<section id="sustentabilidade">
<div class="container">
<h2>Agro e Sustentabilidade</h2>
<div class="card-grid">
<div class="card">
<h3> Preservação Ambiental</h3>
<p>Práticas modernas ajudam a preservar recursos naturais e aumentar
a eficiência da produção agrícola.</p>
</div>

<div class="card">
<h3> Uso Consciente da Água</h3>
<p>Tecnologias de irrigação reduzem desperdícios e melhoram a produtividade.</p>
</div>

<div class="card">
<h3> Produção Responsável</h3>
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
