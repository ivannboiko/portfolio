<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Портфоліо - Іван Бойко</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Roboto:wght@400;700&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" />
  <style>
    :root {
      --bg-light: linear-gradient(135deg, #e3f2fd, #fceabb);
      --bg-dark: #121212;
      --text-light: #222;
      --text-dark: #eee;
      --primary: #8baa24;
    }

    html, body {
      margin: 0;
      padding: 0;
      font-family: 'Roboto', sans-serif;
      font-size: 20px;
      background: var(--bg-light);
      color: var(--text-light);
      transition: all 0.4s ease;
      scroll-behavior: smooth;
    }

    body.dark {
      background: var(--bg-dark);
      color: var(--text-dark);
    }

    .container {
      max-width: 900px;
      margin: 0 auto;
      padding: 30px 20px;
      background: rgba(255, 255, 255, 0.9);
      border-radius: 16px;
      box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
    }

    body.dark .container {
      background: rgba(30, 30, 30, 0.95);
    }

    h1 {
      text-align: center;
      font-family: 'Playfair Display', serif;
      font-size: 40px;
      margin-bottom: 10px;
      color: #2c3e50;
    }

    h2 {
      font-size: 26px;
      margin-top: 30px;
      border-bottom: 2px dashed var(--primary);
      padding-bottom: 6px;
    }

    p, li {
      line-height: 1.6;
      margin-bottom: 12px;
    }

    ul {
      padding-left: 0;
      list-style: none;
    }

    ul li::before {
      content: "⭐";
      margin-right: 10px;
    }

    .highlight {
      background: var(--primary);
      color: #fff;
      padding: 3px 8px;
      border-radius: 5px;
    }

    .lang-switcher {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 10px;
      margin: 20px 0;
    }

    button {
      background: var(--primary);
      border: none;
      color: white;
      padding: 10px 16px;
      border-radius: 10px;
      font-weight: bold;
      font-size: 18px;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      background: #7b1fa2;
    }

    .kitty {
      font-size: 40px;
      text-align: center;
      margin-top: 20px;
      animation: kittyBlink 2s infinite;
    }

    @keyframes kittyBlink {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.1); }
    }

    .contact-info p {
      margin: 6px 0;
    }

    a {
      color: #1976d2;
      font-weight: bold;
      text-decoration: none;
    }

    a:hover {
      color: var(--primary);
    }

    .footer {
      text-align: center;
      font-style: italic;
      margin-top: 40px;
      color: #777;
    }

    .floating-btns {
      position: fixed;
      bottom: 0;
      left: 0;
      width: 100%;
      background: rgba(0, 0, 0, 0.1);
      padding: 10px;
      display: flex;
      justify-content: center;
      gap: 20px;
      z-index: 99;
      border-top-left-radius: 12px;
      border-top-right-radius: 12px;
    }

    .floating-btns a {
      background: var(--primary);
      color: white;
      padding: 10px;
      border-radius: 50%;
      font-size: 22px;
      transition: 0.3s;
    }

    .floating-btns a:hover {
      background: #7b1fa2;
    }

    .social-icons {
      margin-top: 15px;
      text-align: center;
    }

    .social-icons a {
      margin: 0 10px;
      font-size: 24px;
      color: #1976d2;
    }

    @media (max-width: 600px) {
      body {
        font-size: 18px;
      }

      .container {
        margin: 10px;
        padding: 20px;
      }

      h1 {
        font-size: 30px;
      }

      h2 {
        font-size: 22px;
      }

      button {
        font-size: 16px;
        padding: 10px;
      }

      .kitty {
        font-size: 30px;
      }

      .social-icons {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>
</head>
<body>
  <div class="kitty">😺</div>

  <div class="lang-switcher">
    <button onclick="switchLang('uk')">🇺🇦 Українська</button>
    <button onclick="switchLang('en')">🇬🇧 English</button>
    <button onclick="toggleTheme()">🌓 Тема</button>
  </div>

  <div class="container" id="content-uk">
    <h1>Іван Бойко</h1>

    <div class="contact-info">
      <p><span class="highlight">Професія:</span> Студент комп'ютерних наук</p>
      <p><span class="highlight">Email:</span> bivan2544@gmail.com</p>
      <p><span class="highlight">Телефон:</span> +380 68 791 0545</p>
    </div>

    <h2>Про мене</h2>
    <p>Я – мотивований студент першого курсу, навчаюсь на факультеті комп'ютерних наук у КНУБА. Цікавлюсь програмуванням, управлінням проєктами та сучасними технологіями. Завжди прагну до вдосконалення та нових знань.</p>

    <h2>Освіта</h2>
    <ul>
      <li>КНУБА (2024–2028)</li>
      <li>Школа (2013–2024)</li>
    </ul>

    <h2>Навички</h2>
    <ul>
      <li><strong>Мови:</strong> C++, HTML, CSS</li>
      <li><strong>Інструменти:</strong> Git, MS Office</li>
      <li><strong>Англійська:</strong> вище середнього</li>
    </ul>

    <h2>Досвід</h2>
    <ul>
      <li>Участь у командних проєктах</li>
      <li>Онлайн-курси (Coursera, Udemy)</li>
    </ul>

    <h2>Інтереси</h2>
    <ul>
      <li>Песики 🐶</li>
      <li>Спорт</li>
      <li>Рукопашний бій 🥋 <a href="https://www.facebook.com/HandToHandCombatFederation/" target="_blank">Федерація</a></li>
    </ul>

    <div class="footer">
      <p>&copy; 2025 Іван Бойко</p>
    </div>
  </div>

  <div class="container" id="content-en" style="display:none;">
    <h1>Ivan Boiko</h1>

    <div class="contact-info">
      <p><span class="highlight">Profession:</span> Computer Science student</p>
      <p><span class="highlight">Email:</span> bivan2544@gmail.com</p>
      <p><span class="highlight">Phone:</span> +380 68 791 0545</p>
    </div>

    <h2>About Me</h2>
    <p>I’m a motivated first-year CS student at KNUCA. Interested in coding, project management, and modern technology. I always strive to improve and learn something new.</p>

    <h2>Education</h2>
    <ul>
      <li>KNUCA (2024–2028)</li>
      <li>School (2013–2024)</li>
    </ul>

    <h2>Skills</h2>
    <ul>
      <li><strong>Languages:</strong> C++, HTML, CSS</li>
      <li><strong>Tools:</strong> Git, MS Office</li>
      <li><strong>English:</strong> Intermediate</li>
    </ul>

    <h2>Experience</h2>
    <ul>
      <li>Team projects at university</li>
      <li>Online learning (Coursera, Udemy)</li>
      <li>Cats 😸</li>
    </ul>

    <div class="footer">
      <p>&copy; 2025 Ivan Boiko</p>
    </div>
  </div>

  <div class="floating-btns">
    <a href="https://www.instagram.com/boy4ik23/" target="_blank" title="Instagram"><i class="fab fa-instagram"></i></a>
    <a href="https://t.me/ivannboiko" target="_blank" title="Telegram"><i class="fab fa-telegram"></i></a>
  </div>

  <script>
    function switchLang(lang) {
      const uk = document.getElementById('content-uk');
      const en = document.getElementById('content-en');
      if (lang === 'uk') {
        uk.style.display = 'block';
        en.style.display = 'none';
      } else {
        uk.style.display = 'none';
        en.style.display = 'block';
      }
    }

    function toggleTheme() {
      document.body.classList.toggle('dark');
    }
  </script>
</body>
</html>
