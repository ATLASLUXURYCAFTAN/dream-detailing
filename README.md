<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Dream Detailing - DREAM DETALING </title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0; padding: 0;
      background: #000;
      color: #fff;
      scroll-behavior: smooth;
    }
    header {
      position: fixed;
      width: 100%;
      background: rgba(0,0,0,0.85);
      color: white;
      padding: 15px 30px;
      top: 0;
      z-index: 1000;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 2px 10px rgba(255,255,255,0.1);
      font-weight: 600;
      letter-spacing: 1px;
    }
    nav a {
      color: white;
      margin-left: 20px;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
      text-transform: uppercase;
    }
    nav a:hover {
      color: #d4af37; /* Dorado elegante */
    }
    section {
      padding: 100px 20px 60px;
      max-width: 1000px;
      margin: 0 auto;
      opacity: 0;
      transform: translateY(30px);
      transition: all 0.6s ease-out;
    }
    section.visible {
      opacity: 1;
      transform: translateY(0);
    }
    .hero {
      background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1200&q=80') center/cover no-repeat;
      height: 500px;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #d4af37;
      font-size: 3rem;
      font-weight: bold;
      text-shadow: 2px 2px 8px rgba(0,0,0,0.9);
      margin-top: 60px;
      letter-spacing: 3px;
    }
    .service {
      display: flex;
      align-items: center;
      margin-bottom: 40px;
      border-bottom: 1px solid #333;
      padding-bottom: 30px;
    }
    .service:nth-child(even) {
      flex-direction: row-reverse;
    }
    .service img {
      width: 45%;
      border-radius: 15px;
      box-shadow: 0 8px 20px rgba(212,175,55,0.5);
      border: 2px solid #d4af37;
    }
    .service-text {
      width: 50%;
      padding: 0 20px;
    }
    .service-text h2 {
      color: #d4af37;
      margin-bottom: 15px;
      font-size: 2rem;
      letter-spacing: 2px;
    }
    .service-text p {
      font-size: 1.1rem;
      line-height: 1.6;
      color: #eee;
    }
    form {
      background: #111;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 8px 30px rgba(212,175,55,0.4);
      max-width: 600px;
      margin: 0 auto;
      color: #eee;
    }
    form label {
      display: block;
      margin-top: 15px;
      font-weight: 600;
      color: #d4af37;
      letter-spacing: 1px;
    }
    form input, form textarea {
      width: 100%;
      padding: 12px;
      margin-top: 5px;
      border-radius: 8px;
      border: 1px solid #444;
      background: #222;
      color: #eee;
      font-size: 1rem;
      box-sizing: border-box;
      transition: border-color 0.3s;
    }
    form input:focus, form textarea:focus {
      border-color: #d4af37;
      outline: none;
    }
    form button {
      margin-top: 25px;
      background: #d4af37;
      border: none;
      padding: 15px 35px;
      color: black;
      font-weight: 700;
      border-radius: 10px;
      cursor: pointer;
      font-size: 1.2rem;
      letter-spacing: 2px;
      transition: background 0.3s;
      text-transform: uppercase;
    }
    form button:hover {
      background: #b38f1a;
    }
    footer {
      text-align: center;
      padding: 25px;
      background: #111;
      color: #d4af37;
      font-weight: 600;
      letter-spacing: 1.5px;
      margin-top: 40px;
    }
    @media (max-width: 768px) {
      .service {
        flex-direction: column !important;
      }
      .service img, .service-text {
        width: 100%;
        padding: 0;
      }
      section {
        padding: 80px 15px 40px;
      }
      .hero {
        font-size: 2rem;
        height: 350px;
        letter-spacing: 1.5px;
      }
    }
  </style>
</head>
<body>

<header>
  <div>DREAM DETAILING</div>
  <nav>
    <a href="#servicios">Servicios</a>
    <a href="#contacto">Contacto</a>
  </nav>
</header>

<div class="hero">LUJO & ELEGANCIA</div>

<section id="servicios">
  <div class="service">
    <img src="https://images.unsplash.com/photo-1502877338535-766e1452684a?auto=format&fit=crop&w=600&q=80" alt="Reparación Rápida" />
    <div class="service-text">
      <h2>Reparación Rápida</h2>
      <p>Soluciones inmediatas para vehículos de alta gama: cambio de aceite, frenos, baterías, neumáticos y más, con la máxima calidad y rapidez.</p>
    </div>
  </div>
  <div class="service">
    <img src="https://images.unsplash.com/photo-1549924231-f129b911e442?auto=format&fit=crop&w=600&q=80" alt="Detailing Profesional" />
    <div class="service-text">
      <h2>Detailing Profesional</h2>
      <p>Cuidado y limpieza integral para que tu coche de lujo luzca impecable, por dentro y por fuera, con productos y técnicas premium.</p>
    </div>
  </div>
</section>

<section id="contacto">
  <h2>Contacto</h2>
  <form>
    <label for="nombre">Nombre completo</label>
    <input type="text" id="nombre" name="nombre" required />

    <label for="telefono">Teléfono</label>
    <input type="tel" id="telefono" name="telefono" />

    <label for="mensaje">Mensaje</label>
    <textarea id="mensaje" name="mensaje" rows="4" placeholder="Cuéntanos qué necesitas..."></textarea>

    <button type="submit">Enviar</button>
  </form>
</section>

<footer>
  <p>&copy; 2025 Dream Detailing. Todos los derechos reservados.</p>
</footer>

<script>
  // Animar secciones al hacer scroll
  const sections = document.querySelectorAll('section');
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if(entry.isIntersecting) {
        entry.target.classList.add('visible');
      }
    });
  }, { threshold: 0.1 });

  sections.forEach(section => {
    observer.observe(section);
  });

  // Al enviar formulario
  document.querySelector('form').addEventListener('submit', e => {
    e.preventDefault();
    alert('¡Gracias por contactarnos! Te responderemos pronto.');
    e.target.reset();
  });
</script>

</body>
</html>
