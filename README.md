# mylittlehouse
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>7-ой Корпус ВятГУ</title>
    <link rel="stylesheet" href="style_main.css">
    <link href="https://fonts.googleapis.com/css2?family=Tangerine:wght@700&family=Kalam&display=swap" rel="stylesheet">
    <style>
        .ad-container {
            position: fixed;
            right: 20px;
            bottom: 20px;
            width: 300px;
            background-color: #FF9933;
            border: 3px solid #138808;
            border-radius: 10px;
            padding: 10px;
            z-index: 1000;
            box-shadow: 0 0 15px #FF9933;
        }

        .ad-close {
            position: absolute;
            top: 5px;
            right: 5px;
            cursor: pointer;
            font-size: 20px;
            color: #FF0000;
        }

        .ad-content {
            text-align: center;
        }

            .ad-content img {
                max-width: 100%;
                border-radius: 5px;
            }

        .mobile-ad {
            display: none;
        }

        @media (max-width: 768px) {
            .ad-container {
                display: none;
            }

            .mobile-ad {
                display: block;
                position: fixed;
                bottom: 0;
                left: 0;
                width: 100%;
                background-color: #FF9933;
                border-top: 3px solid #138808;
                padding: 10px;
                z-index: 1000;
                text-align: center;
            }

            .mobile-ad-close {
                position: absolute;
                top: 5px;
                right: 15px;
                cursor: pointer;
                font-size: 20px;
                color: #FF0000;
            }
        }
    </style>
</head>
<body>
    <!-- Блок рекламы для десктопов -->
    <div class="ad-container">
        <span class="ad-close" onclick="this.parentElement.style.display='none'">✖</span>
        <div class="ad-content">
            <h3>Специальное предложение!</h3>
            <img src="https://via.placeholder.com/280x150/FF9933/FFFFFF?text=Реклама+чая" alt="Реклама">
            <p>Лучший Йога-Мастер со скидкой 50%!</p>
            <a href="https://vk.com/znahar_vyatka" target="_blank" style="color: #138808; font-weight: bold;">Купить сейчас</a>
        </div>
        <div class="крестик"><i class="fas fa-times"></i></div>
    </div>

    <!-- Блок рекламы для мобильных -->
    <div class="mobile-ad">
        <span class="mobile-ad-close" onclick="this.parentElement.style.display='none'">✖</span>
        <div>
            <h4>Попробуйте наш чай!</h4>
            <a href="https://greenfieldtea.co.uk/" target="_blank" style="color: #138808; font-weight: bold;">Узнать больше</a>
        </div>
    </div>
    <header>
        <div class="header-overlay">
            <h1>7-ой Корпус Вятского Государственного Университета</h1>
            <p>Добро пожаловать в царство знаний и великих традиций</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#" class="active">Главная</a></li>
            <li><a href="#about">О корпусе</a></li>
            <li><a href="#departments">Кафедры</a></li>
            <li><a href="#gallery">Галерея</a></li>
            <li><a href="test.html">Тест о чае</a></li>
        </ul>
    </nav>

    <main>
        <section id="about" class="section-with-bg">
            <div class="container">
                <h2>О 7-м корпусе</h2>
                <div class="content-box">
                    <img src="Корпус.jpg">
                    <p>7-й корпус Вятского Государственного Университета - это уникальное место, где сочетаются передовые технологии и древние индийские традиции обучения. Здесь студенты не только осваивают современные инженерные дисциплины, но и учатся гармонии с миром через философию йоги и чайные церемонии.</p>

                    <div class="video-container">
                        <iframe width="256" height="144" src="Э.mp4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>

                    <p>По мнению большинства учащихся этот корпус - самый душевный и атмосферный из всех остальных, а в аудиториях царит атмосфера, способствующая глубокому погружению в учебу и медитацию.</p>
                </div>
            </div>
        </section>

        <section id="departments">
            <div class="container">
                <h2>Наши кафедры</h2>

                <div class="grid-container">
                    <div class="grid-item">
                        <h3>Кафедра Электропривода</h3>
                        <p>Изучаем энергию так же, как индийские мудрецы изучали прану. Наши выпускники управляют электроприводами с грацией йогов.</p>
                    </div>

                    <div class="grid-item">
                        <h3>Кафедра Мехатроники и робототехники</h3>
                        <p>Создаем роботов, которые могут не только выполнять сложные задачи, но и медитировать на рассвете.</p>
                    </div>

                    <div class="grid-item">
                        <h3>Чайная лаборатория</h3>
                        <p>Уникальное место, где изучают влияние различных сортов чая на процесс обучения и программирования.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="gallery" class="section-with-bg">
            <div class="container">
                <h2>Галерея</h2>

                <div class="image-gallery">
                    <div class="gallery-item">
                        <img src="Ш.jpg" alt="Лекция">
                        <p>Студенты на лекции по электроприводу в традиционных одеждах</p>
                    </div>

                    <div class="gallery-item">
                        <img src="https://media1.tenor.com/m/QHOI_CYtGPQAAAAd/sa.gif" alt="Робот делает чай">
                        <p>Робот-бариста, созданный на кафедре мехатроники, готовит традиционный масала-чай</p>
                    </div>

                    <div class="gallery-item">
                        <img src="https://media.tenor.com/8BqdYZvekw4AAAAM/florp.gif" alt="Медитация">
                        <p>Ежедневная утренняя зарядка студентов перед занятиями</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="tea-culture">
            <div class="container">
                <h2>Чайные традиции корпуса</h2>
                <div class="content-box">
                    <p>В 7-м корпусе особое внимание уделяется чайным традициям, которые помогают студентам сохранять ясность ума во время учебы.</p>

                    <div class="tea-types">
                        <div class="tea-type">
                            <h3>Утренний чай</h3>
                            <p>Зеленый чай с жасмином для бодрости и концентрации</p>
                        </div>

                        <div class="tea-type">
                            <h3>Обеденный чай</h3>
                            <p>Крепкий ассамский чай с молоком и специями</p>
                        </div>

                        <div class="tea-type">
                            <h3>Вечерний чай</h3>
                            <p>Ромашковый чай с медом для расслабления</p>
                        </div>
                    </div>

                    <p>Проверьте свои знания о чае в нашем <a href="test.html" class="test-button">специальном тесте</a>!</p>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>© 2025 7-ой Корпус ВятГУ</p>
            <p>Все права на собственность и чай защищены</p>
        </div>
    </footer>
    <script>
        const randomAd = ads[Math.floor(Math.random() * ads.length)];
        const adContainer = document.querySelector('.ad-content');

        adContainer.innerHTML = `
                <h3>${randomAd.title}</h3>
                <img src="МАКС1.jpg" alt="Реклама">
                <p>${randomAd.text}</p>
                <a href="${randomAd.link}" target="_blank" style="color: #138808; font-weight: bold;">Узнать больше</a>
            `;
        // Показываем рекламу, если она была скрыта
        document.querySelector('.ad-container').style.display = 'block';
        // Первая загрузка рекламы
        window.onload = showRandomAd
    </script>
</body >
</html >
