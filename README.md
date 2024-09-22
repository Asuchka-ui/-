<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Обезьяна Осыпь</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Обезьяна Осыпь: Загадочная Болезнь</h1>
        <nav>
            <ul>
                <li><a href="#introduction">Введение</a></li>
                <li><a href="#gallery">Галерея</a></li>
                <li><a href="#contact">Контакты</a></li>
            </ul>
        </nav>
    </header>

    <section id="introduction">
        <div class="container">
            <h2>Введение</h2>
            <p>Обезьяна осыпь — это редкая и загадочная болезнь, которая поражает как людей, так и обезьян.</p>
        </div>
    </section>

    <section id="gallery">
        <div class="container">
            <h2>Галерея Исследований</h2>
            <div class="gallery">
                <img src="images/rost.png" alt="Рост высыпаний на коже">
                <img src="images/tolstaya.png" alt="Толстая обезьяна с симптомами">
                <!-- Добавь другие изображения -->
            </div>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>Контакты</h2>
            <p>Свяжитесь с нами по адресу: <a href="mailto:info@example.com">info@example.com</a></p>
        </div>
    </section>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #000;
    color: #fff;
}

header {
    background-color: #1a1a1a;
    padding: 20px;
    text-align: center;
}

header nav ul {
    list-style: none;
    padding: 0;
}

header nav ul li {
    display: inline;
    margin: 0 15px;
}

header nav ul li a {
    color: #fff;
    text-decoration: none;
}

.container {
    width: 80%;
    margin: 20px auto;
    padding: 20px;
    background-color: #222;
    border-radius: 8px;
}

h1, h2 {
    color: #4CAF50;
}

.gallery {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}

.gallery img {
    width: 45%;
    margin: 10px 0;
    border-radius: 8px;
    transition: transform 0.3s;
}

.gallery img:hover {
    transform: scale(1.05);
}

footer {
    text-align: center;
    padding: 10px;
    background-color: #1a1a1a;
}

    <footer>
        <p>&copy; 2024 Обезьяна Осыпь. Все права защищены.</p>
    </footer>
</body>
</html>
