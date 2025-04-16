<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Іван Бойко - Портфоліо</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
  <style>
    :root {
      --primary-color: #8e44ad;
      --secondary-color: #ecf0f1;
      --bg-light: #f7f7f7;
      --bg-dark: #2c3e50;
      --text-light: #2c3e50;
      --text-dark: #ecf0f1;
      --highlight: #e74c3c;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Roboto', sans-serif;
      background: var(--bg-light);
      color: var(--text-light);
      transition: all 0.3s ease;
      scroll-behavior: smooth;
    }

    body.dark {
      background: var(--bg-dark);
      color: var(--text-dark);
    }

    .container {
      max-width: 1200px;
      margin: 30px auto;
      padding: 40px;
      border-radius: 20px;
      background-color: rgba(255, 255, 255, 0.9);
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
      transition: background-color 0.5s, color 0.5s;
      opacity: 0;
      animation: fadeIn 1s forwards;
    }

    body.dark .container {
      background-color: rgba(44, 62, 80, 0.9);
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }

    h1 {
      text-align: center;
      font-size: 50px;
      color: var(--primary-color);
      text-transform: uppercase;
      margin-bottom: 20px;
      transition: all 0.3s ease;
    }

    h1:hover {
      transform: scale(1.1);
      color: #fff;
    }

    .intro-text {
      text-align: center;
      font-size: 20px;
      margin-bottom: 40px;
      font-weight: 500;
    }

    .intro-text p {
      margin-top: 10px;
      font-size: 18px;
    }

    .section-title {
      font-size: 28px;
      text-align: center;
      color: var(--primary-color);
      margin: 30px 0;
      border-bottom: 2px dashed var(--primary-color);
      padding-bottom: 8px;
    }

    ul {
      list-style: none;
      padding-left: 0;
    }

    ul li {
      font-size: 18px;
      margin-bottom: 15px;
    }

    .highlight {
      color: var(--highlight);
    }

    button {
      background: var(--primary-color);
      border: none;
      color: white;
      padding: 10px 20px;
      border-radius: 12px;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
      transition: 0.3s ease;
    }

    button:hover {
      background: #7b1fa2;
      transform: scale(1.05);
    }

    /* Парallax ефект */
    .parallax {
      background-image: url('https://www.example.com/background.jpg');
      min-height: 400px;
      background-attachment: fixed;
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
    }

    /* Чат-бот */
    .chatbot {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #4caf50;
      border-radius: 50%;
      color: white;
      font-size: 30px;
      padding: 15px;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
      transition: 0.3s;
    }

    .chatbot:hover {
      background: #388e3c;
    }

    .floating-btns {
      position: fixed;
      bottom: 20px;
      right: 80px;
      z-index: 999;
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .floating-btns a {
      background-color: var(--primary-color);
      color: white;
      padding: 10px;
      border-radius: 50%;
      font-size: 20px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
      text-align: center;
      transition: 0.3s ease;
    }

    .floating-btns a:hover {
      transform: scale(1.1);
      background-color: #7b1fa2;
    }

    @media (max-width: 768px) {
      .container {
        margin: 20px;
        padding: 25px;
      }

      h1 {
        font-size: 36px;
      }

      .section-title {
        font-size: 24px;
      }

      p, li {
        font-size: 16px;
      }
    }
  </style>
</head>
<body>

  <!-- Паралакс фон -->
  <div class="parallax"></div>

  <div class="container">
    <h1>Іван Бойко</h1>
    <div class="intro-text">
      <p>Студент комп'ютерних наук | Програміст | Проєктний менеджер</p>
    </div>

    <h2 class="section-title">Про мене</h2>
    <p>Я студент першого курсу комп'ютерних наук у КНУБА. Моя мета — стати частиною інноваційного світу технологій і програмування.</p>

    <h2 class="section-title">Навички</h2>
    <ul>
      <li><strong>Мови програмування:</strong> C++, HTML, CSS</li>
      <li><strong>Інструменти:</strong> Git, MS Office</li>
      <li><strong>Англійська:</strong> Вільно</li>
    </ul>

    <h2 class="section-title">Контакти</h2>
    <ul>
      <li>Email: bivan2544@gmail.com</li>
      <li>Телефон: +380 68 791 0545</li>
    </ul>
  </div>

  <!-- Кнопка для відкриття чат-бота -->
  <div class="chatbot">
    <i class="fas fa-comments"></i>
  </div>

  <div class="floating-btns">
    <a href="https://www.instagram.com/boy4ik23/" target="_blank"><i class="fab fa-instagram"></i></a>
    <a href="https://t.me/ivannboiko" target="_blank"><i class="fab fa-telegram"></i></a>
  </div>

  <script>
    // Чат-бот інтерактивність
    document.querySelector('.chatbot').addEventListener('click', function() {
      alert('Привіт! Як я можу допомогти?');
    });
  </script>

</body>
</html>
