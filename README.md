<!DOCTYPE html>
<html lang="pt-BR">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Agro e Sustentabilidade - Laura Cristina</title>

<style>

*{
box-sizing:border-box;
}

body{
margin:0;
font-family:Arial;
background:#f8eeee;
color:#3b1018;
font-size:18px;
transition:.3s;
}


header{
background:linear-gradient(135deg,#420814,#9b3b55);
color:white;
padding:45px;
text-align:center;
}


h1{
font-size:45px;
}


button,.saiba{
background:#c56b80;
color:white;
padding:12px 22px;
border:none;
border-radius:25px;
cursor:pointer;
margin:5px;
text-decoration:none;
}


nav{
background:#30050d;
padding:18px;
text-align:center;
}


nav a{
color:white;
margin:15px;
text-decoration:none;
}


section{

width:90%;
max-width:1100px;
margin:30px auto;
background:white;
padding:30px;
border-radius:20px;
box-shadow:0 5px 20px #aaa;

}


img{

width:100%;
height:350px;
object-fit:cover;
border-radius:20px;

}


h2{

color:#8b2942;

}



#mapa{

height:400px;

}



.contraste{

background:#000;
color:white;

}


.contraste section{

background:#111;

}


.contraste h2{

color:#ffb0c0;

}



footer{

background:#420814;
color:white;
padding:25px;
text-align:center;

}


</style>


</head>


<body>


<header>


<h1>Agro & Sustentabilidade</h1>


<h2>Projeto desenvolvido por Laura Cristina</h2>


<p>
Tecnologia, produção agrícola e preservação ambiental.
</p>


<button onclick="aumentar()">Aumentar texto</button>

<button onclick="diminuir()">Diminuir texto</button>

<button onclick="contraste()">Contraste</button>


</header>



<nav>

<a href="#producao">Produção</a>

<a href="#tecnologia">Tecnologia</a>

<a href="#social">Impacto Social</a>

<a href="#dados">Gráficos</a>

<a href="#mapa">Mapa</a>


</nav>




<section>


<img src="img/capa.jpg">


<h2>Agro sustentável</h2>

<p>
O agro sustentável une produção de alimentos, inovação,
economia e preservação da natureza.
</p>


</section>





<section id="producao">


<h2>Produção Sustentável</h2>


<img src="img/producao.jpg">


<p>
A agricultura sustentável protege o solo, reduz desperdícios,
economiza água e busca equilíbrio ambiental.
</p>


<a class="saiba" href="https://pt.wikipedia.org/wiki/Agricultura_sustent%C3%A1vel" target="_blank">
Saiba Mais
</a>


</section>





<section id="tecnologia">


<h2>Tecnologia no Campo</h2>


<img src="img/tecnologia.jpg">


<p>
Máquinas inteligentes, sensores, drones e dados ajudam
na produção agrícola moderna.
</p>


<a class="saiba" href="https://pt.wikipedia.org/wiki/Agricultura_de_precis%C3%A3o" target="_blank">
Saiba Mais
</a>


</section>





<section id="social">


<h2>Impacto Social</h2>


<img src="img/social.jpg">


<p>
O agronegócio gera empregos, fortalece comunidades
e contribui para a segurança alimentar.
</p>


<a class="saiba" href="https://pt.wikipedia.org/wiki/Seguran%C3%A7a_alimentar" target="_blank">
Saiba Mais
</a>


</section>






<section id="dados">


<h2>Indicadores de Sustentabilidade</h2>


<canvas id="grafico"></canvas>


</section>





<section>


<h2>Vídeo educativo</h2>


<iframe width="100%" height="315"
src="https://www.youtube.com/embed"
allowfullscreen>
</iframe>


</section>





<section>


<h2>Mapa agrícola</h2>


<div id="mapa"></div>


</section>






<footer>

Laura Cristina - Agro & Sustentabilidade

</footer>




<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>


<link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css"/>




<script>


let tamanho=18;


function aumentar(){

tamanho+=2;

document.body.style.fontSize=tamanho+"px";

}


function diminuir(){

if(tamanho>12){

tamanho-=2;

document.body.style.fontSize=tamanho+"px";

}

}



function contraste(){

document.body.classList.toggle("contraste");

}




new Chart(document.getElementById("grafico"),{

type:"bar",

data:{

labels:["Água","Solo","Energia","Tecnologia"],

datasets:[{

label:"Sustentabilidade",

data:[90,85,75,95]

}]

}

});





let mapa=L.map("mapa").setView([-15,-47],4);


L.tileLayer(
"https://tile.openstreetmap.org/{z}/{x}/{y}.png"
).addTo(mapa);


L.marker([-15,-47])
.addTo(mapa)
.bindPopup("Área agrícola brasileira");



</script>



</body>

</html>
