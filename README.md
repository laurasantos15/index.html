<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Agro Brasil - Educação e Sustentabilidade</title>
<style>
:root{
  --vermelho1:#B71C1C;
  --vermelho2:#D32F2F;
  --vermelho3:#7F0000;
  --fundo:#fff6f6;
}
*{margin:0;padding:0;box-sizing:border-box;}
body{font-family:Arial; background:var(--fundo); color:#111; font-size:20px; line-height:1.7; transition:0.3s;}
a{text-decoration:none; color:white; font-weight:bold;}
.container{width:90%; max-width:1200px; margin:auto; padding:40px 0;}
.grid{display:grid; grid-template-columns:repeat(auto-fit,minmax(280px,1fr)); gap:20px;}
.card{background:white; padding:20px; border-left:6px solid var(--vermelho2); border-radius:10px; box-shadow:0 3px 10px rgba(0,0,0,0.1); transition:0.3s;}
.card:hover{transform:translateY(-5px);}
.extra{display:none; margin-top:10px;}
h1,h2,h3{transition:0.3s;}
h2{color:var(--vermelho1); margin-bottom:20px;}
header{text-align:center; position:relative; height:70vh; overflow:hidden; display:flex; flex-direction:column; align-items:center; justify-content:center; color:white;}
header video{position:absolute; width:100%; height:100%; object-fit:cover; z-index:-1; filter:brightness(40%);}
header .btn{background:var(--vermelho1); color:white; border:none; padding:10px 15px; margin:5px; border-radius:8px; cursor:pointer; transition:0.3s;}
header .btn:hover{background:var(--vermelho3); transform:scale(1.05);}
nav{background:var(--vermelho3); text-align:center; padding:12px; position:sticky; top:0; z-index:1000;}
nav a{margin:10px;}
footer{background:var(--vermelho3); color:white; text-align:center; padding:20px; margin-top:50px;}
.bar{background:#ddd; border-radius:20px; overflow:hidden; margin:8px 0;}
.bar span{display:block; background:var(--vermelho2); color:white; padding:5px; transition:0.5s;}
.mapa{background:linear-gradient(135deg,#ffdddd,#fff); padding:20px; border-radius:10px; text-align:center; margin-top:20px;}
.alto-contraste{background:black !important; color:white !important;}
.alto-contraste .card{background:black !important; border:1px solid yellow;}
.alto-contraste h1,h2,h3{color:yellow !important;}
.alto-contraste .btn{background:yellow !important; color:black !important;}
/* CARROSSEL */
.carousel{position:relative; overflow:hidden; border-radius:10px; margin:20px 0;}
.carousel img{width:100%; display:none; border-radius:10px;}
.carousel img.active{display:block; animation:fade 1s;}
@keyframes fade{from{opacity:0;} to{opacity:1;}}
@media (max-width:768px){body{font-size:18px;}}
</style>
</head>
<body>

<header>
<video autoplay muted loop>
<source src="https://cdn.pixabay.com/video/2023/03/10/154393-817302878_large.mp4" type="video/mp4">
</video>
<h1>Agro Brasil - Educação e Sustentabilidade</h1>
<p>Explore tecnologia, inovação e cuidado ambiental no agronegócio brasileiro</p>
<div>
<button class="btn" onclick="aumentar()">Aumentar</button>
<button class="btn" onclick="diminuir()">Diminuir</button>
<button class="btn" onclick="contraste()">Contraste</button>
</div>
</header>

<nav>
<a href="#home">Home</a>
<a href="#importancia">Sobre o Agro</a>
<a href="#sustentabilidade">Sustentabilidade</a>
<a href="#tecnologia">Tecnologia</a>
<a href="#dados">Dados</a>
</nav>

<div class="container" id="home">

<!-- CARROSSEL -->
<div class="carousel">
<img src="https://cdn.pixabay.com/photo/2016/09/18/19/51/soy-1675532_1280.jpg" class="active">
<img src="https://cdn.pixabay.com/photo/2017/07/31/11/21/cornfield-2559494_1280.jpg">
<img src="https://cdn.pixabay.com/photo/2016/11/29/10/07/cattle-1867178_1280.jpg">
</div>

</div>

<div class="container">

<!-- IMPORTANCIA -->
<section id="importancia">
<h2>Importância do Agro</h2>
<div class="grid">
<div class="card">
<h3>Alimentação</h3>
<p>Produz alimentos para bilhões de pessoas.</p>
<button class="btn" onclick="toggle('a')">Saiba mais</button>
<div id="a" class="extra">
<p>Garante variedade de produtos, segurança alimentar e acesso a alimentos de qualidade.</p>
</div>
</div>

<div class="card">
<h3>Economia</h3>
<p>Fortalece o Brasil</p>
<button class="btn" onclick="toggle('b')">Saiba mais</button>
<div id="b" class="extra">
<p>Representa grande parte do PIB brasileiro, exportações e geração de empregos diretos e indiretos.</p>
</div>
</div>
</div>
</section>

<!-- SUSTENTABILIDADE -->
<section id="sustentabilidade">
<h2>Sustentabilidade</h2>
<div class="grid">
<div class="card"><h3>Preservação do Solo e Natureza</h3><p>Práticas que protegem o solo e o ecossistema.</p></div>
<div class="card"><h3>Uso Consciente da Água</h3><p>Irrigação eficiente e redução de desperdícios.</p></div>
<div class="card"><h3>Produção Responsável</h3><p>Equilíbrio entre produtividade e responsabilidade ambiental e social.</p></div>
</div>
</section>

<!-- TECNOLOGIA -->
<section id="tecnologia">
<h2>Tecnologia no Campo</h2>
<div class="grid">
<div class="card"><h3>Drones e Sensores</h3><p>Monitoramento aéreo das plantações.</p></div>
<div class="card"><h3>IA e Agricultura de Precisão</h3><p>Melhora produtividade e prevê condições climáticas.</p></div>
<div class="card"><h3>Energia Renovável</h3><p>Uso de energia solar e biomassa nas fazendas.</p></div>
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
<p>Exportações</p>
<div class="bar"><span style="width:90%">90%</span></div>
<p>Empregos</p>
<div class="bar"><span style="width:70%">70%</span></div>
<p>Sustentabilidade</p>
<div class="bar"><span style="width:80%">80%</span></div>
</section>

</div>

<footer>
<p>Agro Brasil • Educação e Sustentabilidade • Desenvolvido para estudo e divulgação • ♿ Acessível</p>
</footer>

<script>
let size=20;
function aumentar(){size+=2;document.body.style.fontSize=size+"px";}
function diminuir(){if(size>14){size-=2;document.body.style.fontSize=size+"px";}}
function contraste(){document.body.classList.toggle("alto-contraste");}
function toggle(id){const el=document.getElementById(id);el.style.display=el
