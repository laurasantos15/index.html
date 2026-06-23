<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vidraçaria Vilas Boas</title>

<link rel="stylesheet" href="style.css">

</head>
<body>

<div class="sidebar">

    <h2>Vidraçaria Vilas Boas</h2>

    <ul>
        <li><a href="#">Dashboard</a></li>
        <li><a href="#">Clientes</a></li>
        <li><a href="#">Orçamentos</a></li>
        <li><a href="#">Projetos 3D</a></li>
        <li><a href="#">Agenda</a></li>
        <li><a href="#">Relatórios</a></li>
    </ul>

</div>

<div class="main">

    <header>
        <h1>Painel Administrativo</h1>

        <button onclick="window.print()">
            🖨️ Imprimir
        </button>
    </header>

    <section class="cards">

        <div class="card">
            <h3>Clientes</h3>
            <p id="totalClientes">0</p>
        </div>

        <div class="card">
            <h3>Orçamentos</h3>
            <p id="totalOrcamentos">0</p>
        </div>

        <div class="card">
            <h3>Projetos</h3>
            <p id="totalProjetos">0</p>
        </div>

    </section>

    <section class="formulario">

        <h2>Novo Orçamento</h2>

        <input
            type="text"
            id="cliente"
            placeholder="Nome do Cliente"
        >

        <input
            type="text"
            id="telefone"
            placeholder="Telefone"
        >

        <select id="produto">
            <option>Janela</option>
            <option>Porta</option>
            <option>Box</option>
            <option>Guarda-Corpo</option>
            <option>Fechamento de Sacada</option>
            <option>Espelho</option>
        </select>

        <input
            type="number"
            id="largura"
            placeholder="Largura (cm)"
        >

        <input
            type="number"
            id="altura"
            placeholder="Altura (cm)"
        >

        <textarea
            id="obs"
            placeholder="Observações"
        ></textarea>

        <button onclick="salvarOrcamento()">
            Salvar Orçamento
        </button>

    </section>

    <section class="preview3d">

        <h2>Projeto 3D</h2>

        <div id="area3d">
            <p>
                Preencha as medidas para gerar o projeto 3D.
<section class="lista-orcamentos">

    <h2>Orçamentos Salvos</h2>

    <div id="listaOrcamentos"></div>

</section>
            </p>
        </div>

    </section>

</div>

<script src="script.js"></script>

</body>
</html>
/* =========================
   VIDRAÇARIA VILAS BOAS
   Tema Vinho Profissional
========================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    display:flex;
    background:#f5f5f5;
}

/* MENU LATERAL */

.sidebar{
    width:250px;
    min-height:100vh;
    background:#6D0F1B;
    color:white;
    padding:20px;
}

.sidebar h2{
    text-align:center;
    margin-bottom:30px;
    border-bottom:1px solid rgba(255,255,255,0.2);
    padding-bottom:15px;
}

.sidebar ul{
    list-style:none;
}

.sidebar ul li{
    margin:15px 0;
}

.sidebar ul li a{
    color:white;
    text-decoration:none;
    display:block;
    padding:12px;
    border-radius:8px;
    transition:0.3s;
}

.sidebar ul li a:hover{
    background:#8B1E2D;
}

/* CONTEÚDO */

.main{
    flex:1;
    padding:25px;
}

/* TOPO */

header{
    display:flex;
    justify-content:space-between;
    align-items:center;
    margin-bottom:25px;
}

header h1{
    color:#6D0F1B;
}

header button{
    background:#8B1E2D;
    color:white;
    border:none;
    padding:10px 18px;
    border-radius:8px;
    cursor:pointer;
}

header button:hover{
    background:#A83246;
}

/* CARDS */

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
    margin-bottom:30px;
}

.card{
    background:white;
    padding:20px;
    border-radius:12px;
    box-shadow:0 2px 10px rgba(0,0,0,0.08);
    text-align:center;
}

.card h3{
    color:#6D0F1B;
    margin-bottom:10px;
}

.card p{
    font-size:28px;
    font-weight:bold;
}

/* FORMULÁRIO */

.formulario{
    background:white;
    padding:25px;
    border-radius:12px;
    margin-bottom:25px;
    box-shadow:0 2px 10px rgba(0,0,0,0.08);
}

.formulario h2{
    color:#6D0F1B;
    margin-bottom:20px;
}

.formulario input,
.formulario select,
.formulario textarea{
    width:100%;
    margin-bottom:15px;
    padding:12px;
    border:1px solid #ccc;
    border-radius:8px;
}

.formulario textarea{
    height:100px;
    resize:none;
}

.formulario button{
    background:#8B1E2D;
    color:white;
    border:none;
    padding:12px 20px;
    border-radius:8px;
    cursor:pointer;
}

.formulario button:hover{
    background:#A83246;
}

/* ÁREA 3D */

.preview3d{
    background:white;
    padding:25px;
    border-radius:12px;
    box-shadow:0 2px 10px rgba(0,0,0,0.08);
}

.preview3d h2{
    color:#6D0F1B;
    margin-bottom:15px;
}

#area3d{
    height:350px;
    border:2px dashed #8B1E2D;
    border-radius:10px;
    display:flex;
    justify-content:center;
    align-items:center;
    color:#777;
}

/* RESPONSIVO */

@media(max-width:768px){

    body{
        flex-direction:column;
    }

    .sidebar{
        width:100%;
        min-height:auto;
    }

    header{
        flex-direction:column;
        gap:10px;
    }
}
function salvarOrcamento() {

    const cliente =
        document.getElementById("cliente").value;

    const telefone =
        document.getElementById("telefone").value;

    const produto =
        document.getElementById("produto").value;

    const largura =
        document.getElementById("largura").value;

    const altura =
        document.getElementById("altura").value;

    const obs =
        document.getElementById("obs").value;

    if (
        cliente === "" ||
        largura === "" ||
        altura === ""
    ) {
        alert(
            "Preencha Cliente, Largura e Altura."
        );
        return;
    }

    const orcamento = {
        cliente,
        telefone,
        produto,
        largura,
        altura,
        obs,
        data: new Date().toLocaleDateString()
    };

    let lista =
        JSON.parse(
            localStorage.getItem("orcamentos")
        ) || [];

    lista.push(orcamento);

    localStorage.setItem(
        "orcamentos",
        JSON.stringify(lista)
    );

    atualizarContadores();

    alert(
        "Orçamento salvo com sucesso!"
    );

    document.getElementById("cliente").value = "";
    document.getElementById("telefone").value = "";
    document.getElementById("largura").value = "";
    document.getElementById("altura").value = "";
    document.getElementById("obs").value = "";
}

function atualizarContadores() {

    let lista =
        JSON.parse(
            localStorage.getItem("orcamentos")
        ) || [];

    document.getElementById(
        "totalOrcamentos"
    ).innerText = lista.length;
}

window.onload = function () {

    atualizarContadores();


};
function carregarOrcamentos() {

    let lista =
        JSON.parse(
            localStorage.getItem("orcamentos")
        ) || [];

    let html = "";

    lista.forEach((orcamento, index) => {

        html += `
        <div class="card">
            <h3>${orcamento.cliente}</h3>

            <p>
                Produto: ${orcamento.produto}
            </p>

            <p>
                Medidas:
                ${orcamento.largura} x
                ${orcamento.altura}
            </p>

            <button onclick="excluirOrcamento(${index})">
                Excluir
            </button>
        </div>
        `;
    });

    document.getElementById(
        "listaOrcamentos"
    ).innerHTML = html;
}

function excluirOrcamento(index){

    let lista =
        JSON.parse(
            localStorage.getItem("orcamentos")
        ) || [];

    lista.splice(index,1);

    localStorage.setItem(
        "orcamentos",
        JSON.stringify(lista)
    );

    atualizarContadores();
    carregarOrcamentos();
}

window.onload = function(){

    atualizarContadores();
    carregarOrcamentos();

carregarOrcamentos();
}
