
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Agro e Sustentabilidade</title>

<style>
:root{
    --vermelho-principal:#B71C1C;
    --vermelho-secundario:#D32F2F;
    --fundo:#FFF8F8;
    --texto:#111;
}

/* BASE */
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family: Arial, Helvetica, sans-serif;
    background:var(--fundo);
    color:var(--texto);
    font-size:20px;
    line-height:1.8;
}

/* HEADER */
header{
    background:linear-gradient(135deg,var(--vermelho-principal),var(--vermelho-secundario));
    color:white;
    text-align:center;
    padding:50px 20px;
}

h1{
    font-size:2.5rem;
}

.controles{
    margin-top:20px;
}

.btn{
    background:#B71C1C;
    color:white;
    border:none;
    padding:10px 15px;
    margin:5px;
    border-radius:8px;
    cursor:pointer;
}

/* NAV */
nav{
    background:#7F0000;
    text-align:center;
    padding:10px;
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
.card-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:20px;
}

.card{
    background:white;
    padding:20px;
    border-left:6px solid var(--vermelho-secundario);
    border-radius:10px;
    box-shadow:0 3px 10px rgba(0,0,0,0.1);
}

.card h3{
    color:#8B0000;
}

/* BOTÃO SAIBA MAIS */
.card button{
    margin-top:10px;
}

/* ALTO CONTRASTE */
.alto-contraste{
    background:black !important;
    color:white !important;
}

.alto-contraste header,
.alto-contraste .card,
.alto-contraste nav{
    background:black !important;
    color:white !important;
    border:1px solid #FFD700;
}

.alto-contraste h1,
.alto-contraste h2,
.alto-contraste h3{
    color:#FFD700 !important;
}

.alto-contraste .btn{
    background:#FFD700 !important;
    color:black !important;
}
</style>
</head>

<body>

<header>
    <h1>Agro e Sustentabilidade</h1>

    <div class="controles">
        <button class="btn" onclick="aumentarFonte()">Aumentar Texto</button>
        <button class="btn" onclick="diminuirFonte()">Diminuir Texto</button>
        <button class="btn" onclick="alternarContraste()">Alto Contraste</button>
    </div>
</header>

<nav>
    <a href="#importancia">Importância</a>
    <a href="#sustentabilidade">Sustentabilidade</a>
    <a href="#tecnologia">Tecnologia</a>
</nav>

<div class="container">

<!-- IMPORTÂNCIA -->
<section id="importancia">
<h2>Importância do Agro</h2>

<div class="card-grid">

<div class="card">
<h3>Alimentação</h3>
<p>O agro produz alimentos para todo o mundo.</p>

<button class="btn" onclick="toggleAlimentacao()">Saiba mais</button>
<div id="maisAlimentacao" style="display:none;">
<p>O agro garante segurança alimentar, diversidade de produtos e abastecimento constante das cidades.</p>
</div>
</div>

<div class="card">
<h3>Economia</h3>
<p>Movimenta a economia brasileira.</p>

<button class="btn" onclick="toggleEconomia()">Saiba mais</button>
<div id="maisEconomia" style="display:none;">
<p>O agronegócio representa grande parte do PIB e das exportações do Brasil, gerando empregos e renda.</p>
</div>
</div>

</div>
</section>

<!-- SUSTENTABILIDADE -->
<section id="sustentabilidade">
<h2>Sustentabilidade no Agro</h2>

<div class="card-grid">

<div class="card">
<h3>Preservação Ambiental</h3>
<p>Proteção da natureza e do solo.</p>
</div>

<div class="card">
<h3>Uso da Água</h3>
<p>Uso consciente e eficiente da água.</p>
</div>

<div class="card">
<h3>Produção Responsável</h3>
<p>Produção equilibrada e sustentável.</p>
</div>

</div>
</section>

<!-- TECNOLOGIA -->
<section id="tecnologia">
<h2>Tecnologia Verde</h2>

<div class="card-grid">

<div class="card">
<h3>Drones e Sensores</h3>
<p>Monitoramento das plantações.</p>

<button class="btn" onclick="toggleDrones()">Saiba mais</button>
<div id="maisDrones" style="display:none;">
<p>Drones ajudam a identificar pragas e melhorar a produtividade da lavoura.</p>
</div>
</div>

<div class="card">
<h3>IA e Agricultura de Precisão</h3>
<p>Uso de inteligência artificial no campo.</p>

<button class="btn" onclick="toggleIA()">Saiba mais</button>
<div id="maisIA" style="display:none;">
<p>A IA analisa clima e solo para melhorar a produção e reduzir desperdícios.</p>
</div>
</div>

<div class="card">
<h3>Energia Renovável</h3>
<p>Energia limpa no campo.</p>

<button class="btn" onclick="toggleEnergia()">Saiba mais</button>
<div id="maisEnergia" style="display:none;">
<p>Energia solar e biomassa reduzem impactos ambientais nas fazendas.</p>
</div>
</div>

</div>
</section>

</div>

<script>
let tamanho = 20;

function aumentarFonte(){
    tamanho += 2;
    document.body.style.fontSize = tamanho + "px";
}

function diminuirFonte(){
    if(tamanho > 14){
        tamanho -= 2;
        document.body.style.fontSize = tamanho + "px";
    }
}

function alternarContraste(){
    document.body.classList.toggle("alto-contraste");
}

/* TOGGLES */
function toggleAlimentacao(){
    const el = document.getElementById("maisAlimentacao");
    el.style.display = el.style.display === "none" ? "block" : "none";
}

function toggleEconomia(){
    const el = document.getElementById("maisEconomia");
    el.style.display = el.style.display === "none" ? "block" : "none";
}

function toggleDrones(){
    const el = document.getElementById("maisDrones");
    el.style.display = el.style.display === "none" ? "block" : "none";
}

function toggleIA(){
    const el = document.getElementById("maisIA");
    el.style.display = el.style.display === "none" ? "block" : "none";
}

function toggleEnergia(){
    const el = document.getElementById("maisEnergia");
    el.style.display = el.style.display === "none" ? "block" : "none";
}
</script>

</body>
</html>
