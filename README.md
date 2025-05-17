<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Activá lo Público</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Luckiest+Guy&display=swap" rel="stylesheet">
  <style>
    :root {
      --celeste: #4DB6E9;
      --azul: #243782;
      --amarillo: #FFF200;
      --rojo: #9C1E25;
      --gris: #E6E6E6;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Montserrat', sans-serif;
      background-color: white;
      color: var(--azul);
      line-height: 1.6;
    }

    header {
      background: linear-gradient(to right, var(--celeste), var(--azul));
      color: white;
      padding: 2rem;
      text-align: center;
    }

    header img {
      max-height: 60px;
      vertical-align: middle;
      margin: 0 1rem;
    }

    h1 {
      font-family: 'Luckiest Guy', cursive;
      font-size: 2.5rem;
    }

    section {
      padding: 3rem 1rem;
      max-width: 900px;
      margin: auto;
    }

    .logos {
      display: flex;
      justify-content: center;
      gap: 2rem;
      padding: 1rem;
      background-color: var(--gris);
    }

    .logos img {
      max-height: 80px;
    }

    .cta {
      text-align: center;
      margin-top: 2rem;
    }

    .cta a {
      background-color: var(--rojo);
      color: white;
      text-decoration: none;
      padding: 1rem 2rem;
      border-radius: 8px;
      font-weight: bold;
    }

    footer {
      background-color: var(--gris);
      color: #555;
      text-align: center;
      padding: 1rem;
    }
  </style>
</head>
<body>
  <header>
    <div>
      <img src="./mnt/data/Logo-Actio-png.png" alt="Red Actio" />
      <h1>Activá lo Público</h1>
      <img src="./mnt/data/LOGO-Botin-png.png" alt="Fundación Botín" />
    </div>
  </header>

  <section>
    <h2>Un programa para despertar tu vocación pública</h2>
    <p>
      "Activá lo Público" es una iniciativa de la Red Argentina de Servidores Públicos con el acompañamiento de la Fundación Botín. Está destinado a jóvenes de entre 18 y 21 años que quieran explorar su vocación por el servicio público.
    </p>
    <p>
      A través de actividades participativas, mentorías y espacios de reflexión, buscamos despertar ese "gen" del liderazgo público que muchos llevan dentro.
    </p>
    <div class="cta">
      <a href="#">¡Postulate ahora!</a>
    </div>
  </section>

  <div class="logos">
    <img src="./mnt/data/Captura de pantalla 2025-05-16 215345.png" alt="Logo Activá lo Público" />
    <img src="./mnt/data/Logo-Actio-png.png" alt="Red Actio" />
    <img src="./mnt/data/LOGO-Botin-png.png" alt="Fundación Botín" />
  </div>

  <footer>
    <p>© 2025 Activá lo Público. Una iniciativa de la Red Actio con el apoyo de la Fundación Botín.</p>
  </footer>
</body>
</html>
