<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Портфоліо - Іван Бойко</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Roboto:wght@400;500&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Roboto', sans-serif;
      background: #f8f9fa;
      color: #333;
      line-height: 1.6;
    }

    .container {
      width: 100%;
      max-width: 960px;
      margin: 40px auto;
      background-color: #fff;
      padding: 40px;
      border-radius: 15px;
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
      overflow: hidden;
      color: #333;
      animation: fadeIn 1s ease-in-out;
      font-family: 'Playfair Display', serif;
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
      font-size: 48px;
      font-weight: bold;
      color: #2c3e50;
      margin-bottom: 20px;
      transition: transform 0.3s ease;
      font-family: 'Playfair Display', serif;
    }

    h1:hover {
      transform: scale(1.05);
    }

    .lang-switcher {
      display: flex;
      justify-content: flex-end;
      margin-bottom: 20px;
    }

    .lang-switcher button {
      background-color: #ffd700;
      border: none;
      color: white;
      padding: 10px 20px;
      margin-left: 15px;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
      font-family: 'Roboto', sans-serif;
      transition: background-color 0.3s ease;
    }

    .lang-switcher button:hover {
      background-color: #e0a800;
    }

    h2 {
      font-size: 30px;
      color: #1a73e8;
      border-bottom: 2px solid #ffd700;
      padding-bottom: 8px;
      margin-top: 40px;
      font-weight: bold;
    }

    p, li {
      font-size: 18px;
      line-height: 1.8;
      margin-bottom: 20px;
    }

    ul {
      list-style: none;
      padding-left: 0;
    }

    .highlight {
      background-color: #ffd700;
      color: #2c3e50;
      padding: 4px 10px;
      border-radius: 5px;
      font-weight: bold;
    }

    .contact-info {
      margin-bottom: 30px;
    }

    .contact-info p {
      margin: 10px 0;
    }

    a {
      color: #1a73e8;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }

    a:hover {
      color: #ffd700;
    }

    .emoji {
      font-size: 22px;
    }

    .footer {
      font-style: italic;
      color: #777;
      text-align: center;
      margin-top: 40px;
    }

    /* Mobile responsiveness */
    @media screen and (max-width: 768px) {
      .container {
        margin: 20px;
        padding: 25px;
      }

      h1 {
        font-size: 36px;
      }

      h2 {
        font-size: 26px;
      }

      p, li {
        font-size: 16px;
      }

      .lang-switcher {
        flex-direction: column;
        align-items: center;
      }

      .lang-switcher button {
        margin: 10px 0;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="lang-switcher">
      <button onclick="switchLang('uk')">🇺🇦 Українська</button>
      <button onclick="switchLang('en')">🇬🇧 English</button>
    </div>

    <div id="content-uk">
      <h1>Іван Бойко</h1>

      <div class="contact-info">
        <p><span class="highlight">Професія:</span> Студент комп'ютерних наук</p>
        <p><span class="highlight">Email:</span> bivan2544@gmail.com</p>
        <p><span class="highlight">Телефон:</span> +380 68 791 0545</p>
      </div>

      <h2>Про мене</h2>
      <p>Я – мотивований студент першого курсу, навчаюсь на факультеті комп'ютерних наук у КНУБА. Цікавлюсь програмуванням, управлінням проєктами та сучасними технологіями. Відкритий до нових знань і завжди прагну вдосконалювати свої навички.</p>

      <h2>Освіта</h2>
      <ul>
        <li>Київський національний університет будівництва і архітектури (2024–2028)</li>
        <li>Загальноосвітня школа (2013–2024)</li>
      </ul>

      <h2>Навички</h2>
      <ul>
        <li><strong>Мови програмування:</strong> C++, HTML, CSS</li>
        <li><strong>Інструменти:</strong> Git, MS Office</li>
        <li><strong>Мови:</strong> Англійська – вище середнього</li>
      </ul>

      <h2>Досвід</h2>
      <ul>
        <li>Участь у командних проєктах в університеті</li>
        <li>Самостійне навчання через онлайн-курси (Coursera, Udemy)</li>
      </ul>

      <h2>Інтереси</h2>
      <ul>
        <li>Домашні улюбленці (особливо песики 🐶)</li>
        <li>Спорт та активний відпочинок</li>
        <li>Читання технічної літератури</li>
        <li>Рукопашний бій (КМС) – можу показати шлях руки та постояти в кібадачі 🥋<br>
          <a href="https://www.facebook.com/HandToHandCombatFederation/" target="_blank">Федерація рукопашного бою України</a>
        </li>
        <li>Колекціонування та торгівля людьми онлайн 🛍️</li>
      </ul>

      <div class="footer">
        <p>А ще маю файних філімонів 😸 – завжди поруч, підтримують і муркотять.</p>
      </div>
    </div>

    <div id="content-en" style="display:none;">
      <h1>Ivan Boiko</h1>

      <div class="contact-info">
        <p><span class="highlight">Profession:</span> Computer Science student</p>
        <p><span class="highlight">Email:</span> bivan2544@gmail.com</p>
        <p><span class="highlight">Phone:</span> +380 68 791 0545</p>
      </div>

      <h2>About Me</h2>
      <p>I am a motivated first-year student studying Computer Science at KNUCA. I am interested in programming, project management, and modern technologies. I am open to new knowledge and always strive to improve my skills.</p>

      <h2>Education</h2>
      <ul>
        <li>Kyiv National University of Construction and Architecture (2024–2028)</li>
        <li>Secondary School (2013–2024)</li>
      </ul>

      <h2>Skills</h2>
      <ul>
        <li><strong>Programming languages:</strong> C++, HTML, CSS</li>
        <li><strong>Tools:</strong> Git, MS Office</li>
        <li><strong>Languages:</strong> English – Intermediate</li>
      </ul>

      <h2>Experience</h2>
      <ul>
        <li>Participation in university team projects</li>
        <li>Self-learning through online courses (Coursera, Udemy)</li>
      </ul>

      <h2>Interests</h2>
      <ul>
        <li>Pets (especially dogs 🐶)</li>
        <li>Sports and outdoor activities</li>
        <li>Reading technical literature</li>
        <li>Hand-to-hand combat (2nd degree black belt) – I can demonstrate the way of the hand and stand in Kibadachi 🥋<br>
          <a href="https://www.facebook.com/HandToHandCombatFederation/" target="_blank">Federation of Hand-to-Hand Combat of Ukraine</a>
        </li>
        <li>Collecting and trading online goods 🛍️</li>
      </ul>

      <div class="footer">
        <p>I also have some cool felines 😸 – always around, supporting and purring.</p>
      </div>
    </div>
  </div>

  <script>
    function switchLang(lang) {
      const contentUk = document.getElementById('content-uk');
      const contentEn = document.getElementById('content-en');
      
      if (lang === 'uk') {
        contentUk.style.display = 'block';
        contentEn.style.display = 'none';
      } else {
        contentUk.style.display = 'none';
        contentEn.style.display = 'block';
      }
    }
  </script>
</body>
</html>
