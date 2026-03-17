<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Flash Light | Paquetería & Logística</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:'Inter',sans-serif;background:#f4f6fb;color:#1f2937}

header{background:white;border-bottom:1px solid #e5e7eb;position:sticky;top:0;z-index:10}
.container{max-width:1200px;margin:auto;padding:0 20px}

nav{display:flex;justify-content:space-between;align-items:center;padding:18px 0}
.logo{font-size:22px;font-weight:700;color:#1e3a8a}
nav a{margin-left:20px;text-decoration:none;color:#374151;font-weight:500}
nav a:hover{color:#2563eb}

.hero{background:linear-gradient(120deg,#1e3a8a,#2563eb);color:white;padding:110px 20px;text-align:center}
.hero h1{font-size:48px;margin-bottom:15px}
.hero p{font-size:20px;opacity:0.9}
.hero button{margin-top:25px;padding:14px 30px;border:none;border-radius:8px;background:#facc15;font-weight:600;cursor:pointer}

.section{padding:80px 20px}
.section h2{font-size:32px;margin-bottom:25px;color:#1e3a8a}
.section p{line-height:1.7;margin-bottom:18px}

.services{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:25px;margin-top:30px}

.card{background:white;padding:30px;border-radius:12px;box-shadow:0 10px 25px rgba(0,0,0,0.08);transition:0.2s}
.card:hover{transform:translateY(-5px)}
.card h3{margin-bottom:10px;color:#2563eb}

.tracking{background:white;padding:40px;border-radius:12px;box-shadow:0 10px 25px rgba(0,0,0,0.08);max-width:600px;margin:auto;text-align:center}

input{padding:12px;width:65%;border:1px solid #d1d5db;border-radius:6px}
button.search{padding:12px 20px;border:none;background:#2563eb;color:white;border-radius:6px;margin-left:10px;cursor:pointer}

.result{margin-top:25px;padding:15px;border-radius:8px;background:#eef2ff;display:none}

footer{background:#0f172a;color:white;padding:40px 20px;margin-top:80px}
.footer-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:30px}
.footer-grid h4{margin-bottom:10px}
.copyright{text-align:center;margin-top:25px;font-size:14px;opacity:0.7}

.admin{background:white;padding:40px;border-radius:12px;box-shadow:0 10px 25px rgba(0,0,0,0.08);max-width:600px;margin:auto}

</style>
</head>

<body>

<header>
<div class="container">
<nav>
<div class="logo">FLASH LIGHT</div>
<div>
<a href="#mision">Misión</a>
<a href="#vision">Visión</a>
<a href="#politica">Política</a>
<a href="#servicios">Servicios</a>
<a href="#rastreo">Rastreo</a>
<a href="#contacto">Contacto</a>
</div>
</nav>
</div>
</header>

<section class="hero">
<h1>Flash Light Paquetería & Logística</h1>
<p>Soluciones modernas de envío rápido, seguro y confiable</p>
<button onclick="location.href='#rastreo'">Rastrear envío</button>
</section>

<section class="section container" id="mision">
<h2>Misión</h2>
<p>En Flash Light S.A. de C.V. nuestra misión es brindar servicios de logística y entrega de paquetes con los más altos estándares de calidad, garantizando eficiencia y efectividad en los tiempos de entrega.</p>
<p>Nos comprometemos a satisfacer las necesidades de nuestros clientes mediante un servicio confiable, ágil y seguro, priorizando siempre la atención y la experiencia del cliente.</p>
</section>

<section class="section container" id="vision">
<h2>Visión</h2>
<p>Aspiramos a consolidarnos como una empresa líder en el sector de paquetería y logística, reconocida por la excelencia, rapidez y confiabilidad en cada uno de nuestros servicios.</p>
<p>Buscamos fortalecer continuamente nuestros procesos mediante innovación tecnológica y mejora continua.</p>
</section>

<section class="section container" id="politica">
<h2>Política de Calidad</h2>
<p>En Flash Light S.A de C.V estamos comprometidos con ofrecer soluciones logísticas eficientes, seguras y oportunas que satisfagan las necesidades y expectativas de nuestros clientes.</p>
<p>Promovemos una cultura organizacional basada en la mejora continua y el cumplimiento de los lineamientos del Sistema de Gestión de Calidad ISO 9001.</p>
</section>

<section class="section container" id="servicios">
<h2>Servicios</h2>
<div class="services">

<div class="card">
<h3>Envíos Nacionales</h3>
<p>Distribución rápida en todo el país.</p>
</div>

<div class="card">
<h3>Envíos Express</h3>
<p>Servicio prioritario para entregas urgentes.</p>
</div>

<div class="card">
<h3>Logística Empresarial</h3>
<p>Soluciones de logística para empresas.</p>
</div>

<div class="card">
<h3>Seguimiento en Línea</h3>
<p>Consulta el estado de tu paquete.</p>
</div>

</div>
</section>

<section class="section container" id="rastreo">
<h2>Rastrea tu paquete</h2>
<div class="tracking">
<p>Ingresa tu número de guía</p>
<br>
<input id="trackingInput" type="text" placeholder="Ej: FL123456MX">
<button class="search" onclick="buscarPaquete()">Buscar</button>

<div class="result" id="resultado"></div>
</div>
</section>

<section class="section container" id="contacto">
<h2>Contacto</h2>
<p>Email: contacto@flashlightlogistica.com</p>
<p>Teléfono: +52 55 0000 0000</p>
<p>Horario: Lunes a Viernes 8:00 AM - 6:00 PM</p>
</section>

<footer>
<div class="container footer-grid">

<div>
<h4>Flash Light</h4>
<p>Empresa mexicana especializada en paquetería y logística.</p>
</div>

<div>
<h4>Servicios</h4>
<p>Envíos nacionales</p>
<p>Envíos express</p>
<p>Logística empresarial</p>
</div>

<div>
<h4>Calidad</h4>
<p>Sistema ISO 9001</p>
<p>Mejora continua</p>
</div>

</div>

<div class="copyright">
© 2026 Flash Light Paquetería & Logística
</div>
</footer>

<script>
function buscarPaquete(){

let guia=document.getElementById("trackingInput").value
let resultado=document.getElementById("resultado")

if(guia===""){
resultado.style.display="block"
resultado.innerHTML="Por favor ingresa un número de guía"
return
}

resultado.style.display="block"
resultado.innerHTML="\n<b>Guía:</b> "+guia+"<br><br>\n<b>Estado:</b> En tránsito 🚚<br>\n<b>Ubicación:</b> Centro Logístico CDMX<br>\n<b>Entrega estimada:</b> 24 - 48 horas\n"
}
</script>

</body>
</html>
