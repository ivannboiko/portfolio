<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Портфоліо - Іван Бойко</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Roboto:wght@400;500&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" />
  <style>
    :root {
      --bg-light: linear-gradient(135deg, #e3f2fd, #fceabb);
      --bg-dark: #121212;
      --text-light: #333;
      --text-dark: #eee;
      --primary: rgb(139, 170, 36);
    }

    html, body {
      height: 100%;
      margin: 0;
      padding: 0;
      overflow-x: hidden;
      font-family: 'Roboto', sans-serif;
      scroll-behavior: smooth;
      transition: all 0.5s ease;
    }

    body {
      background: var(--bg-light);
      color: var(--text-light);
    }

    body.dark {
      background: var(--bg-dark);
      color: var(--text-dark);
    }

    .container {
      max-width: 960px;
      margin: 40px auto;
      background: rgba(255, 255, 255, 0.95);
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 25px 50px rgba(0, 0, 0, 0.1);
      animation: fadeIn 1s ease;
      font-family: 'Playfair Display', serif;
      transition: background 0.5s ease, color 0.5s ease;
    }

    body.dark .container {
      background: rgba(30, 30, 30, 0.95);
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    h1 {
      text-align: center;
      font-size: 48px;
      color: #2c3e50;
      margin-bottom: 20px;
      transition: 0.3s ease;
    }

    h1:hover {
      transform: scale(1.05);
      color: var(--primary);
    }

    .kitty {
      text-align: center;
      font-size: 48px;
      animation: kittyBlink 2s infinite;
    }

    @keyframes kittyBlink {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.1); }
    }

    .lang-switcher, .theme-switcher {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 15px;
      margin-bottom: 20px;
    }

    button {
      background: var(--primary);
      border: none;
      color: white;
      padding: 10px 20px;
      border-radius: 12px;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      transition: 0.3s ease;
    }

    button:hover {
      background: #7b1fa2;
      transform: scale(1.05);
    }

    h2 {
      font-size: 28px;
      color: #1a237e;
      border-bottom: 2px dashed var(--primary);
      padding-bottom: 8px;
      margin-top: 30px;
    }

    body.dark h2 {
      color: #ffc107;
    }

    p, li {
      font-size: 18px;
      margin-bottom: 15px;
    }

    ul {
      list-style: none;
      padding-left: 0;
    }

    ul li::before {
      content: '⭐';
      margin-right: 10px;
    }

    .highlight {
      background-color: var(--primary);
      color: #2c3e50;
      padding: 4px 10px;
      border-radius: 5px;
      font-weight: bold;
    }

    .contact-info p {
      margin: 8px 0;
    }

    a {
      color: #1976d2;
      font-weight: bold;
      text-decoration: none;
    }

    a:hover {
      color: var(--primary);
      text-decoration: underline;
    }

    .footer {
      text-align: center;
      font-style: italic;
      color: #777;
      margin-top: 40px;
    }

    .floating-btns {
      position: fixed;
      bottom: 0;
      left: 0;
      width: 100%;
      background: rgba(0, 0, 0, 0.05);
      padding: 10px 0;
      display: flex;
      justify-content: center;
      gap: 20px;
      z-index: 999;
      border-top-left-radius: 12px;
      border-top-right-radius: 12px;
      box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.1);
      touch-action: manipulation;
    }

    .floating-btns a {
      background-color: var(--primary);
      color: white;
      padding: 10px;
      border-radius: 50%;
      font-size: 20px;
      text-align: center;
      transition: 0.3s ease;
    }

    .floating-btns a:hover {
      transform: scale(1.1);
      background-color: #7b1fa2;
    }

    .social-icons {
      font-size: 18px;
      margin-top: 15px;
    }

    .social-icons a {
      margin: 0 10px;
      color: #1976d2;
      font-size: 24px;
    }

    /* 📱 Мобільна адаптація */
    @media (max-width: 480px) {
      html, body {
        font-size: 14px;
        margin: 0;
        padding: 0;
        overflow-x: hidden;
      }

      .container {
        margin: 5px;
        padding: 15px;
        border-radius: 12px;
        box-shadow: none;
        font-size: 14px;
      }

      h1 {
        font-size: 24px;
        margin-bottom: 10px;
      }

      h2 {
        font-size: 18px;
        margin-top: 20px;
        margin-bottom: 10px;
      }

      .kitty {
        font-size: 28px;
        margin-bottom: 5px;
      }

      .lang-switcher, .theme-switcher {
        flex-direction: column;
        gap: 8px;
        padding: 0 10px;
      }

      button {
        width: 100%;
        font-size: 14px;
        padding: 10px;
        border-radius: 8px;
      }

      p, li {
        font-size: 14px;
        margin-bottom: 10px;
        line-height: 1.4;
      }

      ul {
        padding-left: 10px;
      }

      ul li::before {
        content: '•';
        margin-right: 6px;
      }

      .contact-info p {
        margin: 5px 0;
      }

      .social-icons {
        font-size: 18px;
        text-align: center;
      }

      .social-icons a {
        font-size: 20px;
        margin: 0 6px;
      }

      .floating-btns {
        flex-direction: row;
        justify-content: center;
        gap: 12px;
        padding: 6px 0;
        border-radius: 0;
        background: rgba(0,0,0,0.08);
      }

      .floating-btns a {
        font-size: 18px;
        padding: 8px;
        width: 40px;
        height: 40px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
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
    <p>Я – мотивований студент першого курсу, навчаюсь на факультеті комп'ютерних наук у КНУБА. Цікавлюсь програмуванням, управлінням проєктами та сучасними технологіями.</p>

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
    <p>I’m a motivated first-year CS student at KNUCA. Interested in coding, project management, and technology.</p>

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
      <li>Self-learning via Coursera, Udemy</li>
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
