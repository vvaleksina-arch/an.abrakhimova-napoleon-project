<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Наполеон Бонапарт: путь к империи</title>
    <style>
    :root {
        --bg: #f9f7f4;
        --primary: #2c2c2c;
        --accent: #d4af37;
        --card: #ffffff;
    }

    html {
        scroll-behavior: smooth;
    }

    .battle-link {
        color: var(--accent);
        text-decoration: none;
        font-weight: bold;
    }

    .battle-link:hover {
        color: #fff;
        background-color: var(--primary);
        padding: 2px 4px;
        border-radius: 3px;
    }

        body {
            font-family: 'Garamond', Georgia, serif;
            background-color: var(--bg);
            color: #222;
            line-height: 1.7;
            margin: 0;
            padding: 0;
        }

        header {
            background: var(--primary);
            color: white;
            padding: 2.5rem 1rem;
            text-align: center;
            border-bottom: 6px solid var(--accent);
        }

        h1 { margin: 0; letter-spacing: 1px; }

        nav { margin-top: 1.2rem; }
        nav a {
            color: var(--accent);
            text-decoration: none;
            margin: 0 14px;
            font-weight: bold;
            font-size: 1.1rem;
        }
        nav a:hover { color: #fff; text-decoration: underline; }

        main {
            max-width: 960px;
            margin: 2rem auto;
            padding: 0 1rem;
        }

        .card {
            background: var(--card);
            padding: 2rem;
            border-radius: 4px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.12);
            border: 1px solid #e0ddd5;
        }

        h2 {
            color: var(--primary);
            border-left: 5px solid var(--accent);
            padding-left: 12px;
            margin-top: 0;
        }

        p { margin-bottom: 1rem; }

           .carousel-container {
            position: relative;
            width: 100%;
            max-width: 800px;
            height: 450px; 
            margin: 20px auto;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
            background-color: #f0f0f0;
        }

        .carousel-track {
            display: flex;
            width: 100%;
            height: 100%;
            transition: transform 0.5s cubic-bezier(0.25, 1, 0.5, 1);
        }

        .carousel-slide {
            min-width: 100%;
            height: 100%;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }

        .carousel-slide img {
            width: 100%;
            height: 100%;
            object-fit: contain;
            display: block;
        }

        .carousel-caption {
            position: absolute;
            bottom: 20px;
            left: 20px;
            right: 20px;
            background: rgba(0, 0, 0, 0.6);
            color: white;
            padding: 8px 12px;
            border-radius: 4px;
            font-size: 0.9rem;
        }

        .carousel-btn {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background: rgba(0, 0, 0, 0.5);
            color: white;
            border: none;
            padding: 15px;
            cursor: pointer;
            z-index: 10;
            font-size: 24px;
        }
        .prev { left: 10px; }
        .next { right: 10px; }
        .carousel-btn:hover { background: rgba(0, 0, 0, 0.8); }

        .carousel-indicators {
            position: absolute;
            bottom: 15px;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 10px;
            z-index: 10;
        }

        .dot {
            width: 12px;
            height: 12px;
            background: rgba(255, 255, 255, 0.5);
            border-radius: 50%;
            cursor: pointer;
        }
        .dot.active {
            background: #d4af37;
            transform: scale(1.2);
        }

        table { width: 100%; border-collapse: collapse; margin: 1.5rem 0; font-family: Arial, sans-serif; }
        th, td { border: 1px solid #ddd; padding: 12px; }
        th { background: var(--primary); color: white; }
        tr:nth-child(even) { background: #fafafa; }

        footer {
            text-align: center;
            padding: 2rem;
            color: #555;
            font-size: 0.9rem;
            border-top: 1px solid #e0ddd5;
            margin-top: 2rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>Наполеон Бонапарт: путь к империи</h1>
        <nav>
            <a href="#carousel">Галерея</a>
            <a href="#bio">Биография</a>
            <a href="#wars">Сражения</a>
            <a href="#reforms">Реформы</a>
        </nav>
    </header>

    <main>
        <section id="carousel" class="card">
            <h2>Галерея: Наполеон в разные годы</h2>

            <div class="carousel-container">
                <button class="carousel-btn prev" id="prevBtn" aria-label="Назад">&#10094;</button>
                <button class="carousel-btn next" id="nextBtn" aria-label="Вперед">&#10095;</button>

                    <div class="carousel-track" id="track">
                    
                    <div class="carousel-slide">
                        <img src="images/n1.jpg" alt="Молодой Наполеон" onerror="this.src='https://via.placeholder.com/800x450?text=Image+Not+Found'">
                        <div class="carousel-caption">Наполеон в молодости — путь от артиллерийского офицера к славе.</div>
                    </div>

                    
                    <div class="carousel-slide">
                        <img src="images/n2.jpg" alt="Император Наполеон I" onerror="this.src='https://via.placeholder.com/800x450?text=Image+Not+Found'">
                        <div class="carousel-caption">Император Наполеон I — символ власти и военной славы Франции.</div>
                    </div>

                    
                    <div class="carousel-slide">
                        <img src="images/n3.jpg" alt="Наполеон на Святой Елене" onerror="this.src='https://via.placeholder.com/800x450?text=Image+Not+Found'">
                        <div class="carousel-caption">Последние годы на острове Святой Елены — закат великой карьеры.</div>
                    </div>

                    
                    <div class="carousel-slide">
                        <img src="images/n4.jpg" alt="Наполеон в парадной форме" onerror="this.src='https://via.placeholder.com/800x450?text=Image+Not+Found'">
                        <div class="carousel-caption">Наполеон в парадной военной форме — образ полководца.</div>
                    </div>
                </div>

                
                <div class="carousel-indicators" id="indicators"></div>
            </div>
        </section>

        
        <section id="bio" class="card">
            <h2>Биография: от Корсики до Тюильри</h2>
            <p>Наполеон I Бонапарт (1769–1821) — французский полководец, государственный деятель, император Франции в 1804–1814 и в 1815 году. Родился на острове Корсика, который незадолго до этого перешёл под власть Франции. С детства проявлял интерес к математике и военной истории, поступил в военное училище и быстро сделал карьеру в революционной армии.</p>
            <p>Его стремительный взлёт — редкий пример, когда талант, дисциплина и удача совпали в одной эпохе. Уже к 24 годам он стал бригадным генералом, а в 30 — фактически главой государства.</p>
        </section>

        
        <section id="wars" class="card">
    <h2>Ключевые сражения</h2>
    <table>
        <thead>
            <tr>
                <th>Год</th>
                <th>Сражение</th>
                <th>Значение</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1805</td>
                <td><a href="#austerlitz" class="battle-link">Аустерлиц</a></td>
                <td>Решающая победа над русско-австрийскими войсками («Битва трёх императоров»).</td>
            </tr>
            <tr>
                <td>1805</td>
                <td><a href="#trafalgar" class="battle-link">Трафальгар</a></td>
                <td>Поражение франко-испанского флота, господство Британии на море.</td>
            </tr>
            <tr>
                <td>1812</td>
                <td><a href="#borodino" class="battle-link">Бородинское сражение</a></td>
                <td>Крупнейшая битва кампании в России, стратегическая катастрофа для Наполеона.</td>
            </tr>
            <tr>
                <td>1813</td>
                <td><a href="#leipzig" class="battle-link">Лейпциг («Битва народов»)</a></td>
                <td>Решающее поражение коалиции, начало конца империи.</td>
            </tr>
            <tr>
                <td>1815</td>
                <td><a href="#waterloo" class="battle-link">Ватерлоо</a></td>
                <td>Окончательное поражение от войск герцога Веллингтона и Блюхера.</td>
            </tr>
        </tbody>
    </table>
</section>

        
        <section id="reforms" class="card">
            <h2>Реформы и наследие</h2>
            <ul>
                <li><strong>Гражданский кодекс (Кодекс Наполеона, 1804)</strong> — унифицировал право Франции, стал образцом для многих стран мира.</li>
                <li><strong>Банк Франции (1800)</strong> — стабилизировал финансы и валюту.</li>
                <li><strong>Система лицеев (1802)</strong> — единая сеть государственных школ.</li>
                <li><strong>Конкордат с Папой (1801)</strong> — урегулировал отношения государства и церкви после революции.</li>
            </ul>
        </section>
<section id="austerlitz" class="card" style="margin-top: 2rem;">
    <h2>Аустерлиц (1805)</h2>
    <p><strong>«Битва трёх императоров»</strong> стала вершиной военного гения Наполеона. Он намеренно создал видимость слабости, заманив союзные русско-австрийские войска в наступление.</p>
    <p>Ключевым моментом стала атака на Праценские высоты, которая расколола армию союзников надвое. Победа позволила Наполеону диктовать условия мира и фактически распустить Третью коалицию.</p>
</section>

<section id="trafalgar" class="card" style="margin-top: 2rem;">
    <h2>Трафальгар (1805)</h2>
    <p>Это морское сражение стало катастрофой для планов Наполеона по вторжению в Англию. Несмотря на гибель адмирала Нельсона, британский флот под его командованием разгромил объединённые силы Франции и Испании.</p>
    <p>Англия сохранила господство на морях на весь XIX век, а Наполеон был вынужден отказаться от высадки на Британские острова и сосредоточиться на войнах в Европе.</p>
</section>

<section id="borodino" class="card" style="margin-top: 2rem;">
    <h2>Бородинское сражение (1812)</h2>
    <p>Одно из самых кровопролитных однодневных сражений в истории. Хотя формально поле боя осталось за французами, русская армия под командованием Кутузова сохранила боеспособность.</p>
    <p>Потери были колоссальными с обеих сторон. Для Наполеона взятие Москвы не принесло победы, а лишь стало началом гибели его «Великой армии» из-за пожара, голода и суровой зимы.</p>
</section>

<section id="leipzig" class="card" style="margin-top: 2rem;">
    <h2>Лейпциг (1813)</h2>
    <p>Известная как «Битва народов», она собрала на поле боя войска почти всей Европы против Франции. Силы коалиции (Россия, Пруссия, Австрия, Швеция) значительно превосходили армию Наполеона.</p>
    <p>Поражение под Лейпцигом привело к освобождению Германии от французского владычества и вынудило Наполеона отступить за Рейн, к границам Франции.</p>
</section>

<section id="waterloo" class="card" style="margin-top: 2rem;">
    <h2>Ватерлоо (1815)</h2>
    <p>Последнее крупное сражение Наполеона, произошедшее после его возвращения с острова Эльба («Сто дней»). Армии герцога Веллингтона и прусские войска под командованием Блюхера нанесли ему сокрушительный удар.</p>
    <p>После Ватерлоо Наполеон был сослан на остров Святой Елены, где и провёл остаток жизни. Это сражение окончательно положило конец наполеоновским войнам.</p>
</section>
    </main>

    <footer>
        <p>&copy; 2026 Учебный проект по информатике. Автор: Абрахимова Анастасия.</p>
    </footer>

    
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const track = document.getElementById('track');
            const slides = Array.from(track.children);
            const prevBtn = document.getElementById('prevBtn');
            const nextBtn = document.getElementById('nextBtn');
            const indicatorsContainer = document.getElementById('indicators');

            let currentIndex = 0;
            const totalSlides = slides.length;

            
            slides.forEach((_, index) => {
                const dot = document.createElement('div');
                dot.classList.add('dot');
                if (index === 0) dot.classList.add('active');
                dot.addEventListener('click', () => goToSlide(index));
                indicatorsContainer.appendChild(dot);
            });

            const dots = document.querySelectorAll('.dot');

            function updateUI() {
                track.style.transform = `translateX(-${currentIndex * 100}%)`;
                dots.forEach((dot, index) => {
                    dot.classList.toggle('active', index === currentIndex);
                });
            }

            function goToSlide(index) {
                currentIndex = (index + totalSlides) % totalSlides;
                updateUI();
            }

            prevBtn.addEventListener('click', () => {
                currentIndex = (currentIndex - 1 + totalSlides) % totalSlides;
                updateUI();
            });

            nextBtn.addEventListener('click', () => {
                currentIndex = (currentIndex + 1) % totalSlides;
                updateUI();
            });

            
            setInterval(() => {
                currentIndex = (currentIndex + 1) % totalSlides;
                updateUI();
            }, 5000);

            updateUI(); 
        });
    </script>
</body>
</html>
