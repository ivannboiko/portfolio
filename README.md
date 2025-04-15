<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Портфоліо - Іван Бойко</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(to right, #edf2f7, #dbeafe);
    }

    .container {
      background-color: #ffffff;
      max-width: 900px;
      margin: 40px auto;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
    }

    h1 {
      font-size: 32px;
      text-align: center;
      margin-bottom: 20px;
      color: #1e293b;
    }

    h2 {
      font-size: 22px;
      margin-top: 30px;
      margin-bottom: 10px;
      color: #1e293b;
      border-bottom: 1px solid #cbd5e1;
      padding-bottom: 5px;
    }

    p, li {
      font-size: 16px;
      line-height: 1.6;
      color: #334155;
    }

    ul {
      padding-left: 20px;
    }

    strong {
      background-color: #e0e7ff;
      padding: 2px 6px;
      border-radius: 5px;
      font-weight: 600;
    }

    .footer {
      margin-top: 40px;
      font-style: italic;
      text-align: center;
      color: #475569;
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
    }

    .lang-switcher button:hover {
      background-color: #a5b4fc;
    }

    @media screen and (max-width: 600px) {
      .container {
        margin: 20px;
        padding: 20px;
      }

      h1 {
        font-size: 26px;
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
      <p><strong>Професія:</strong> Студент комп'ютерних наук</p>
      <p><strong>Email:</strong> bivan2544@gmail.com</p>
      <p><strong>Телефон:</strong> +380 68 791 0545</p>

      <h2>Про мене</h2>
      <p>Я – мотивований студент першого курсу, навчаюсь на факультеті комп'ютерних наук у КНУБА. Цікавлюсь програмуванням, управлінням проєктами та сучасними технологіями. Відкритий до нових знань і завжди прагну вдосконалювати свої навички.</p>

      <h2>Освіта</h2>
      <ul>
        <li>Київський національний університет будівництва і архітектури (2024–2028)</li>
        <li>Загальноосвітня школа (2013–2024)</li>
      </ul>

      <h2>Навички</h2>
      <ul>
        <li>Мови програмування: C++, HTML, CSS</li>
        <li>Англійська – вище середнього</li>
        <li>MS Office, Git</li>
      </ul>

      <h2>Досвід</h2>
      <ul>
        <li>Участь у командних проєктах в університеті</li>
        <li>Самостійне навчання через онлайн-курси</li>
      </ul>

      <h2>Інтереси</h2>
      <ul>
        <li>Кішки 🐱</li>
        <li>Спорт</li>
        <li>Читання технічної літератури</li>
      </ul>

      <div class="footer">А ще маю файних філімонів 😸 — муркотять як сервери в дата-центрі!</div>
    </div>

    <div id="content-en" style="display: none;">
      <h1>Ivan Boiko</h1>
      <p><strong>Profession:</strong> Computer Science Student</p>
      <p><strong>Email:</strong> bivan2544@gmail.com</p>
      <p><strong>Phone:</strong> +380 68 791 0545</p>

      <h2>About Me</h2>
      <p>I am a motivated first-year student studying Computer Science at KNUCA. I'm interested in programming, project management, and modern technologies. Always eager to learn and improve my skills.</p>

      <h2>Education</h2>
      <ul>
        <li>Kyiv National University of Construction and Architecture (2024–2028)</li>
        <li>Secondary School (2013–2024)</li>
      </ul>

      <h2>Skills</h2>
      <ul>
        <li>Programming Languages: C++, HTML, CSS</li>
        <li>English – Upper-Intermediate</li>
        <li>MS Office, Git</li>
      </ul>

      <h2>Experience</h2>
      <ul>
        <li>Team projects at university</li>
        <li>Self-learning through online courses</li>
      </ul>

      <h2>Interests</h2>
      <ul>
        <li>Cats 🐱</li>
        <li>Sports</li>
        <li>Reading tech books</li>
      </ul>

      <div class="footer">Also got some cool cats 😸 — they purr like servers in a data center!</div>
    </div>
  </div>

  <script>
    function switchLang(lang) {
      document.getElementById('content-uk').style.display = lang === 'uk' ? 'block' : 'none';
      document.getElementById('content-en').style.display = lang === 'en' ? 'block' : 'none';
    }
  </script>
</body>
</html>
