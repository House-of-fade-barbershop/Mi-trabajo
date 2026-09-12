<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>House Of Fade Barbershop</title>

    <meta name="description" content="House Of Fade Barbershop - Cortes, estilo y precisión.">

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Oswald:wght@400;500;600;700&family=Playfair+Display:wght@500;600;700&family=Montserrat:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    background: #080808;
    color: #fff;
    font-family: 'Montserrat', sans-serif;
    overflow-x: hidden;
}


/* ==============================
   HEADER
================================= */

header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;

    height: 82px;

    display: flex;
    align-items: center;
    justify-content: space-between;

    padding: 0 7%;

    z-index: 1000;

    background: rgba(8, 8, 8, 0.88);
    backdrop-filter: blur(15px);

    border-bottom: 1px solid rgba(255,255,255,0.08);
}


/* LOGO */

.logo {
    text-decoration: none;
    color: white;

    display: flex;
    flex-direction: column;

    line-height: 1;
}

.logo-top {
    font-family: 'Playfair Display', serif;

    font-size: 11px;

    letter-spacing: 4px;

    color: #c8a66a;

    margin-bottom: 4px;
}

.logo-main {
    font-family: 'Oswald', sans-serif;

    font-size: 24px;

    font-weight: 600;

    letter-spacing: 2px;
}

.logo-bottom {
    font-size: 7px;

    letter-spacing: 4px;

    color: #aaa;

    margin-top: 4px;
}


/* NAV */

nav {
    display: flex;
    gap: 32px;
}

nav a {
    text-decoration: none;

    color: #ddd;

    font-size: 12px;

    font-weight: 600;

    letter-spacing: 1px;

    transition: 0.3s;
}

nav a:hover {
    color: #c8a66a;
}


/* MENU */

.menu-btn {
    display: none;

    font-size: 25px;

    color: white;

    cursor: pointer;
}


/* ==============================
   HERO
================================= */

.hero {

    min-height: 100vh;

    position: relative;

    display: flex;

    align-items: center;

    overflow: hidden;

    padding: 130px 7% 80px;

    background:

        radial-gradient(
            circle at 75% 45%,
            rgba(200,166,106,0.14),
            transparent 30%
        ),

        linear-gradient(
            120deg,
            #050505 0%,
            #101010 55%,
            #070707 100%
        );
}


/* textura */

.hero::before {

    content: "";

    position: absolute;

    inset: 0;

    background-image:
        linear-gradient(
            rgba(255,255,255,0.025) 1px,
            transparent 1px
        ),
        linear-gradient(
            90deg,
            rgba(255,255,255,0.025) 1px,
            transparent 1px
        );

    background-size: 55px 55px;

    opacity: 0.25;
}


/* círculo decorativo */

.hero::after {

    content: "";

    position: absolute;

    width: 520px;
    height: 520px;

    right: -160px;
    top: 50%;

    transform: translateY(-50%);

    border: 1px solid rgba(200,166,106,0.15);

    border-radius: 50%;

    box-shadow:
        0 0 0 35px rgba(200,166,106,0.025),
        0 0 0 70px rgba(200,166,106,0.015);
}


/* CONTENIDO */

.hero-content {

    position: relative;

    z-index: 2;

    max-width: 760px;
}


/* pequeño título */

.eyebrow {

    display: flex;

    align-items: center;

    gap: 12px;

    margin-bottom: 24px;

    color: #c8a66a;

    font-size: 11px;

    font-weight: 700;

    letter-spacing: 4px;

    text-transform: uppercase;
}

.eyebrow::before {

    content: "";

    width: 35px;

    height: 1px;

    background: #c8a66a;
}


/* TITULO */

.hero h1 {

    font-family: 'Oswald', sans-serif;

    font-size: clamp(
        58px,
        10vw,
        115px
    );

    font-weight: 600;

    line-height: 0.9;

    letter-spacing: -2px;

    text-transform: uppercase;

    margin-bottom: 30px;
}

.hero h1 span {

    color: #c8a66a;

    display: block;
}


/* SUBTITULO */

.hero-text {

    max-width: 570px;

    color: #aaa;

    font-size: 15px;

    line-height: 1.8;

    margin-bottom: 35px;
}


/* ==============================
   BOTONES
================================= */

.hero-buttons {

    display: flex;

    gap: 14px;

    flex-wrap: wrap;
}


.btn {

    display: inline-flex;

    align-items: center;

    justify-content: center;

    min-width: 175px;

    padding: 16px 25px;

    text-decoration: none;

    font-size: 11px;

    font-weight: 700;

    letter-spacing: 1.5px;

    transition: 0.3s;

}


/* principal */

.btn-gold {

    background: #c8a66a;

    color: #080808;
}

.btn-gold:hover {

    transform: translateY(-3px);

    box-shadow:
        0 12px 30px
        rgba(200,166,106,0.18);
}


/* secundario */

.btn-outline {

    border: 1px solid rgba(255,255,255,0.2);

    color: white;
}

.btn-outline:hover {

    border-color: #c8a66a;

    color: #c8a66a;
}


/* ==============================
   EMBLEMA DECORATIVO
================================= */

.hero-badge {

    position: absolute;

    right: 12%;
    top: 50%;

    transform: translateY(-50%);

    width: 300px;
    height: 300px;

    border: 1px solid rgba(200,166,106,0.25);

    border-radius: 50%;

    display: flex;

    align-items: center;
    justify-content: center;

    z-index: 2;
}


.hero-badge::before {

    content: "";

    position: absolute;

    inset: 18px;

    border: 1px solid rgba(200,166,106,0.15);

    border-radius: 50%;
}


.badge-content {

    text-align: center;

    z-index: 2;
}


.badge-content .small {

    display: block;

    font-family: 'Playfair Display', serif;

    color: #c8a66a;

    font-size: 13px;

    letter-spacing: 3px;
}


.badge-content strong {

    display: block;

    font-family: 'Oswald', sans-serif;

    font-size: 38px;

    letter-spacing: 3px;

    margin: 5px 0;
}


.badge-content .line {

    width: 50px;

    height: 1px;

    background: #c8a66a;

    margin: 10px auto;
}


.badge-content small {

    font-size: 8px;

    letter-spacing: 3px;

    color: #999;
}


/* ==============================
   SCROLL
================================= */

.scroll {

    position: absolute;

    bottom: 28px;
    left: 7%;

    display: flex;

    align-items: center;

    gap: 12px;

    color: #777;

    font-size: 9px;

    letter-spacing: 3px;

    z-index: 3;
}

.scroll-line {

    width: 40px;

    height: 1px;

    background: #555;
}


/* ==============================
   RESPONSIVE
================================= */

@media (max-width: 850px) {

    header {
        height: 72px;
        padding: 0 6%;
    }

    nav {
        display: none;
    }

    .menu-btn {
        display: block;
    }

    .hero {

        padding:
            120px
            6%
            90px;
    }

    .hero h1 {

        font-size: 64px;

        letter-spacing: -1px;
    }

    .hero-badge {

        width: 210px;
        height: 210px;

        right: -70px;

        opacity: 0.35;
    }

    .badge-content strong {
        font-size: 28px;
    }

    .hero-text {
        font-size: 14px;
        max-width: 500px;
    }

    .hero-buttons {
        flex-direction: column;

        align-items: flex-start;
    }

    .btn {
        width: 100%;
        max-width: 250px;
    }

    .scroll {
        left: 6%;
    }
}


@media (max-width: 500px) {

    .logo-main {
        font-size: 20px;
    }

    .logo-top {
        font-size: 8px;
        letter-spacing: 3px;
    }

    .logo-bottom {
        font-size: 6px;
    }

    .hero h1 {
        font-size: 55px;
    }

    .hero-badge {
        right: -105px;
        opacity: 0.22;
    }

}

</style>
</head>


<body>


<!-- ==============================
     HEADER
================================= -->

<header>

    <a href="#inicio" class="logo">

        <span class="logo-top">
            HOUSE OF FADE
        </span>

        <span class="logo-main">
            BARBERSHOP
        </span>

        <span class="logo-bottom">
            EST. STYLE & PRECISION
        </span>

    </a>


    <nav>

        <a href="#inicio">
            INICIO
        </a>

        <a href="#servicios">
            SERVICIOS
        </a>

        <a href="#cortes">
            CORTES
        </a>

        <a href="#contacto">
            CONTACTO
        </a>

    </nav>


    <div class="menu-btn">
        ☰
    </div>

</header>



<!-- ==============================
     HERO
================================= -->

<section class="hero" id="inicio">


    <div class="hero-content">

        <div class="eyebrow">
            HOUSE OF FADE BARBERSHOP
        </div>


        <h1>

            TU ESTILO

            <span>
                TU FADE.
            </span>

        </h1>


        <p class="hero-text">

            Más que un corte. Una experiencia pensada
            para que salgas con un estilo que realmente
            vaya contigo.

        </p>


        <div class="hero-buttons">

            <a
                href="#servicios"
                class="btn btn-gold"
            >
                VER SERVICIOS
            </a>


            <a
                href="#contacto"
                class="btn btn-outline"
            >
                RESERVAR CITA
            </a>

        </div>

    </div>



    <!-- EMBLEMA -->

    <div class="hero-badge">

        <div class="badge-content">

            <span class="small">
                HOUSE OF
            </span>

            <strong>
                FADE
            </strong>

            <div class="line"></div>

            <small>
                BARBERSHOP
            </small>

        </div>

    </div>



    <!-- SCROLL -->

    <div class="scroll">

        <span class="scroll-line"></span>

        SCROLL

    </div>


</section>
<!-- ==============================
     SERVICIOS
================================= -->

<section class="services" id="servicios">

    <div class="section-title">

        <span>LO QUE HACEMOS</span>

        <h2>
            SERVICIOS
        </h2>

        <p>
            Precisión en cada detalle. Elige el servicio
            que mejor se adapte a tu estilo.
        </p>

    </div>


    <div class="services-grid">

        <div class="service-card">

            <div class="service-number">01</div>

            <h3>
                FADE
            </h3>

            <p>
                Degradado limpio y personalizado
                según tu estilo.
            </p>

            <strong>
                $___
            </strong>

        </div>


        <div class="service-card featured">

            <div class="service-number">02</div>

            <h3>
                CORTE + FADE
            </h3>

            <p>
                Corte completo con degradado
                y acabado profesional.
            </p>

            <strong>
                $___
            </strong>

        </div>


        <div class="service-card">

            <div class="service-number">03</div>

            <h3>
                BARBA
            </h3>

            <p>
                Perfilado y arreglo de barba
                con acabado preciso.
            </p>

            <strong>
                $___
            </strong>

        </div>


        <div class="service-card">

            <div class="service-number">04</div>

            <h3>
                CORTE + BARBA
            </h3>

            <p>
                El combo completo para renovar
                tu estilo.
            </p>

            <strong>
                $___
            </strong>

        </div>

    </div>

</section>



<!-- ==============================
     CORTES
================================= -->

<section class="cuts" id="cortes">

    <div class="section-title">

        <span>NUESTRO TRABAJO</span>

        <h2>
            CORTES
        </h2>

        <p>
            Algunos de nuestros estilos.
            Próximamente podrás ver aquí los trabajos
            realizados en House Of Fade.
        </p>

    </div>


    <div class="cuts-grid">

        <!-- FOTO 1 -->

        <div class="cut-card">

            <div class="cut-placeholder">

                <span>HOUSE OF FADE</span>

                <strong>
                    FADE
                </strong>

                <small>
                    PRÓXIMAMENTE
                </small>

            </div>

        </div>


        <!-- FOTO 2 -->

        <div class="cut-card">

            <div class="cut-placeholder">

                <span>HOUSE OF FADE</span>

                <strong>
                    STYLE
                </strong>

                <small>
                    PRÓXIMAMENTE
                </small>

            </div>

        </div>


        <!-- FOTO 3 -->

        <div class="cut-card">

            <div class="cut-placeholder">

                <span>HOUSE OF FADE</span>

                <strong>
                    PRECISION
                </strong>

                <small>
                    PRÓXIMAMENTE
                </small>

            </div>

        </div>

    </div>

</section>



<!-- ==============================
     EXPERIENCIA
================================= -->

<section class="experience">

    <div class="experience-content">

        <span>
            HOUSE OF FADE
        </span>

        <h2>
            NO ES SOLO<br>
            UN CORTE.
        </h2>

        <p>
            Es tu estilo, tu momento y la confianza
            de salir de la barbería sintiéndote bien
            con tu imagen.
        </p>

    </div>


    <div class="experience-stats">

        <div>
            <strong>01</strong>
            <span>ESTILO</span>
        </div>

        <div>
            <strong>02</strong>
            <span>PRECISIÓN</span>
        </div>

        <div>
            <strong>03</strong>
            <span>ACTITUD</span>
        </div>

    </div>

</section>



<!-- ==============================
     CONTACTO
================================= -->

<section class="contact" id="contacto">

    <div class="contact-box">

        <span>
            RESERVA TU CITA
        </span>

        <h2>
            ¿LISTO PARA<br>
            TU PRÓXIMO FADE?
        </h2>

        <p>
            Agenda tu cita y déjanos trabajar
            en tu próximo estilo.
        </p>


        <div class="contact-buttons">

            <!-- CAMBIA EL NÚMERO POR EL DE TU AMIGO -->

            <a
                href="https://wa.me/527121081755"
                target="_blank"
                class="btn btn-gold"
            >
                WHATSAPP
            </a>


            <a
                href="#inicio"
                class="btn btn-outline"
            >
                VOLVER ARRIBA
            </a>

        </div>

    </div>


    <div class="contact-info">

        <div>

            <span>
                UBICACIÓN
            </span>

            <p>
                Próximamente
            </p>

        </div>


        <div>

            <span>
                HORARIO
            </span>

            <p>
                Próximamente
            </p>

        </div>


        <div>

            <span>
                CONTACTO
            </span>

            <p>
                WhatsApp
            </p>

        </div>

    </div>

</section>



<!-- ==============================
     FOOTER
================================= -->

<footer>

    <div class="footer-logo">

        <span>
            HOUSE OF
        </span>

        <strong>
            FADE
        </strong>

        <small>
            BARBERSHOP
        </small>

    </div>


    <p>
        © 2026 House Of Fade Barbershop.
        Todos los derechos reservados.
    </p>


    <a href="#inicio">
        ↑
    </a>

</footer>



<!-- ==============================
     ESTILOS PARTE 2
================================= -->

<style>

/* ==============================
   GENERAL SECTIONS
================================= */

section:not(.hero) {
    padding: 100px 7%;
}

.section-title {
    max-width: 650px;
    margin-bottom: 55px;
}

.section-title > span {
    color: #c8a66a;
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 4px;
}

.section-title h2 {
    font-family: 'Oswald', sans-serif;
    font-size: 60px;
    margin: 12px 0 15px;
}

.section-title p {
    color: #888;
    font-size: 14px;
    line-height: 1.8;
}


/* ==============================
   SERVICIOS
================================= */

.services {
    background: #0b0b0b;
}

.services-grid {
    display: grid;

    grid-template-columns:
        repeat(4, 1fr);

    gap: 15px;
}

.service-card {
    position: relative;

    padding: 35px 28px;

    min-height: 280px;

    background: #111;

    border: 1px solid rgba(255,255,255,0.07);

    transition: 0.3s;
}

.service-card:hover {
    transform: translateY(-6px);

    border-color:
        rgba(200,166,106,0.5);
}

.service-card.featured {
    background:
        linear-gradient(
            145deg,
            #17130d,
            #101010
        );

    border-color:
        rgba(200,166,106,0.35);
}

.service-number {
    color: #c8a66a;

    font-family: 'Oswald', sans-serif;

    font-size: 13px;

    margin-bottom: 45px;
}

.service-card h3 {
    font-family: 'Oswald', sans-serif;

    font-size: 27px;

    letter-spacing: 1px;

    margin-bottom: 15px;
}

.service-card p {
    color: #888;

    font-size: 12px;

    line-height: 1.7;

    margin-bottom: 25px;
}

.service-card strong {
    color: #c8a66a;

    font-size: 18px;
}


/* ==============================
   CORTES
================================= */

.cuts {
    background: #080808;
}

.cuts-grid {
    display: grid;

    grid-template-columns:
        repeat(3, 1fr);

    gap: 18px;
}

.cut-card {
    height: 430px;

    overflow: hidden;

    background: #101010;
}

.cut-placeholder {
    height: 100%;

    display: flex;

    flex-direction: column;

    align-items: center;

    justify-content: center;

    text-align: center;

    position: relative;

    background:
        radial-gradient(
            circle,
            rgba(200,166,106,0.12),
            transparent 55%
        );

    border: 1px solid
        rgba(255,255,255,0.06);

    transition: 0.4s;
}

.cut-placeholder:hover {
    transform: scale(1.02);
}

.cut-placeholder span {
    font-size: 9px;

    letter-spacing: 4px;

    color: #c8a66a;

    margin-bottom: 12px;
}

.cut-placeholder strong {
    font-family: 'Oswald', sans-serif;

    font-size: 50px;

    letter-spacing: 3px;
}

.cut-placeholder small {
    margin-top: 15px;

    color: #555;

    font-size: 8px;

    letter-spacing: 3px;
}


/* ==============================
   EXPERIENCE
================================= */

.experience {

    display: grid;

    grid-template-columns:
        1.5fr 1fr;

    gap: 80px;

    background: #101010;
}

.experience-content > span {
    color: #c8a66a;

    font-size: 10px;

    font-weight: 700;

    letter-spacing: 4px;
}

.experience-content h2 {
    font-family: 'Oswald', sans-serif;

    font-size: clamp(
        55px,
        7vw,
        90px
    );

    line-height: 0.9;

    margin: 20px 0 25px;
}

.experience-content p {
    max-width: 500px;

    color: #888;

    line-height: 1.8;

    font-size: 14px;
}

.experience-stats {

    display: grid;

    grid-template-columns:
        repeat(3, 1fr);

    align-items: center;

    gap: 20px;
}

.experience-stats div {
    text-align: center;

    border-left:
        1px solid
        rgba(200,166,106,0.25);

    padding: 20px;
}

.experience-stats strong {
    display: block;

    color: #c8a66a;

    font-family: 'Oswald', sans-serif;

    font-size: 42px;
}

.experience-stats span {
    display: block;

    color: #777;

    font-size: 8px;

    letter-spacing: 2px;

    margin-top: 8px;
}


/* ==============================
   CONTACTO
================================= */

.contact {
    background: #080808;

    text-align: center;
}

.contact-box {
    max-width: 750px;

    margin: auto;
}

.contact-box > span {
    color: #c8a66a;

    font-size: 10px;

    letter-spacing: 4px;

    font-weight: 700;
}

.contact-box h2 {
    font-family: 'Oswald', sans-serif;

    font-size: clamp(
        50px,
        8vw,
        85px
    );

    line-height: 0.9;

    margin: 20px 0;
}

.contact-box p {
    color: #888;

    font-size: 14px;

    line-height: 1.7;

    margin-bottom: 30px;
}

.contact-buttons {
    display: flex;

    justify-content: center;

    gap: 12px;

    flex-wrap: wrap;
}

.contact-info {
    max-width: 900px;

    margin: 80px auto 0;

    padding-top: 35px;

    border-top:
        1px solid
        rgba(255,255,255,0.08);

    display: grid;

    grid-template-columns:
        repeat(3, 1fr);

    gap: 20px;
}

.contact-info span {
    color: #c8a66a;

    font-size: 9px;

    letter-spacing: 3px;

    font-weight: 700;
}

.contact-info p {
    color: #777;

    font-size: 12px;

    margin-top: 10px;
}


/* ==============================
   FOOTER
================================= */

footer {

    min-height: 150px;

    padding: 40px 7%;

    display: flex;

    align-items: center;

    justify-content: space-between;

    gap: 30px;

    background: #050505;

    border-top:
        1px solid
        rgba(255,255,255,0.06);
}

.footer-logo {
    display: flex;

    flex-direction: column;

    line-height: 1;
}

.footer-logo span {
    color: #c8a66a;

    font-family: 'Playfair Display', serif;

    font-size: 8px;

    letter-spacing: 3px;
}

.footer-logo strong {
    font-family: 'Oswald', sans-serif;

    font-size: 28px;

    letter-spacing: 2px;

    margin: 5px 0;
}

.footer-logo small {
    color: #555;

    font-size: 7px;

    letter-spacing: 3px;
}

footer p {
    color: #555;

    font-size: 10px;
}

footer > a {
    width: 38px;
    height: 38px;

    display: flex;

    align-items: center;
    justify-content: center;

    border: 1px solid
        rgba(255,255,255,0.15);

    color: white;

    text-decoration: none;

    transition: 0.3s;
}

footer > a:hover {
    border-color: #c8a66a;

    color: #c8a66a;
}


/* ==============================
   MOBILE
================================= */

@media (max-width: 900px) {

    .services-grid {
        grid-template-columns:
            repeat(2, 1fr);
    }

    .cuts-grid {
        grid-template-columns:
            repeat(2, 1fr);
    }

    .experience {
        grid-template-columns: 1fr;

        gap: 50px;
    }

}


@media (max-width: 600px) {

    section:not(.hero) {
        padding: 75px 6%;
    }

    .section-title h2 {
        font-size: 50px;
    }

    .services-grid {
        grid-template-columns: 1fr;
    }

    .service-card {
        min-height: 240px;
    }

    .cuts-grid {
        grid-template-columns: 1fr;
    }

    .cut-card {
        height: 360px;
    }

    .experience-stats {
        grid-template-columns:
            repeat(3, 1fr);

        gap: 5px;
    }

    .experience-stats strong {
        font-size: 30px;
    }

    .experience-stats span {
        font-size: 7px;
    }

    .contact-info {
        grid-template-columns: 1fr;

        gap: 30px;
    }

    footer {
        flex-direction: column;

        text-align: center;
    }

}

</style>


<!-- ==============================
     JAVASCRIPT
================================= -->

<script>

const menuButton =
    document.querySelector('.menu-btn');

const nav =
    document.querySelector('nav');


menuButton.addEventListener(
    'click',
    () => {

        if (
            nav.style.display === 'flex'
        ) {

            nav.style.display = 'none';

        } else {

            nav.style.display = 'flex';

            nav.style.flexDirection =
                'column';

            nav.style.position =
                'absolute';

            nav.style.top =
                '72px';

            nav.style.right =
                '6%';

            nav.style.padding =
                '20px';

            nav.style.background =
                '#101010';

            nav.style.border =
                '1px solid rgba(255,255,255,0.1)';

        }

    }
);


/* cerrar menú al seleccionar */

document.querySelectorAll('nav a')
.forEach(link => {

    link.addEventListener(
        'click',
        () => {

            if (
                window.innerWidth <= 850
            ) {

                nav.style.display =
                    'none';

            }

        }
    );

});


</script>


</body>
</html>
