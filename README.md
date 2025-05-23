<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Blog Fundamento Tecnología de la Información</title>
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #f9f9f9;
      margin: 0;
      padding: 0;
      color: #333;
    }

    header {
      background-color: #34495e;
      color: white;
      padding: 30px 20px;
      text-align: center;
    }

    nav {
      background-color: #2c3e50;
      padding: 12px 0;
      text-align: center;
    }

    nav a {
      color: white;
      margin: 0 12px;
      text-decoration: none;
      font-size: 1rem;
      display: inline-block;
      padding: 8px 5px;
    }

    nav a:hover {
      text-decoration: underline;
    }

    /* NUEVO: estilo para la parte superior con "Sobre mí" y "Categorías" */
    .top-info {
      display: flex;
      justify-content: space-around;
      background-color: #ecf0f1;
      padding: 20px 10px;
      flex-wrap: wrap;
    }

    .top-info section {
      max-width: 500px;
      margin: 10px;
    }

    .top-info h3 {
      margin-top: 0;
      color: #2c3e50;
    }

    .top-info ul {
      list-style-type: none;
      padding-left: 0;
    }

    .top-info li {
      margin: 6px 0;
    }

    .top-info a {
      text-decoration: none;
      color: #1abc9c;
      font-weight: bold;
    }

    .top-info a:hover {
      text-decoration: underline;
    }

    .container {
      display: flex;
      flex-wrap: wrap;
      max-width: 1200px;
      margin: 20px auto;
      padding: 0 20px;
      gap: 20px;
    }

    main {
      flex: 1 1 60%;
    }

    article {
      background: white;
      padding: 20px;
      margin-bottom: 20px;
      border-radius: 6px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    article h2 {
      margin-bottom: 10px;
    }

    article p {
      line-height: 1.6;
    }

    .sidebar {
      flex: 1 1 35%;
      background-color: #ecf0f1;
      padding: 20px;
      border-radius: 6px;
      height: fit-content;
    }

    footer {
      background-color: #34495e;
      color: white;
      text-align: center;
      padding: 15px 0;
      margin-top: 40px;
    }

    @media (max-width: 768px) {
      nav a {
        display: block;
        margin: 10px 0;
      }

      .container {
        flex-direction: column;
        padding: 0 15px;
      }

      .sidebar {
        margin-top: 20px;
      }
    }

    @media (max-width: 480px) {
      header h1 {
        font-size: 1.5em;
      }

      nav a {
        font-size: 1em;
      }

      article h2 {
        font-size: 1.2em;
      }

      .top-info section {
        width: 100%;
        text-align: center;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Origen y Evolución</h1>
    <p>Historias y artículos interesantes</p>
  </header>

  <nav>
    <a href="#">Inicio</a>
    <a href="#">Categorías</a>
    <a href="#">Sobre mí</a>
    <a href="#">Contacto</a>
  </nav>

  <!-- NUEVO BLOQUE DE CATEGORÍAS Y SOBRE MÍ EN LA PARTE SUPERIOR -->
  <div class="top-info">
    <section class="about-top">
      <h3>Sobre mí</h3>
      <p>
        Primera página web de la materia Fundamentos de la Tecnología y la Información.<br>
        Universidad Autónoma de Guerrero, Facultad de Ingeniería en Computación.
      </p>
    </section>

    <section class="categories-top">
      <h3>Categorías</h3>
      <ul>
        <li><a href="Estructura_Componentes.html">Estructura y Componentes</a></li>
        <li><a href="Servicios_aplicaciones_internet.html">Servicios y aplicaciones de Internet</a></li>
        <li><a href="Seguridad_Internet.html">Seguridad en Internet</a></li>
        <li><a href="Nuevas_Tecnologias_Emergentes.html">Nuevas Tecnologías Emergentes</a></li>
      </ul>
    </section>
  </div>

  <div class="container">
    <main>
      <article>
        <h2><a href="Estructura_Componentes.html">🌄 Primer artículo: Estructura y Componentes</a></h2>
        <p><strong>Publicado el:</strong> 22 de mayo de 2025</p>
        <p>Este es el primer artículo del blog. Aquí puedes compartir tus pensamientos, experiencias o contenido informativo para tus lectores.</p>
      </article>

      <article>
        <h2>📚 Segundo artículo: Aprendiendo HTML</h2>
        <p><strong>Publicado el:</strong> 20 de mayo de 2025</p>
        <p>HTML es el lenguaje de marcado principal para la creación de páginas web. Con él puedes estructurar textos, imágenes, enlaces y mucho más.</p>
      </article>

      <article>
        <h2>🌄 Tercer artículo del blog</h2>
        <p><strong>Publicado el:</strong> 22 de mayo de 2025</p>
        <p>Este es el tercer artículo del blog. Aquí puedes compartir tus pensamientos, experiencias o contenido informativo para tus lectores.</p>
      </article>

      <article>
        <h2>🌄 Cuarto artículo del blog</h2>
        <p><strong>Publicado el:</strong> 22 de mayo de 2025</p>
        <p>Este es el cuarto artículo del blog. Aquí puedes compartir tus pensamientos, experiencias o contenido informativo para tus lectores.</p>
      </article>
    </main>

    <!-- Puedes eliminar este sidebar si ya no lo necesitas -->
    <aside class="sidebar">
      <h3>Sidebar (opcional)</h3>
      <p>Este espacio puede utilizarse para otros enlaces, banners o recursos relacionados.</p>
    </aside>
  </div>

  <footer>
    <p>&copy; 2025 Mi Blog Personal. Todos los derechos reservados.</p>
  </footer>

</body>
</html>
