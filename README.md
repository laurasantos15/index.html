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
