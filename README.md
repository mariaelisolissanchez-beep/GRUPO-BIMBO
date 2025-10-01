# GRUPO-BIMBO
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Manuales Bimbo - Proyecto Escolar</title>
  <!-- Fuentes y librerías -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link href="https://unpkg.com/aos@2.3.4/dist/aos.css" rel="stylesheet">
  
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: 'Poppins', sans-serif; line-height: 1.6; background:#fff; color:#333; }
    a { text-decoration: none; }

    /* HEADER */
    header {
      height: 100vh;
      background: linear-gradient(rgba(0,75,147,0.7), rgba(227,6,19,0.7)),
                  url('banner-pan.jpg') center/cover no-repeat;
      display: flex; flex-direction: column; justify-content: center; align-items: center;
      text-align: center; color: white; padding: 20px;
    }
    header h1 { font-size: 3.5em; margin-bottom: 20px; }
    header p { font-size: 1.4em; max-width: 600px; }

    /* NAV */
    nav {
      background: white; position: sticky; top:0; z-index:1000; padding:15px;
      display: flex; justify-content: center; gap: 25px;
      box-shadow:0 3px 8px rgba(0,0,0,0.1);
    }
    nav a {
      color:#004B93; font-weight:600; transition: all 0.3s;
      position: relative;
    }
    nav a::after {
      content: ""; width:0%; height:3px; background:#E30613;
      position: absolute; left:0; bottom:-5px; transition: width 0.3s;
    }
    nav a:hover::after { width:100%; }

    /* MANUALES */
    .manuales { display:flex; flex-wrap:wrap; justify-content:center; gap:30px; padding:70px 20px; }
    .card {
      width:280px; padding:25px; border-radius:15px; text-align:center;
      box-shadow:0 6px 15px rgba(0,0,0,0.1); transition:all 0.4s; 
      background:#fff; position:relative; overflow:hidden;
    }
    .card:hover { transform:translateY(-10px) scale(1.02); box-shadow:0 12px 25px rgba(0,0,0,0.25); }
    .card i { font-size:40px; margin-bottom:15px; color:#004B93; }
    .card h2 { margin-bottom:12px; color:#004B93; }
    .card p { margin-bottom:20px; }
    .btn {
      display:inline-block; background:#E30613; color:white; padding:12px 20px;
      border-radius:8px; font-weight:600; transition:all 0.3s;
    }
    .btn:hover { background:#BF0810; transform:scale(1.05); }

    /* SOBRE */
    .sobre { padding:80px 20px; background:#F7F7F7; text-align:center; }
    .sobre h2 { color:#004B93; margin-bottom:20px; font-size:2.2em; }
    .sobre p { max-width:800px; margin:10px auto; font-size:1.1em; }

    /* FOOTER */
    footer {
      background: linear-gradient(90deg,#004B93,#E30613);
      color:white; text-align:center; padding:40px 20px;
    }
    footer .social { margin:15px 0; }
    footer .social a {
      color:white; margin:0 10px; font-size:1.5em; transition:0.3s;
    }
    footer .social a:hover { color: #FFD700; }
    footer p { margin:6px 0; }

    /* RESPONSIVE */
    @media(max-width:900px){
      header h1{ font-size:2.5em; }
      .manuales { flex-direction:column; align-items:center; }
    }
  </style>
</head>
<body>

  <!-- HEADER -->
  <header>
    <h1 data-aos="fade-down">Manuales Organizacionales Bimbo</h1>
    <p data-aos="fade-up">Proyecto académico de Organización | Una visión completa de la empresa líder en panificación</p>
  </header>

  <!-- NAV -->
  <nav>
    <a href="#manuales">Manuales</a>
    <a href="#sobre">Sobre Bimbo</a>
    <a href="#contacto">Contacto</a>
  </nav>

  <!-- SECCIÓN MANUALES -->
  <section class="manuales" id="manuales">
    <div class="card bienvenida" data-aos="zoom-in">
      <i class="fa-solid fa-handshake"></i>
      <h2>Manual de Bienvenida</h2>
      <p>Conoce la cultura, historia y valores de Grupo Bimbo.</p>
      <a href="manual-bienvenida.pdf" class="btn">Ver Manual</a>
    </div>

    <div class="card procesos" data-aos="zoom-in" data-aos-delay="100">
      <i class="fa-solid fa-gears"></i>
      <h2>Manual de Procesos</h2>
      <p>Procedimientos clave para la operación eficiente.</p>
      <a href="manual-procesos.pdf" class="btn">Ver Manual</a>
    </div>

    <div class="card organizacion" data-aos="zoom-in" data-aos-delay="200">
      <i class="fa-solid fa-sitemap"></i>
      <h2>Manual de Organización</h2>
      <p>Estructura jerárquica y funciones principales.</p>
      <a href="manual-organizacion.pdf" class="btn">Ver Manual</a>
    </div>

    <div class="card politicas" data-aos="zoom-in" data-aos-delay="300">
      <i class="fa-solid fa-book"></i>
      <h2>Manual de Políticas</h2>
      <p>Normas y lineamientos internos de la empresa.</p>
      <a href="#" class="btn">Próximamente</a>
    </div>

    <div class="card seguridad" data-aos="zoom-in" data-aos-delay="400">
      <i class="fa-solid fa-shield-halved"></i>
      <h2>Manual de Seguridad</h2>
      <p>Protocolos de seguridad y prevención de riesgos.</p>
      <a href="#" class="btn">Próximamente</a>
    </div>
  </section>

  <!-- SECCIÓN SOBRE BIMBO -->
  <section class="sobre" id="sobre">
    <h2 data-aos="fade-up">Sobre Bimbo</h2>
    <p data-aos="fade-up" data-aos-delay="100">
      Grupo Bimbo es la empresa de panificación más grande del mundo, con presencia en más de 30 países y un portafolio de más de 13,000 productos.
      Su misión es alimentar un mundo mejor y su visión es ser la empresa de alimentos más confiable, sustentable y cercana a los consumidores.
    </p>
  </section>

  <!-- FOOTER -->
  <footer id="contacto">
    <div class="social">
      <a href="#"><i class="fab fa-facebook"></i></a>
      <a href="#"><i class="fab fa-twitter"></i></a>
      <a href="#"><i class="fab fa-instagram"></i></a>
    </div>
    <p>Proyecto escolar | Organización | Tu Nombre</p>
    <p><i>No es una página oficial de Grupo Bimbo</i></p>
  </footer>

  <!-- JS de animaciones -->
  <script src="https://unpkg.com/aos@2.3.4/dist/aos.js"></script>
  <script>
    AOS.init({ duration: 1000, once: true });
  </script>
</body>
