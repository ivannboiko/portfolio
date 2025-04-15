
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <title>Портфоліо - Іван Бойко</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(to right, #eef2f3, #dfe9f3);
      margin: 0;
      padding: 0;
      color: #333;
    }

    .container {
      background-color: #ffffff;
      max-width: 900px;
      margin: 40px auto;
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
      animation: fadeIn 1s ease-in-out;
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
      color: #2c3e50;
      font-size: 40px;
      margin-bottom: 10px;
      text-align: center;
      font-weight: 700;
      transition: transform 0.3s ease;
    }

    h1:hover {
      transform: scale(1.05);
    }

    h2 {
      color: #34495e;
      border-bottom: 2px solid #ccc;
      padding-bottom: 5px;
      margin-top: 30px;
      font-size: 24px;
    }

    p, li {
      font-size: 16px;
      line-height: 1.6;
    }

    ul {
      padding-left: 20px;
    }

    .footer {
      margin-top: 50px;
      font-style: italic;
      color: #666;
      text-align: center;
      font-size: 15px;
    }

    .highlight {
      background-color: #dde1f3;
      padding: 4px 10px;
      border-radius: 5px;
      font-weight: bold;
    }

    .contact-info {
      margin-bottom: 20px;
    }

    .contact-info p {
      margin: 5px 0;
    }

    a {
      color: #2c3e50;
      text-decoration: underline;
      transition: color 0.3s ease;
    }

    a:hover {
      color: #1a73e8;
    }

    .emoji {
      font-size: 20px;
    }

    .lang-switcher {
      text-align: right;
      margin-bottom: 10px;
    }

    .lang-switcher button {
      margin-left: 10px;
      padding: 6px 12px;
      border-radius: 6px;
      border: none;
      background-color: #c7d2fe;
      cursor: pointer;
      font-weight: 600;
      color: #1e3a8a;
      transition: background-color 0.3s ease;
    }

    .lang-switcher button:hover {
      background-color: #a5b4fc;
    }

    .lang-switcher button:focus {
      outline: none;
    }

    @media screen and (max-width: 600px) {
      .container {
        margin: 20px;
        padding: 20px;
      }

      h1 {
        font-size: 28px;
      }

      h2 {
        font-size: 20px;
      }

      p, li {
        font-size: 15px;
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
