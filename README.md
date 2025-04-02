<!DOCTYPE html>
<html lang="ru">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Анастасия Сатина</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link
        href="https://fonts.googleapis.com/css2?family=Rubik:wght@500;600&family=Plus+Jakarta+Sans:wght@400;500;600&display=swap"
        rel="stylesheet">
    <style>
        :root {
            --primary: #026670;
            --primary-light: #026670;
            --text: #374151;
            --text-light: #374151;
            --bg: #f9fafb;
            --card: #ffffff;
            --border: #e5e7eb;
            --skill-bg: #fcf2e289;

            --font-heading: 'Rubik', sans-serif;
            --font-main: 'Plus Jakarta Sans', sans-serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: var(--font-main);
            line-height: 1.6;
            color: var(--text);
            background-color: var(--bg);
        }

        .container {
            max-width: 800px;
            margin: 2rem auto;
            padding: 2.5rem;
            background: var(--card);
            border-radius: 16px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
            border: 1px solid var(--border);
        }

        header {
            text-align: center;
            margin-bottom: 2.5rem;
        }

        h1 {
            font-family: var(--font-heading);
            font-size: 2.25rem;
            font-weight: 600;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .subtitle {
            font-size: 1.1rem;
            color: var(--text-light);
            margin-bottom: 1.5rem;
            font-weight: 500;
        }

        h2 {
            font-family: var(--font-heading);
            font-size: 1.6rem;
            font-weight: 600;
            color: var(--primary);
            margin: 2.5rem 0 1.25rem;
            position: relative;
        }

        h2::after {
            content: '';
            position: absolute;
            bottom: -8px;
            left: 0;
            width: 50px;
            height: 3px;
            background: var(--primary-light);
            border-radius: 3px;
        }

        p {
            margin-bottom: 1.25rem;
            color: var(--text);
            font-size: 1.05rem;
            line-height: 1.7;
        }

        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 0.75rem;
            margin: 1.75rem 0;
        }

        .skill {
            background: var(--skill-bg);
            color: var(--primary);
            padding: 0.6rem 1.1rem;
            border-radius: 20px;
            font-size: 0.95rem;
            font-weight: 500;
            border: 1px solid var(--primary-light);
        }

        .contact-list {
            list-style: none;
            margin-top: 1.5rem;
        }

        .contact-list li {
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
        }

        .contact-list a {
            color: var(--primary);
            text-decoration: none;
            transition: all 0.2s ease;
            margin-left: 0.75rem;
            font-weight: 500;
        }

        .contact-list a:hover {
            color: var(--primary-light);
            text-decoration: underline;
        }

        .icon {
            width: 22px;
            height: 22px;
            fill: var(--primary);
            transition: fill 0.2s ease;
        }

        .telegram-icon {
            width: 22px;
            height: 22px;
            background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath fill='%23026670' d='M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm4.64 6.8c-.25 1.58-1.32 5.41-1.87 7.19-.19.6-.57.75-.93.71-.47-.05-.74-.31-1.15-.61-.64-.45-1-.73-1.62-1.17-.54-.38-.2-.58.13-.91.12-.12 2.38-2.19 2.42-2.37.01-.05.01-.23-.09-.33-.09-.09-.23-.06-.33-.03-.14.04-2.39 1.52-3.05 1.92-.29.17-.55.25-.79.25-.26 0-.38-.09-.38-.25v-.23c.03-.43.93-4.48 1.3-5.96.14-.54.28-.73.92-.73.23 0 .46.01.68.01.26.03.29.12.26.4-.05.57-1.14 5.72-1.4 6.69-.17.63-.34.85-.63.85-.18 0-.45-.09-.81-.32-.45-.29-1.02-.65-1.89-1.23-1.48-1.01-2.01-1.66-2.87-2.36-.23-.19-.01-.29.18-.3.23-.02.75-.02 1.22-.02.46 0 .61.09.78.38.86 1.43 1.91 3.04 2.26 3.04.2 0 .29-.09.29-.56v-2.66c-.01-.96-.53-1.03-.53-1.03-.2-.05-.57-.11-.92-.16-.47-.06-.94-.13-1.3-.26-.35-.13-.63-.3-.7-.47-.06-.16.04-.24.28-.35.85-.38 2.7-.64 4.12-.66 1.42-.02 2.59.14 3.34.38.45.14.8.33.88.52.09.19.06.29-.01.4z'/%3E%3C/svg%3E") no-repeat center;
            transition: all 0.2s ease;
        }

        .contact-list li:hover .telegram-icon {
            background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'%3E%3Cpath fill='%23026670' d='M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm4.64 6.8c-.25 1.58-1.32 5.41-1.87 7.19-.19.6-.57.75-.93.71-.47-.05-.74-.31-1.15-.61-.64-.45-1-.73-1.62-1.17-.54-.38-.2-.58.13-.91.12-.12 2.38-2.19 2.42-2.37.01-.05.01-.23-.09-.33-.09-.09-.23-.06-.33-.03-.14.04-2.39 1.52-3.05 1.92-.29.17-.55.25-.79.25-.26 0-.38-.09-.38-.25v-.23c.03-.43.93-4.48 1.3-5.96.14-.54.28-.73.92-.73.23 0 .46.01.68.01.26.03.29.12.26.4-.05.57-1.14 5.72-1.4 6.69-.17.63-.34.85-.63.85-.18 0-.45-.09-.81-.32-.45-.29-1.02-.65-1.89-1.23-1.48-1.01-2.01-1.66-2.87-2.36-.23-.19-.01-.29.18-.3.23-.02.75-.02 1.22-.02.46 0 .61.09.78.38.86 1.43 1.91 3.04 2.26 3.04.2 0 .29-.09.29-.56v-2.66c-.01-.96-.53-1.03-.53-1.03-.2-.05-.57-.11-.92-.16-.47-.06-.94-.13-1.3-.26-.35-.13-.63-.3-.7-.47-.06-.16.04-.24.28-.35.85-.38 2.7-.64 4.12-.66 1.42-.02 2.59.14 3.34.38.45.14.8.33.88.52.09.19.06.29-.01.4z'/%3E%3C/svg%3E") no-repeat center;
            opacity: 0.8;
        }

        @media (max-width: 768px) {
            .container {
                margin: 1rem;
                padding: 1.75rem;
                border-radius: 12px;
            }

            h1 {
                font-size: 2rem;
            }

            h2 {
                font-size: 1.4rem;
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <header>
            <h1>Анастасия Сатина</h1>
            <p class="subtitle">Студент 4-го курса НИЯУ МИФИ</p>
        </header>

        <section>
            <h2>Обо мне</h2>
            <p>
                Занимаюсь программированием с фокусом на backend-разработку и анализ данных.
                Имею опыт работы с C++, Python и SQL. В свободное время занимаюсь разработкой системы умного дома на
                основе голосового помощника "Алиса" с поддержкой протокола ZigBee.
            </p>
        </section>

        <section>
            <h2>Навыки</h2>
            <div class="skills-container">
                <span class="skill">C++</span>
                <span class="skill">STL</span>
                <span class="skill">Алгоритмы</span>
                <span class="skill">Qt</span>
                <span class="skill">ООП</span>
                <span class="skill">Python</span>
                <span class="skill">SQL</span>
                <span class="skill">Git</span>
                <span class="skill">Docker</span>
                <span class="skill">Linux</span>
            </div>
        </section>

        <section>
            <h2>Образование</h2>
            <p><strong>Национальный Исследовательский Ядерный Университет "МИФИ"</strong></p>
            <p>Бакалавриат по специальности "Биотехнические системы и технологии"</p>
            <p>2021 — 2025</p>
        </section>

        <section>
            <h2>Контакты</h2>
            <ul class="contact-list">
                <li>
                    <svg class="icon" viewBox="0 0 24 24">
                        <path
                            d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12" />
                    </svg>
                    <a href="https://github.com/nastyaskysat" target="_blank">github.com/nastyaskysat</a>
                </li>
                <li>
                    <svg class="icon" viewBox="0 0 24 24">
                        <path
                            d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z" />
                    </svg>
                    <a href="mailto:nastyaskysat@mail.ru">nastyaskysat@mail.ru</a>
                </li>
                <li>
                    <div class="telegram-icon"></div>
                    <a href="https://t.me/nssttn" target="_blank">t.me/nssttn</a>
                </li>
            </ul>
        </section>
    </div>
</body>

</html>
