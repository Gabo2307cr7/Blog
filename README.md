
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

      .sidebar h3 {
        font-size: 1.1em;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Blog Fundamento Tecnología de la Información</h1>
    <p>Historias y artículos interesantes</p>
  </header>

  <nav>
    <a href="#">Inicio</a>
    <a href="#">Categorías</a>
    <a href="#">Sobre mí</a>
    <a href="#">Contacto</a>
  </nav>

  <div class="container">
    <main>
      <article>
        <h2>🌄 Primer artículo: Estructura y Componentes</h2>
        <p><strong>Publicado el:</strong> <span id="fechaActual"></span></p>
        <p>Este es el primer artículo del blog. Aquí puedes compartir tus pensamientos, experiencias o contenido informativo para tus lectores.</p>
      </article>

      <article>
        <h2>📚 Segundo artículo: Servicios y Aplicaciones de Internet</h2>
        <p><strong>Publicado el:</strong> 20 de mayo de 2025</p>
        <p>HTML es el lenguaje de marcado principal para la creación de páginas web. Con él puedes estructurar textos, imágenes, enlaces y mucho más.</p>
      </article>

      <article>
        <h2>📚 Tercer artículo: Seguridad en Internet</h2>
        <p><strong>Publicado el:</strong> 20 de mayo de 2025</p>
        <p>HTML es el lenguaje de marcado principal para la creación de páginas web. Con él puedes estructurar textos, imágenes, enlaces y mucho más.</p>
      </article>

      <article>
        <h2>📚 Cuarto artículo: Nuevas tecnologías Emergentes</h2>
        <p><strong>Publicado el:</strong> 20 de mayo de 2025</p>
        <p>HTML es el lenguaje de marcado principal para la creación de páginas web. Con él puedes estructurar textos, imágenes, enlaces y mucho más.</p>
      </article>

      <article>
        <h2>📊 Encuesta: ¿Cuál es tu lenguaje de programación favorito?</h2>
        <form id="encuestaForm">
          <label><input type="radio" name="lenguaje" value="HTML" required> HTML</label><br>
          <label><input type="radio" name="lenguaje" value="CSS"> CSS</label><br>
          <label><input type="radio" name="lenguaje" value="JavaScript"> JavaScript</label><br>
          <label><input type="radio" name="lenguaje" value="Python"> Python</label><br><br>
          <button type="submit">Votar</button>
        </form>
        <p id="resultadoEncuesta" style="margin-top: 10px; font-weight: bold;"></p>
      </article>
    </main>

    <aside class="sidebar">
      <h3>Sobre mí</h3>
      <p>Soy un apasionado por la escritura, la tecnología y el diseño. Este blog es un espacio para compartir lo que aprendo cada día.</p>
      <hr>
      <h3>Categorías</h3>
      <ul>
        <li>Tecnología</li>
        <li>Reflexiones</li>
        <li>Diseño web</li>
        <li>Vida personal</li>
      </ul>
    </aside>
  </div>

  <footer>
    <p>&copy; 2025 Mi Blog Personal. Todos los derechos reservados.</p>
  </footer>

  <!-- JavaScript al final del body -->
  <script>
    // Mostrar fecha actual para el primer artículo
    document.getElementById("fechaActual").textContent = new Date().toLocaleDateString("es-ES", {
      year: "numeric", month: "long", day: "numeric"
    });

    // Encuesta interactiva
    document.getElementById('encuestaForm').addEventListener('submit', function(event) {
      event.preventDefault(); // Evita que recargue la página
      const seleccion = document.querySelector('input[name="lenguaje"]:checked');
      const resultado = document.getElementById('resultadoEncuesta');

      if (seleccion) {
        resultado.textContent = `¡Gracias por votar! Elegiste: ${seleccion.value}`;
      } else {
        resultado.textContent = 'Por favor, selecciona una opción.';
      }
    });
  </script>

</body>
</html>

