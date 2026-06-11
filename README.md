<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Agro & Sustentabilidade - Laura Cristina</title>
  <style>
    :root {
      --rosa: #e75480;
      --vinho: #7a1030;
      --bg: #fff5f8;
    }
    * { box-sizing: border-box; font-family: Arial, sans-serif; }
    body { margin: 0; background: var(--bg); color: #333; transition: .3s; }
    header { background: linear-gradient(135deg, var(--vinho), var(--rosa)); color: #fff; padding: 60px 20px; text-align: center; }
    nav { background: var(--vinho); padding: 12px; text-align: center; position: sticky; top: 0; }
    nav a { color: #fff; text-decoration: none; margin: 0 10px; }
    section { max-width: 1100px; margin: 20px auto; background: #fff; padding: 25px; border-radius: 15px; box-shadow: 0 2px 8px rgba(0,0,0,.15); }
    .btn { background: var(--rosa); color: #fff; border: none; padding: 12px 18px; border-radius: 25px; cursor: pointer; margin: 4px; }
    .gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 12px; }
    .gallery img, .hero { width: 100%; border-radius: 12px; }
    iframe { width: 100%; height: 420px; border: 0; border-radius: 12px; }
    .alto-contraste { background: #000; color: #fff; }
    .alto-contraste section { background: #111; color: #fff; }
    .modal { display: none; position: fixed; inset: 0; background: rgba(0,0,0,.8); overflow: auto; }
    .modal-content { background: #fff; max-width: 900px; margin: 30px auto; padding: 25px; border-radius: 15px; }
    .close { float: right; font-size: 30px; cursor: pointer; }
    footer { background: var(--vinho); color: #fff; text-align: center; padding: 20px; }
  </style>
</head>
<body>
<header>
  <h1>Agro & Sustentabilidade</h1>
  <h2>Laura Cristina</h2>
  <p>Projeto acadêmico profissional sobre agro, tecnologia e sustentabilidade.</p>
  <button class="btn" onclick="aumentarTexto()">Aumentar Texto</button>
  <button class="btn" onclick="diminuirTexto()">Diminuir Texto</button>
  <button class="btn" onclick="contraste()">Alto Contraste</button>
</header>

<nav>
  <a href="#agro">Agro</a>
  <a href="#sust">Sustentabilidade</a>
  <a href="#tec">Tecnologia</a>
</nav>

<section>
  <img class="hero" src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&w=1200&q=80">
</section>

<section id="agro">
  <h2>O Agronegócio Brasileiro</h2>
  <p>O agronegócio é um dos principais setores da economia brasileira.</p>
  <button class="btn" onclick="abrirModal()">Saiba Mais</button>
</section>

<section id="sust">
  <h2>Sustentabilidade</h2>
  <p>Práticas sustentáveis ajudam a preservar recursos naturais.</p>
</section>

<section id="tec">
  <h2>Tecnologia no Campo</h2>
  <p>Drones, sensores e agricultura de precisão aumentam a produtividade.</p>
</section>

<section>
  <h2>Galeria</h2>
  <div class="gallery">
    <img src="https://images.unsplash.com/photo-1464226184884-fa280b87c399?auto=format&fit=crop&w=800&q=80">
    <img src="https://images.unsplash.com/photo-1500382017468