<!--<!DOCTYPE html>-->
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Activá lo Público</title>
    <!-- Fuentes modernas: Poppins para dar un look limpio, juvenil y profesional -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        /* Reseteo y Base */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #F4F7F6; /* Un gris/celeste muy claro, más cálido que el blanco puro */
            color: #2C3E50;
            line-height: 1.7;
            overflow-x: hidden;
        }

        /* Utilidades */
        .text-highlight {
            color: #5A77A6;
            font-weight: 700;
        }

        /* Header Moderno con Curva */
        header {
            background: linear-gradient(135deg, #050A30 0%, #1a2b5e 50%, #5A77A6 100%);
            color: white;
            padding: 5rem 2rem 8rem 2rem;
            text-align: center;
            position: relative;
        }
        
        .header-logos {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-bottom: 3rem;
            position: relative;
            z-index: 2;
        }
        
        .header-logos img {
            height: 65px;
            border-radius: 8px;
            background-color: rgba(255, 255, 255, 0.95);
            padding: 8px 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }
        .header-logos img:hover {
            transform: translateY(-3px);
        }

        header h1 {
            font-size: clamp(3rem, 8vw, 6.5rem);
            text-transform: uppercase;
            font-weight: 700;
            margin: 0;
            line-height: 1.05;
            letter-spacing: -2px;
            position: relative;
            z-index: 2;
            text-shadow: 0 4px 20px rgba(5, 10, 48, 0.4);
        }

        header p {
            font-size: clamp(1.1rem, 3vw, 1.4rem);
            margin-top: 1.5rem;
            font-weight: 300;
            opacity: 0.9;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            position: relative;
            z-index: 2;
        }

        /* SVG Curva de fondo para dar "calidez" y romper la estructura rígida */
        .custom-shape-divider-bottom {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            overflow: hidden;
            line-height: 0;
            transform: rotate(180deg);
        }
        .custom-shape-divider-bottom svg {
            position: relative;
            display: block;
            width: calc(100% + 1.3px);
            height: 70px;
        }
        .custom-shape-divider-bottom .shape-fill {
            fill: #F4F7F6;
        }

        /* Botón Principal (Glassmorphism sutil) */
        .btn-header {
            display: inline-block;
            margin-top: 2.5rem;
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.3);
            color: white;
            font-size: 1.2rem;
            font-weight: 600;
            padding: 1rem 3rem;
            border-radius: 50px;
            text-decoration: none;
            transition: all 0.3s ease;
            position: relative;
            z-index: 2;
        }
        .btn-header:hover {
            background: white;
            color: #050A30;
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.15);
        }

        /* Secciones y Contenedores */
        section {
            padding: 5rem 2rem;
            max-width: 1000px;
            margin: auto;
        }
        
        /* Títulos H2 refinados */
        h2 {
            font-size: 2.2rem;
            color: #050A30;
            text-align: center;
            margin-bottom: 3rem;
            font-weight: 700;
            position: relative;
            padding-bottom: 1rem;
        }
        h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 4px;
            background: #7393C6;
            border-radius: 2px;
        }

        /* Misión Destacada - Convertida en una tarjeta elegante */
        .mision-destacada {
            background: white;
            padding: 3.5rem 2rem;
            margin-top: -8rem; /* Sube la tarjeta sobre el header */
            position: relative;
            z-index: 10;
            text-align: center;
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(5, 10, 48, 0.08);
            border-top: 6px solid #5A77A6;
            margin-bottom: 4rem;
        }
        .mision-destacada h3 {
            font-size: 1.2rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            color: #7393C6;
            margin-bottom: 1rem;
            font-weight: 600;
        }
        .mision-destacada p {
            font-size: 1.6rem;
            font-weight: 700;
            color: #050A30;
            line-height: 1.4;
        }

        /* Textos Generales */
        .text-block {
            background: white;
            padding: 2.5rem;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.03);
            margin-bottom: 2rem;
        }

        /* Grid de Criterios y Contenidos (Tarjetas limpias) */
        .grid-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            list-style: none;
            margin-top: 2rem;
        }
        .card-item {
            background: white;
            padding: 1.8rem;
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.04);
            border-left: 4px solid #7393C6;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.08);
            border-left-color: #050A30;
        }

        /* ---------------------------------------------------
           NUEVO TIMELINE (Vertical Moderno)
        ----------------------------------------------------- */
        .timeline-modern {
            position: relative;
            max-width: 900px;
            margin: 4rem auto;
            padding: 2rem 0;
        }
        /* Línea central */
        .timeline-modern::after {
            content: '';
            position: absolute;
            width: 4px;
            background-color: #e0e6ed;
            top: 0;
            bottom: 0;
            left: 50%;
            margin-left: -2px;
            border-radius: 2px;
        }

        .timeline-item {
            padding: 10px 40px;
            position: relative;
            background-color: inherit;
            width: 50%;
        }

        /* Nodos/Puntos */
        .timeline-item::after {
            content: '';
            position: absolute;
            width: 24px;
            height: 24px;
            right: -12px;
            background-color: white;
            border: 4px solid #5A77A6;
            top: 20px;
            border-radius: 50%;
            z-index: 1;
            transition: all 0.3s ease;
        }

        .left { left: 0; }
        .right { left: 50%; }

        .left::after {
            right: -12px;
        }
        .right::after {
            left: -12px;
        }

        .timeline-item:hover::after {
            background-color: #050A30;
            border-color: #7393C6;
            transform: scale(1.2);
        }

        .timeline-content {
            padding: 1.5rem;
            background-color: white;
            position: relative;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }
        
        .timeline-content:hover {
            transform: translateY(-3px);
        }

        .timeline-date {
            color: #7393C6;
            font-weight: 700;
            font-size: 1.1rem;
            margin-bottom: 0.5rem;
            display: block;
        }
        .timeline-desc {
            color: #2C3E50;
            font-size: 0.95rem;
            margin: 0;
        }

        /* Responsive Timeline */
        @media screen and (max-width: 768px) {
            .timeline-modern::after {
                left: 31px;
            }
            .timeline-item {
                width: 100%;
                padding-left: 70px;
                padding-right: 0px;
                margin-bottom: 1.5rem;
            }
            .timeline-item::after {
                left: 19px;
            }
            .right {
                left: 0%;
            }
        }

        /* Botón de Postulación Final */
        .postulate-btn {
            display: block;
            width: fit-content;
            margin: 4rem auto 1rem auto;
            background: #050A30;
            color: white;
            font-size: 1.3rem;
            font-weight: 600;
            padding: 1.2rem 3rem;
            border-radius: 50px;
            text-decoration: none;
            text-align: center;
            transition: all 0.3s ease;
            box-shadow: 0 10px 25px rgba(5, 10, 48, 0.2);
        }
        .postulate-btn:hover {
            background: #5A77A6;
            transform: translateY(-3px);
            box-shadow: 0 15px 35px rgba(5, 10, 48, 0.3);
        }

        /* Footer Modernizado */
        footer {
            background-color: #050A30;
            color: white;
            padding: 4rem 2rem 2rem 2rem;
            margin-top: 3rem;
            text-align: center;
        }
        
        .footer-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 3rem;
            max-width: 900px;
            margin: 0 auto 3rem auto;
        }

        .footer-block h4 {
            color: #7393C6;
            margin-bottom: 1rem;
            font-size: 1.2rem;
        }

        .footer-block p {
            opacity: 0.8;
            font-weight: 300;
        }

        .copyright {
            border-top: 1px solid rgba(255,255,255,0.1);
            padding-top: 2rem;
            font-size: 0.9rem;
            opacity: 0.6;
            font-weight: 300;
        }

        /* Animaciones */
        .fade-in {
            animation: fadeIn 1s ease forwards;
            opacity: 0;
            transform: translateY(20px);
        }

        @keyframes fadeIn {
            to { opacity: 1; transform: translateY(0); }
        }

        @media (min-width: 768px) {
            header {
                padding: 6rem 4rem 10rem 4rem;
            }
            .header-logos {
                position: absolute;
                top: 2rem;
                right: 3rem;
                margin-bottom: 0;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="header-logos fade-in" style="animation-delay: 0.1s;">
            <img src="logo-actio.png" alt="Actio">
            <img src="logo-botin.png" alt="Fundación Botín">
        </div>
        <h1 class="fade-in" style="animation-delay: 0.3s;">Activá<br>lo Público</h1>
        <p class="fade-in" style="animation-delay: 0.5s;">El programa para enamorar a las juventudes de lo público.</p>
        <a href="#fechas" class="btn-header fade-in" style="animation-delay: 0.7s;">#SeActiva</a>
        
        <!-- Curva Decorativa -->
        <div class="custom-shape-divider-bottom">
            <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
                <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
            </svg>
        </div>
    </header>

    <section>
        <!-- Misión destacada sobrepuesta -->
        <div class="mision-destacada fade-in" style="animation-delay: 0.9s;">
            <h3>Nuestra Misión</h3>
            <p>"Que más de las y los mejores se enamoren de lo público"</p>
        </div>

        <h2>¿Quiénes Somos?</h2>
        <div class="text-block">
            <p><strong>Actio</strong> es una asociación civil formada por personas comprometidas con la función pública en Argentina, fundada en 2020 por ex becarios del Programa para el Fortalecimiento de la Función Pública en América Latina de la Fundación Botín. Actualmente reúne a <span class="text-highlight">74 miembros</span>.</p>
            <br>
            <p>Nuestro principal aliado es la <strong>Fundación Botín</strong>, creada en 1964, que actúa en toda España y América Latina con la misión de contribuir al desarrollo integral de la sociedad.</p>
        </div>

        <h2>El Programa</h2>
        <div class="text-block">
            <p>Buscamos llegar a jóvenes de Argentina a través de una experiencia federal y latinoamericanista, con un componente vivencial y otro formativo, que contribuya a entender, involucrarse y defender el valor de lo público.</p>
        </div>
        
        <ul class="grid-cards">
            <li class="card-item">
                <strong class="text-highlight">Etapa Virtual</strong><br><br>
                Participan 50 jóvenes de todas las provincias argentinas. Incluye clases magistrales semanales, conversaciones, talleres de simulación y encuentros virtuales con referentes de Argentina y Latinoamérica.
            </li>
            <li class="card-item">
                <strong class="text-highlight">Etapa Presencial</strong><br><br>
                Se seleccionarán 25 participantes con base en su desempeño. Se realizará en Córdoba, en el camping de AGEC (Santa Ana).<br><br>
                <em>Ejes: Actividad vivencial, charlas con líderes y networking.</em>
            </li>
        </ul>

        <h2 style="margin-top: 4rem;">Criterios de Selección</h2>
        <p style="text-align: center; margin-bottom: 2rem;">El programa está dirigido a jóvenes de Argentina de 18 a 21 años que hayan finalizado el colegio secundario y estén cursando estudios universitarios o terciarios.</p>
        
        <ul class="grid-cards">
            <li class="card-item">Poseer nacionalidad argentina.</li>
            <li class="card-item">Haber nacido entre el 14 de Julio de 2004 y el 13 de Julio de 2008 inclusive.</li>
            <li class="card-item">Haber finalizado el secundario, ser estudiante de grado/terciario y no haber superado el 50% de la carrera.</li>
            <li class="card-item">Contar con buen expediente académico y compromiso social.</li>
            <li class="card-item">Vocación de servicio e interés por ser agente de cambio.</li>
        </ul>

        <!-- LÍNEA DE TIEMPO MODERNIZADA -->
        <h2 id="fechas" style="margin-top: 5rem;">Fechas Clave</h2>
        
        <div class="timeline-modern">
            <div class="timeline-item left">
                <div class="timeline-content">
                    <span class="timeline-date">27 de Abril</span>
                    <p class="timeline-desc">Lanzamiento y apertura de postulaciones.</p>
                </div>
            </div>
            
            <div class="timeline-item right">
                <div class="timeline-content">
                    <span class="timeline-date">29 de Mayo</span>
                    <p class="timeline-desc">Cierre del período de postulaciones.</p>
                </div>
            </div>
            
            <div class="timeline-item left">
                <div class="timeline-content">
                    <span class="timeline-date">Hasta el 24 de Junio</span>
                    <p class="timeline-desc">Período de evaluación de postulaciones.</p>
                </div>
            </div>
            
            <div class="timeline-item right">
                <div class="timeline-content">
                    <span class="timeline-date">Hasta el 1 de Julio</span>
                    <p class="timeline-desc">Etapa de entrevistas.</p>
                </div>
            </div>
            
            <div class="timeline-item left">
                <div class="timeline-content">
                    <span class="timeline-date">5 de Julio</span>
                    <p class="timeline-desc">Inicio de la etapa virtual.</p>
                </div>
            </div>
            
            <div class="timeline-item right">
                <div class="timeline-content">
                    <span class="timeline-date">22 de Julio</span>
                    <p class="timeline-desc">Anuncio de seleccionados y seleccionadas.</p>
                </div>
            </div>
            
            <div class="timeline-item left">
                <div class="timeline-content">
                    <span class="timeline-date">9 de Septiembre</span>
                    <p class="timeline-desc">Fin de la etapa virtual.</p>
                </div>
            </div>
            
            <div class="timeline-item right">
                <div class="timeline-content">
                    <span class="timeline-date">14 de Septiembre</span>
                    <p class="timeline-desc">Anuncio de seleccionados/as para la etapa presencial.</p>
                </div>
            </div>
            
            <div class="timeline-item left">
                <div class="timeline-content">
                    <span class="timeline-date">2, 3 y 4 de Octubre</span>
                    <p class="timeline-desc">Etapa presencial (Córdoba).</p>
                </div>
            </div>
        </div>

        <a href="https://docs.google.com/forms/d/e/1FAIpQLSc8UXKnP1Wgiz1MV9g4C8mYZVBhqbL7IvHLtiNJA6kRepQPYQ/viewform?usp=dialog" target="_blank" class="postulate-btn">Postulate Aquí</a>
    </section>

    <footer>
        <div class="footer-grid">
            <div class="footer-block">
                <h4>Contacto</h4>
                <p>redactioargentina@gmail.com</p>
            </div>
            <div class="footer-block">
                <h4>Redes Sociales</h4>
                <p>Instagram: @red.actio</p>
            </div>
        </div>
        <div class="copyright">
            <p>© 2026 Activá lo Público. Desarrollado por la Asociación Civil Actio.</p>
        </div>
    </footer>

</body>
</html>
