<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ACTIVÁ LO PÚBLICO</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #CAE8FF;
      color: #051F3E;
      font-size: 5rem;
    }

    header {
      background-color: #050A30;
      color: white;
      padding: 2rem;
      text-align: center;
    }

    header h1 {
      font-size: 3rem;
      text-transform: uppercase;
    }

    section {
      padding: 2rem;
      max-width: 900px;
      margin: auto;
    }

    h2 {
      color: #050A30;
      border-bottom: 2px solid #5A77A6;
      padding-bottom: 0.5rem;
      margin-top: 2rem;
      background-color: #7393C6;
      padding: 1rem;
      color: white;
      border-radius: 0.5rem;
    }

    footer {
      background-color: #051F3E;
      color: white;
      text-align: center;
      padding: 1rem;
    }

    .contacto {
      background-color: #7393C6;
      padding: 1rem;
      color: white;
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

    @keyframes escribir {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }

    @keyframes titilar {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }

    .mision-destacada {
      background-color: #050A30;
      color: #FFFFFF;
      padding: 2rem;
      margin-top: 2rem;
      text-align: center;
      border-radius: 1rem;
    }

    .mision-animada {
      font-family: Impact, sans-serif;
      font-size: 1.8rem;
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
  </style>
</head>
<body>

  <header>
    <h1>Activá lo Público</h1>
    <p>El programa para enamorar a las y los jóvenes de lo público</p>
  </header>

  <section>
    <h2>¿Quiénes somos?</h2>
    <p>Actio es una asociación civil integrada por personas comprometidas con el servicio público en Argentina. Fundada en 2020 por exbecarios del Programa para el Fortalecimiento de la Función Pública en América Latina de la Fundación Botín, reúne actualmente a 74 miembros. Su propósito es consolidarse como un espacio de articulación, formación y colaboración para promover y fortalecer la función pública en el país.</p>

    <h2>¿Por qué “Activá lo Público”?</h2>
    <p>Buscamos despertar el compromiso de las y los jóvenes con el servicio público, a través de una experiencia virtual con sesiones semanales que los conecte con referentes de cada sector y estimule su comprensión de lo público. Además, proponemos una experiencia vivencial de 3 días para las y los 25 mejores estudiantes de la etapa virtual.</p>

    <h2>Nuestros aliados</h2>
    <p>Creada en 1964, la Fundación Botín actúa en España y América Latina con la misión de contribuir al desarrollo integral de la sociedad. Para ello, impulsa nuevas formas de identificar y potenciar el talento creativo, generando riqueza cultural, social y económica. Sus programas abarcan los campos del arte y la cultura, la educación, el fortalecimiento institucional, la ciencia y el desarrollo rural.</p>

    <h2>Misión</h2>
    <div class="mision-destacada">
      <p class="mision-animada" id="mision"></p>
    </div>

    <h2>Visión</h2>
    <p>Llegar a jóvenes de Argentina a través de una experiencia federal y latinoamericanista, con un componente vivencial y otro formativo, que contribuya a entender, involucrarse y defender el valor de lo público.</p>

    <h2>Público objetivo</h2>
    <p>Jóvenes de Argentina de 18 a 21 años que hayan finalizado el colegio secundario y estén cursando estudios universitarios de grado o terciarios.</p>

    <h2>Cronograma</h2>
    <div class="timeline">
      <div class="timeline-container left">
        <div class="content">
          <h3>17 de mayo</h3>
          <p>Lanzamiento del programa y apertura de inscripciones</p>
        </div>
      </div>
      <div class="timeline-container right">
        <div class="content">
          <h3>7 de junio</h3>
          <p>Cierre de postulaciones</p>
        </div>
      </div>
      <div class="timeline-container left">
        <div class="content">
          <h3>15 de junio al 2 de julio</h3>
          <p>Evaluación de postulaciones y entrevistas</p>
        </div>
      </div>
      <div class="timeline-container right">
        <div class="content">
          <h3>9 de julio</h3>
          <p>Anuncio de seleccionados para la etapa virtual</p>
        </div>
      </div>
      <div class="timeline-container left">
        <div class="content">
          <h3>6 de agosto</h3>
          <p>Inicio de la etapa virtual</p>
        </div>
      </div>
      <div class="timeline-container right">
        <div class="content">
          <h3>24 de septiembre</h3>
          <p>Fin de la etapa virtual y anuncio de seleccionados/as para la etapa presencial</p>
        </div>
      </div>
      <div class="timeline-container left">
        <div class="content">
          <h3>10, 11 y 12 de octubre</h3>
          <p>Actividad presencial</p>
        </div>
      </div>
    </div>

    <h2>Criterios de selección</h2>
    <ul class="criterios">
      <li>Poseer nacionalidad argentina.</li>
      <li>Haber nacido entre el 7 de agosto de 2003 y el 6 de agosto de 2007 inclusive, a la fecha de inicio del programa.</li>
      <li>Haber finalizado el colegio secundario, ser estudiante universitario o terciario y no haber cursado aún más del 50% de la carrera.</li>
      <li>Contar con buen expediente académico y compromiso social.</li>
      <li>Vocación de servicio e interés por ser agente de cambio.</li>
    </ul>

    <h2>Contenidos del programa</h2>
    <p>Formación intensiva, mentorías, actividades prácticas, encuentros con referentes públicos.</p>
  </section>

  <footer class="contacto">
    <p>redactioargentina@gmail.com | @red.actio</p>
    <p>CUIL No. 00-000000000-0</p>
  </footer>

<script>
  const contenedor = document.getElementById("mision");
  const frase = "Que más de las y los mejores se enamoren de lo público";

  function animarFrase() {
    contenedor.innerHTML = ""; // limpiar para reiniciar

    // Crear spans con delay progresivo
    frase.split("").forEach((letra, index) => {
      const span = document.createElement("span");
      span.textContent = letra;
      span.style.animationDelay = `${index * 0.05}s`;
      contenedor.appendChild(span);
    });

    // Tiempo total de la animación de aparición + un pequeño delay
    const duracionAparicion = frase.length * 50 + 500; // ms

    // Después que todas las letras aparecen, agregar clase blink para titilar
    setTimeout(() => {
      contenedor.classList.add("blink");
    }, duracionAparicion);

    // Quitar clase blink y reiniciar animación para repetir
    setTimeout(() => {
      contenedor.classList.remove("blink");
      animarFrase();
    }, duracionAparicion + 1500); // tiempo total para ciclo completo
  }

  animarFrase();
</script>
</body>
</html>
