<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ACTIVÁ LO PÚBLICO</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Nunito', sans-serif;
      margin: 0;
      background-color: #ffffff;
      color: #051F3E;
      font-size: 1.2rem;
      line-height: 1.6;
    }

    header {
      position: relative;
      background: linear-gradient(135deg, #050A30, #5A77A6);
      color: white;
      padding: 2rem 2rem;
      text-align: left;
      border-radius: 0.2rem;
    }

    .header-logos {
      position: absolute;
      top: 1rem;
      right: 1rem;
      display: flex;
      gap: 1rem;
    }

    .header-logos img {
      height: 60px;
      border-radius: 0.5rem;
    }

    header h1 {
      font-size: 10rem;
      text-transform: uppercase;
      margin: 0;
    }

    header p {
      font-size:1.5rem;
      margin-top: 1rem;
    }

    section {
      padding: 2rem;
      max-width: 900px;
      margin: auto;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    h2 {
      background: #051F3E;
      padding: 1.5rem;
      color: white;
      border-radius: 0.5rem;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      margin-top: 1.5rem;
      opacity: 0;
      animation: fadeIn 1.2s ease forwards;
    }

    h2:nth-of-type(1) { animation-delay: 0.3s; }
    h2:nth-of-type(2) { animation-delay: 0.6s; }
    h2:nth-of-type(3) { animation-delay: 0.9s; }
    h2:nth-of-type(4) { animation-delay: 1.2s; }
    h2:nth-of-type(5) { animation-delay: 1.5s; }
    h2:nth-of-type(6) { animation-delay: 1.8s; }
    h2:nth-of-type(7) { animation-delay: 2.1s; }
    h2:nth-of-type(8) { animation-delay: 2.4s; }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .postulate-btn {
      display: block;
      width: fit-content;
      margin: 2rem auto;
      background: linear-gradient(135deg, #050A30, #5A77A6);
      color: white;
      font-size: 1.5rem;
      padding: 1rem 2rem;
      border: none;
      border-radius: 0.6rem;
      text-decoration: none;
      transition: background-color 0.3s;
    }

    .postulate-btn:hover {
      background-color: #3b558a;
    }

    footer.contacto {
      position: relative;
      background-color: #051F3E;
      color: white;
      text-align: center;
      padding: 2rem;
    }

    .footer-logos {
      position: absolute;
      bottom: 1rem;
      right: 1rem;
      display: flex;
      gap: 1rem;
    }

    .footer-logos img {
      height: 50px;
      border-radius: 0.5rem;
    }

    .timeline {
      position: relative;
      margin: 2rem 0;
      padding-left: 30px;
      border-left: 4px solid #5A77A6;
    }

    .event {
      margin-bottom: 1.5rem;
      position: relative;
    }

    .event::before {
      content: '';
      position: absolute;
      left: -10px;
      top: 0.3rem;
      width: 15px;
      height: 15px;
      background-color: #050A30;
      border-radius: 50%;
      border: 2px solid #5A77A6;
    }

    .event h4 {
      margin: 0;
      color: #050A30;
    }

    .event p {
      margin: 0.2rem 0 0 0;
    }

    .mision-destacada {
      background-color: #050A30;
      color: #FFFFFF;
      padding: 2rem;
      margin-top: 2rem;
      text-align: center;
      border-radius: 1rem;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 150px;
    }

    .mision-animada {
      font-size: 1.5rem;
      font-weight: bold;
      display: inline-block;
      white-space: nowrap;
      overflow: hidden;
    }

    .mision-animada span {
      opacity: 0;
      animation: escribir 0.05s forwards;
    }

    .mision-animada.completa {
      animation: titilar 1s ease-in-out 3s 2;
    }

    .criterios li {
      margin-bottom: 0.8rem;
    }

    @keyframes escribir {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }

    @keyframes titilar {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }
  </style>
</head>
<body>
  <header>
    <div class="header-logos">
      <img src="https://pbs.twimg.com/profile_images/1283194599230656518/w-jtPYkO_400x400.jpg" alt="Logo Red Actio" />
      <img src="https://www.voluntare.org/wp-content/uploads/2022/07/logo-fundacion-botin.png" alt="Logo Fundación Botín" />
    </div>
    <h1>Activá lo público</h1>
    <p>El programa para enamorar a las y los jóvenes de lo público</p>
  </header>

  <section>
    <h2>¿Quiénes somos?</h2>
    <p>Actio es una asociación civil integrada por personas comprometidas con el servicio público en Argentina...</p>

    <h2>¿Por qué “Activá lo Público”?</h2>
    <p>Buscamos despertar el compromiso de las y los jóvenes con el servicio público...</p>

    <a href="https://redactio.github.io/activalopublico" class="postulate-btn">¡Click acá para inscribirte!</a>

    <h2>Nuestros aliados</h2>
    <p>Creada en 1964, la Fundación Botín actúa en España y América Latina...</p>

    <h2>Misión</h2>
    <div class="mision-destacada">
      <p class="mision-animada" id="mision"></p>
    </div>

    <h2>Visión</h2>
    <p>Llegar a jóvenes de Argentina a través de una experiencia federal...</p>

    <h2>Público objetivo</h2>
    <p>Jóvenes de Argentina de 18 a 21 años...</p>

    <h2>Cronograma</h2>
    <div class="timeline">
      <!-- Fechas del cronograma -->
      <div class="event"><h4>17 de mayo</h4><p>Lanzamiento del programa...</p></div>
      <div class="event"><h4>7 de junio</h4><p>Cierre de postulaciones</p></div>
      <div class="event"><h4>15 de junio al 2 de julio</h4><p>Evaluación...</p></div>
      <div class="event"><h4>9 de julio</h4><p>Anuncio de seleccionados</p></div>
      <div class="event"><h4>6 de agosto</h4><p>Inicio etapa virtual</p></div>
      <div class="event"><h4>24 de septiembre</h4><p>Fin de la etapa virtual</p></div>
      <div class="event"><h4>10, 11 y 12 de octubre</h4><p>Actividad presencial</p></div>
    </div>

    <h2>Criterios de selección</h2>
    <ul class="criterios">
      <li>Poseer nacionalidad argentina.</li>
      <li>Haber nacido entre el 7 de agosto de 2003 y el 6 de agosto de 2007 inclusive.</li>
      <li>Haber finalizado el colegio secundario...</li>
      <li>Contar con buen expediente académico...</li>
      <li>Vocación de servicio...</li>
    </ul>

    <h2>Contenidos del programa</h2>
    <p>Formación intensiva, mentorías, actividades prácticas, encuentros con referentes públicos.</p>
  </section>

  <footer class="contacto">
    <p>redactioargentina@gmail.com | @red.actio</p>
    <p>CUIL No. 00-000000000-0</p>
    <div class="footer-logos">
      <img src="https://pbs.twimg.com/profile_images/1283194599230656518/w-jtPYkO_400x400.jpg" alt="Logo Red Actio" />
      <img src="https://www.voluntare.org/wp-content/uploads/2022/07/logo-fundacion-botin.png" alt="Logo Fundación Botín" />
    </div>
  </footer>

  <script>
    const contenedor = document.getElementById("mision");
    const frase = "Que más de las y los mejores se enamoren de lo público";

    function animarFrase() {
      contenedor.innerHTML = "";
      frase.split("").forEach((letra, index) => {
        const span = document.createElement("span");
        span.textContent = letra;
        span.style.animationDelay = `${index * 0.05}s`;
        contenedor.appendChild(span);
      });
      const duracionAparicion = frase.length * 50 + 500;
      setTimeout(() => {
        contenedor.classList.add("blink");
      }, duracionAparicion);
      setTimeout(() => {
        contenedor.classList.remove("blink");
        animarFrase();
      }, duracionAparicion + 1500);
    }

    animarFrase();
  </script>
</body>
</html>
