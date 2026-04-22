<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mobilidade e Acessibilidade</title>

<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #b3e5fc, #81d4fa);
    color: #003049;
    transition: 0.3s;
}

/* MENU */
nav {
    background: rgba(255,255,255,0.6);
    padding: 15px;
    text-align: center;
}

nav a {
    color: #003049;
    margin: 0 10px;
    text-decoration: none;
    font-weight: bold;
}

/* BOTÃO */
#darkBtn {
    margin-left: 15px;
    padding: 8px 15px;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    background: #003049;
    color: white;
    font-weight: bold;
}

/* HEADER */
header {
    text-align: center;
    padding: 50px 20px;
}

header p {
    max-width: 900px;
    margin: auto;
    line-height: 1.6;
}

/* CARDS */
.container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    padding: 40px;
}

.card {
    background: rgba(255,255,255,0.7);
    padding: 20px;
    border-radius: 15px;
    transition: 0.3s;
}

.card:hover {
    transform: scale(1.05);
}

/* SEÇÕES */
.section {
    padding: 40px;
    text-align: center;
}

.section ul {
    list-style: none;
    padding: 0;
}

.section li {
    margin: 10px 0;
}

/* GALERIA */
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 15px;
    padding: 40px;
}

.gallery img {
    width: 100%;
    border-radius: 10px;
}

/* RODAPÉ */
footer {
    text-align: center;
    padding: 20px;
    background: rgba(255,255,255,0.6);
}

/* 🌙 MODO ESCURO */
.dark-mode {
    background: #121212 !important;
    color: #ffffff;
}

.dark-mode nav {
    background: #000;
}

.dark-mode .card {
    background: rgba(255,255,255,0.05);
}

.dark-mode footer {
    background: #000;
}
</style>
</head>

<body>

<nav>
    <a href="#inicio">Início</a>
    <a href="#explicacao">Explicação</a>
    <a href="#problemas">Problemas</a>
    <a href="#solucoes">Soluções</a>
    <a href="#galeria">Galeria</a>

    <button onclick="toggleDark()" id="darkBtn">🌙 Modo Escuro</button>
</nav>

<header id="inicio">
    <h1>Mobilidade e Acessibilidade</h1>
    <p>
        A mobilidade e a acessibilidade são essenciais para garantir que todas as pessoas possam se locomover com segurança e autonomia.
        Uma cidade acessível promove inclusão social e qualidade de vida.
    </p>
</header>

<!-- CARDS -->
<section class="container" id="explicacao">

    <div class="card">
        <h3>🚀 Mobilidade</h3>

        <p>
            A mobilidade urbana deixou de ser apenas a forma como vamos do ponto A ao ponto B.
            Hoje, ela é o coração das cidades inteligentes e influencia a qualidade de vida.
        </p>

        <p>
            Com o crescimento das cidades, novas soluções estão surgindo para tornar o transporte mais eficiente.
        </p>

        <ul>
            <li>⚡ Veículos elétricos</li>
            <li>🚲 Micromobilidade</li>
            <li>📱 Mobilidade por aplicativos</li>
            <li>🤖 Veículos autônomos</li>
        </ul>

        <p><i>"Planejar a mobilidade é planejar cidades para pessoas."</i></p>
    </div>

    <div class="card">
        <h3>♿ Acessibilidade</h3>
        <p>
            A acessibilidade garante que todas as pessoas possam utilizar espaços com segurança e autonomia.
        </p>

        <p>
            Inclui rampas, transporte adaptado e sinalização adequada, promovendo inclusão social.
        </p>
    </div>

    <div class="card">
        <h3>🌍 Importância</h3>
        <p>
            A mobilidade e a acessibilidade são essenciais para a qualidade de vida nas cidades.
        </p>

        <p>
            Elas permitem acesso ao trabalho, estudo e serviços, reduzindo desigualdades.
        </p>
    </div>

</section>

<!-- PROBLEMAS -->
<section class="section" id="problemas">
    <h2>Problemas</h2>
    <ul>
        <li>Falta de rampas</li>
        <li>Calçadas ruins</li>
        <li>Transporte inadequado</li>
    </ul>
</section>

<!-- SOLUÇÕES -->
<section class="section" id="solucoes">
    <h2>Soluções</h2>
    <ul>
        <li>Infraestrutura acessível</li>
        <li>Melhor transporte</li>
        <li>Tecnologia assistiva</li>
    </ul>
</section>

<!-- GALERIA -->
<section class="section" id="galeria">
    <h2>Galeria</h2>
</section>

<div class="gallery">
    <img src="https://images.unsplash.com/photo-1570129477492-45c003edd2be">
    <img src="https://images.unsplash.com/photo-1502920917128-1aa500764cbd">
    <img src="https://images.unsplash.com/photo-1487958449943-2429e8be8625">
</div>

<footer>
    <p>Projeto Mobilidade e Acessibilidade © 2026</p>
</footer>

<script>
function toggleDark() {
    document.body.classList.toggle("dark-mode");

    let btn = document.getElementById("darkBtn");

    if(document.body.classList.contains("dark-mode")){
        btn.innerHTML = "☀️ Modo Claro";
    } else {
        btn.innerHTML = "🌙 Modo Escuro";
    }
}
</script>

</body>
</html>
