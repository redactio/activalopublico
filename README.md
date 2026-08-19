<!--<!DOCTYPE html>-->
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Activá lo Público</title>
    <style>
        /* Estilos Generales y Reseteo */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }

        /* Header Responsivo */
        header {
            background: linear-gradient(135deg, #050A30, #5A77A6);
            color: white;
            padding: 4rem 2rem;
            text-align: center;
            position: relative;
        }
        .header-logos {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-bottom: 2rem;
        }
        .header-logos img {
            height: 60px;
            border-radius: 0.5rem;
            background-color: white;
            padding: 5px;
        }
        header h1 {
            font-size: clamp(3rem, 8vw, 8rem);
            text-transform: uppercase;
            margin: 0;
            line-height: 1.1;
        }
        header p {
            font-size: clamp(1.2rem, 3vw, 1.5rem);
            margin-top: 1rem;
            font-weight: 300;
        }

        /* Secciones */
        section {
            padding: 2rem;
            max-width: 900px;
            margin: auto;
        }
        
        /* Títulos H2 Animados */
        h2 {
            background: #051F3E;
            padding: 1.5rem;
            color: white;
            border-radius: 0.5rem;
            text-align: center;
            margin-top: 3rem;
            margin-bottom: 1.5rem;
            opacity: 0;
            animation: fadeIn 1.2s ease forwards;
        }
        h2:nth-of-type(1) { animation-delay: 0.3s; }
        h2:nth-of-type(2) { animation-delay: 0.6s; }
        h2:nth-of-type(3) { animation-delay: 0.9s; }
        h2:nth-of-type(4) { animation-delay: 1.2s; }
        h2:nth-of-type(5) { animation-delay: 1.5s; }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Misión Destacada */
        .mision-destacada {
            background-color: #050A30;
            color: #FFFFFF;
            padding: 3rem 2rem;
            margin-top: 2rem;
            text-align: center;
            border-radius: 1rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        .mision-destacada h3 {
            font-size: 1.8rem;
            margin-bottom: 1rem;
            color: #7393C6;
        }

        /* Listas y Criterios */
        .criterios, .contenidos {
            list-style: none;
            padding: 0;
        }
        .criterios li, .contenidos li {
            background: white;
            margin-bottom: 0.8rem;
            padding: 1rem;
            border-left: 5px solid #5A77A6;
            border-radius: 4px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }

        /* Timeline (Fechas Clave) */
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
            left: -39px;
            top: 0.2rem;
            width: 15px;
            height: 15px;
            background-color: #050A30;
            border-radius: 50%;
            border: 3px solid #5A77A6;
        }
        .event h4 {
            margin: 0;
            color: #050A30;
            font-size: 1.2rem;
        }
        .event p {
            margin: 0.2rem 0 0 0;
            color: #555;
        }

        /* Botón de Postulación */
        .postulate-btn {
            display: block;
            width: fit-content;
            margin: 3rem auto;
            background: linear-gradient(135deg, #050A30, #5A77A6);
            color: white;
            font-size: 1.5rem;
            font-weight: bold;
            padding: 1rem 2.5rem;
            border: none;
            border-radius: 0.6rem;
            text-decoration: none;
            text-align: center;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(5, 10, 48, 0.4);
        }
        .postulate-btn:hover {
            background: linear-gradient(135deg, #051F3E, #7393C6);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(5, 10, 48, 0.6);
        }

        /* Footer y Contacto */
        footer {
            background-color: #051F3E;
            color: white;
            text-align: center;
            padding: 2rem 1rem;
            margin-top: 3rem;
        }
        .contacto {
            background-color: #7393C6;
            padding: 1.5rem;
            color: white;
            border-radius: 0.5rem;
            margin-bottom: 2rem;
        }
        .contacto p {
            margin-bottom: 0.5rem;
            font-size: 1.1rem;
        }

        /* Media Queries para Tablets y Móviles */
        @media (min-width: 768px) {
            header {
                text-align: left;
                padding: 6rem 4rem;
            }
            .header-logos {
                position: absolute;
                top: 2rem;
                right: 2rem;
                margin-bottom: 0;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="header-logos">
            <img src="logo-actio.png" alt="Actio"><!--[cite: 1] -->
            <img src="logo-botin.png" alt="Fundación Botín"><!--[cite: 1] -->
        </div>
        <h1>Activá<br>lo Público</h1>
        <p>El programa para enamorar a las juventudes de lo público.<!--[cite: 1] --></p>
        <a href="#fechas" class="postulate-btn">#SeActiva<!--[cite: 1] --></a>
    </header>

    <section>
        <div class="mision-destacada">
            <h3>Nuestra Misión</h3>
            <p>Que más de las y los mejores se enamoren de lo público.<!--[cite: 1] --></p>
        </div>

        <h2>¿Quiénes Somos?</h2>
        <p><strong>Actio</strong> es una asociación civil formada por personas comprometidas con la función pública en Argentina, fundada en 2020 por ex becarios del Programa para el Fortalecimiento de la Función Pública en América Latina de la Fundación Botín. Actualmente reúne a 74 miembros.<!--[cite: 1] --></p>
        <br>
        <p>Nuestro principal aliado es la <strong>Fundación Botín</strong>, creada en 1964, que actúa en toda España y América Latina con la misión de contribuir al desarrollo integral de la sociedad.<!--[cite: 1] --></p>

        <h2>El Programa</h2>
        <p>Buscamos llegar a jóvenes de Argentina a través de una experiencia federal y latinoamericanista, con un componente vivencial y otro formativo, que contribuya a entender, involucrarse y defender el valor de lo público.<!--[cite: 1] --></p>
        <br>
        <h3>Etapa Virtual</h3>
        <p>Participan 50 jóvenes de todas las provincias argentinas. Incluye clases magistrales semanales, conversaciones, talleres de simulación de toma de decisiones y encuentros virtuales con referentes de nuestro país y toda Latinoamérica.<!--[cite: 1] --></p>
        <br>
        <h3>Etapa Presencial</h3>
        <p>Se seleccionarán 25 participantes con base en su desempeño e interés demostrado en la fase virtual. Se realizará en la Provincia de Córdoba, en el camping de AGEC (Santa Ana).<!--[cite: 1] --> Sus tres ejes fundamentales son:</p>
        <ul class="contenidos">
            <li>Actividad vivencial.<!--[cite: 1] --></li>
            <li>Conversaciones con líderes.<!--[cite: 1] --></li>
            <li>Espacios de networking.<!--[cite: 1] --></li>
        </ul>

        <h2>Público y Criterios de Selección</h2>
        <p>El programa está dirigido a jóvenes de Argentina de 18 a 21 años que hayan finalizado el colegio secundario y estén cursando estudios universitarios de grado o terciarios.<!--[cite: 1] --></p>
        <br>
        <ul class="criterios">
            <li>Poseer nacionalidad argentina.<!--[cite: 1] --></li>
            <li>Haber nacido entre el 14 de Julio de 2004 y el 13 de Julio de 2008 inclusive.<!--[cite: 1] --></li>
            <li>Haber finalizado el colegio secundario, ser estudiante universitario o terciario y no haber cursado aún más del 50% de la carrera.<!--[cite: 1] --></li>
            <li>Contar con buen expediente académico y compromiso social.<!--[cite: 1] --></li>
            <li>Vocación de servicio e interés por ser agente de cambio.<!--[cite: 1] --></li>
        </ul>

        <h2 id="fechas">Fechas Clave</h2>
        <div class="timeline">
            <div class="event">
                <h4>27 de Abril</h4>
                <p>Lanzamiento y apertura de postulaciones.<!--[cite: 1] --></p>
            </div>
            <div class="event">
                <h4>29 de Mayo</h4>
                <p>Cierre del período de postulaciones.<!--[cite: 1] --></p>
            </div>
            <div class="event">
                <h4>Hasta el 24 de Junio</h4>
                <p>Período de evaluación de postulaciones.<!--[cite: 1] --></p>
            </div>
            <div class="event">
                <h4>Hasta el 1 de Julio</h4>
                <p>Etapa de entrevistas.<!--[cite: 1] --></p>
            </div>
            <div class="event">
                <h4>5 de Julio</h4>
                <p>Inicio de la etapa virtual.<!--[cite: 1] --></p>
            </div>
            <div class="event">
                <h4>22 de Julio</h4>
                <p>Anuncio de seleccionados y seleccionadas.<!--[cite: 1] --></p>
            </div>
            <div class="event">
                <h4>9 de Septiembre</h4>
                <p>Fin de la etapa virtual.<!--[cite: 1] --></p>
            </div>
            <div class="event">
                <h4>14 de Septiembre</h4>
                <p>Anuncio de seleccionados y seleccionadas para la etapa presencial.<!--[cite: 1] --></p>
            </div>
            <div class="event">
                <h4>2, 3 y 4 de Octubre</h4>
                <p>Etapa presencial.<!--[cite: 1] --></p>
            </div>
        </div>

        <!-- REEMPLAZÁ ACÁ EL LINK DE POSTULACIÓN -->
        <a href="https://ejemplo.com/tu-formulario" target="_blank" class="postulate-btn">Postulate Aquí</a>
    </section>

    <footer>
        <div class="contacto">
            <h3>Contacto</h3>
            <p>Email: redactioargentina@gmail.com<!--[cite: 1] --></p>
            <p>Instagram: @red.actio<!--[cite: 1] --></p>
        </div>
        <p>© 2026 Activá lo Público. Desarrollado por la Asociación Civil Actio.<!--[cite: 1] --></p>
    </footer>

</body>
</html>
