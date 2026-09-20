<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Александр Максимов | Портфолио</title>

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
            background: #000;
            color: #fff;
            font-family: Arial, sans-serif;
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        /* HEADER */

        header {
            min-height: 100vh;
            display: flex;
            align-items: center;
            border-bottom: 1px solid #222;
        }

        .container {
            width: 90%;
            max-width: 1150px;
            margin: auto;
        }

        .header-content {
            padding: 100px 0;
        }

        .small-title {
            color: #777;
            text-transform: uppercase;
            letter-spacing: 4px;
            font-size: 13px;
            margin-bottom: 25px;
        }

        h1 {
            font-size: clamp(50px, 9vw, 110px);
            line-height: .95;
            letter-spacing: -5px;
            margin-bottom: 30px;
        }

        .header-description {
            max-width: 700px;
            color: #999;
            font-size: 20px;
        }

        /* NAV */

        nav {
            position: sticky;
            top: 0;
            z-index: 100;
            background: rgba(0, 0, 0, .95);
            border-bottom: 1px solid #222;
        }

        .nav-container {
            min-height: 70px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-weight: bold;
            font-size: 20px;
        }

        .menu {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        .menu a {
            color: #888;
            font-size: 14px;
            transition: .2s;
        }

        .menu a:hover {
            color: white;
        }

        /* SECTIONS */

        section {
            padding: 100px 0;
            border-bottom: 1px solid #222;
        }

        .section-number {
            color: #555;
            font-size: 13px;
            letter-spacing: 3px;
            margin-bottom: 10px;
        }

        .section-title {
            font-size: 45px;
            margin-bottom: 45px;
        }

        /* ABOUT */

        .about {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 70px;
        }

        .about p {
            color: #aaa;
            font-size: 18px;
            margin-bottom: 20px;
        }

        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .skill {
            padding: 9px 14px;
            border: 1px solid #333;
            border-radius: 8px;
            color: #bbb;
        }

        /* PROJECTS */

        .projects {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }

        .project {
            padding: 30px;
            min-height: 240px;
            background: #090909;
            border: 1px solid #252525;
            border-radius: 15px;
            transition: .25s;
        }

        .project:hover {
            transform: translateY(-5px);
            border-color: #555;
        }

        .project h3 {
            font-size: 25px;
            margin-bottom: 15px;
        }

        .project p {
            color: #999;
            line-height: 1.7;
        }

        .project-tags {
            margin-top: 25px;
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .tag {
            border: 1px solid #333;
            border-radius: 6px;
            padding: 5px 9px;
            font-size: 12px;
            color: #aaa;
        }

        /* COURSES */

        .courses {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }

        .course {
            padding: 30px;
            border: 1px solid #252525;
            background: #090909;
            border-radius: 15px;
        }

        .course h3 {
            font-size: 24px;
            margin-bottom: 15px;
        }

        .course p {
            color: #999;
        }

        /* CERTIFICATES */

        .certificates {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }

        .certificate {
            padding: 25px;
            border: 1px solid #252525;
            border-radius: 15px;
            background: #090909;
        }

        .certificate h3 {
            margin-bottom: 15px;
            font-size: 22px;
        }

        .certificate p {
            color: #999;
            margin-bottom: 15px;
            line-height: 1.6;
        }

        .certificate p strong {
            color: #ddd;
        }

        /* NOTES */

        .notes {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .note {
            padding: 30px;
            border: 1px solid #252525;
            background: #090909;
            border-radius: 15px;
        }

        .note h3 {
            font-size: 25px;
            margin-bottom: 15px;
        }

        .note p {
            color: #999;
            margin-bottom: 20px;
        }

        .button {
            display: inline-block;
            border: 1px solid #555;
            padding: 10px 15px;
            border-radius: 8px;
            transition: .2s;
            margin-top: 5px;
        }

        .button:hover {
            background: white;
            color: black;
        }

        /* FOOTER */

        footer {
            padding: 40px 0;
            color: #555;
        }

        /* MOBILE */

        @media (max-width: 800px) {

            .nav-container {
                flex-direction: column;
                padding: 15px 0;
                gap: 15px;
            }

            .menu {
                gap: 12px;
                flex-wrap: wrap;
                justify-content: center;
            }

            .menu a {
                font-size: 12px;
            }

            .about {
                grid-template-columns: 1fr;
            }

            .projects {
                grid-template-columns: 1fr;
            }

            .courses {
                grid-template-columns: 1fr;
            }

            .certificates {
                grid-template-columns: 1fr;
            }

            section {
                padding: 70px 0;
            }

            .section-title {
                font-size: 36px;
            }
        }
    </style>
</head>

<body>

<!-- ================= NAVIGATION ================= -->

<nav>
    <div class="container nav-container">

        <div class="logo">
            АМ
        </div>

        <ul class="menu">

            <li>
                <a href="#about">Обо мне</a>
            </li>

            <li>
                <a href="#projects">Проекты</a>
            </li>

            <li>
                <a href="#courses">Курсы</a>
            </li>

            <li>
                <a href="#certificates">Сертификаты</a>
            </li>

            <li>
                <a href="#notes">Конспекты</a>
            </li>

        </ul>

    </div>
</nav>

<!-- ================= MAIN ================= -->

<header>

    <div class="container">

        <div class="header-content">

            <div class="small-title">
                Личное портфолио
            </div>

            <h1>
                Александр

                Максимов
            </h1>

            <p class="header-description">
                Студент 3 курса Люберецкого техникума
                имени Гагарина. Изучаю программирование,
                информационные технологии и разработку
                сайтов.
            </p>

        </div>

    </div>

</header>

<!-- ================= ABOUT ================= -->

<section id="about">

    <div class="container">

        <div class="section-number">
            01 — ABOUT
        </div>

        <h2 class="section-title">
            Обо мне
        </h2>

        <div class="about">

            <div>

                <p>
                    Я студент <strong>
                    3 курса Люберецкого техникума
                    имени Гагарина
                    </strong>.
                </p>

                <p>
                    Изучаю программирование,
                    веб-разработку и современные
                    информационные технологии.
                </p>

                <p>
                    В данном портфолио представлены
                    мои учебные проекты, курсы,
                    сертификаты и конспекты.
                </p>

            </div>

            <div>

                <h3 style="margin-bottom:20px;">
                    Навыки
                </h3>

                <div class="skills">

                    <span class="skill">HTML</span>
                    <span class="skill">CSS</span>
                    <span class="skill">JavaScript</span>
                    <span class="skill">Python</span>
                    <span class="skill">SQL</span>
                    <span class="skill">Git</span>
                    <span class="skill">Linux</span>
                    <span class="skill">Web</span>

                </div>

            </div>

        </div>

    </div>

</section>

<!-- ================= PROJECTS ================= -->

<section id="projects">

    <div class="container">

        <div class="section-number">
            02 — PROJECTS
        </div>

        <h2 class="section-title">
            Мои проекты
        </h2>

        <div class="projects">

            <div class="project">

                <h3>
                    Курсовая работа
                </h3>

                <p>
                    Моя курсовая работа, выполненная
                    в рамках обучения в Люберецком
                    техникуме имени Гагарина.
                </p>

                <p>
                    Здесь будет размещено подробное
                    описание проекта, его цель,
                    задачи и используемые технологии.
                </p>

                <div class="project-tags">

                    <span class="tag">
                        Курсовая
                    </span>

                    <span class="tag">
                        Учебный проект
                    </span>

                </div>

            </div>

            <div class="project">

                <h3>
                    Инструкция по созданию сайтов
                </h3>

                <p>
                    Учебная инструкция, посвящённая
                    созданию сайтов с нуля.
                </p>

                <p>
                    В ней рассматриваются HTML,
                    CSS, структура страницы,
                    оформление элементов и
                    основные принципы веб-разработки.
                </p>

                <div class="project-tags">

                    <span class="tag">
                        HTML
                    </span>

                    <span class="tag">
                        CSS
                    </span>

                    <span class="tag">
                        Web
                    </span>

                </div>

            </div>

        </div>

    </div>

</section>

<!-- ================= COURSES ================= -->

<section id="courses">

    <div class="container">

        <div class="section-number">
            03 — COURSES
        </div>

        <h2 class="section-title">
            Курсы
        </h2>

        <div class="courses">

            <div class="course">

                <h3>
                    VK Образование
                </h3>

                <p>
                    Образовательные программы
                    и материалы VK.
                </p>

            </div>

            <div class="course">

                <h3>
                    Сбер Университет
                </h3>

                <p>
                    Образовательные программы
                    и курсы Сбера.
                </p>

            </div>

        </div>

    </div>

</section>

<!-- ================= CERTIFICATES ================= -->

<section id="certificates">

    <div class="container">

        <div class="section-number">
            04 — CERTIFICATES
        </div>

        <h2 class="section-title">
            Сертификаты
        </h2>

        <div class="certificates">

            <div class="certificate">

                <h3>
                    Сертификат VK Education
                </h3>

                <p>
                    Об успешном прохождении образовательной
                    программы «Новые медиа: SMM и digital-маркетинг»
                    от VK Education.
                </p>

                <p>
                    Получено <strong>30 из 37 баллов</strong>,
                    20 академических часов, 30 занятий.
                </p>

                <a
                    class="button"
                    href="images/vk-certificate.jpg"
                    target="_blank"
                >
                    Посмотреть сертификат →
                </a>

            </div>

            <div class="certificate">

                <h3>
                    Сертификат Сбер Университета
                </h3>

                <p>
                    Подтверждает участие в электронном курсе
                    «Работа с LLM GigaChat» в АНО ДПО
                    «Корпоративный университет Сбербанка».
                </p>

                <p>
                    Период обучения: с 6 по 6 ноября 2025 г.
                </p>

                <a
                    class="button"
                    href="images/sber-certificate.jpg"
                    target="_blank"
                >
                    Посмотреть сертификат →
                </a>

            </div>

        </div>

    </div>

</section>

<!-- ================= NOTES ================= -->

<section id="notes">

    <div class="container">

        <div class="section-number">
            05 — NOTES
        </div>

        <h2 class="section-title">
            Конспекты
        </h2>

        <div class="notes">

            <!-- БЕРЕЖЛИВОЕ ПРОИЗВОДСТВО -->

            <div class="note">

                <h3>
                    Основы бережливого производства
                </h3>

                <p>
                    Конспект по основам бережливого
                    производства. Включает основные
                    понятия, принципы бережливого
                    подхода, виды потерь и способы
                    повышения эффективности процессов.
                </p>

            </div>

            <!-- GOOGLE DOCS -->

            <div class="note">

                <h3>
                    Конспект Google Документы
                </h3>

                <p>
                    Учебный материал, размещённый
                    в Google Документах.
                </p>

                <a
                    class="button"
                    href="https://docs.google.com/document/d/1q3782K7LHkS_HTzgI3f-DnR59fNaVXq-FYq6_izazh0/edit?tab=t.0#heading=h.467w74uc5cy7"
                    target="_blank"
                >
                    Открыть конспект →
                </a>

            </div>

            <!-- GOOGLE COLAB -->

            <div class="note">

                <h3>
                    Конспект Google Colab
                </h3>

                <p>
                    Конспект по работе с Google Colab,
                    Python и интерактивными ноутбуками.
                </p>

                <a
                    class="button"
                    href="https://colab.research.google.com/drive/1DjDBNZLRoRo4367skNmWN-1mjgNtX6F7#scrollTo=sF1NfM5HJ95I"
                    target="_blank"
                >
                    Открыть Google Colab →
                </a>

            </div>

        </div>

    </div>

</section>

<!-- ================= FOOTER ================= -->

<footer>

    <div class="container">

        © 2026 Александр Максимов

    </div>

</footer>

</body>
</html>
