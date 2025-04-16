<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Портфоліо - Іван Бойко</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Roboto:wght@400;500&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
  <style>
    :root {
      --bg-light: linear-gradient(135deg, #e3f2fd, #fceabb);
      --bg-dark: #121212;
      --text-light: #333;
      --text-dark: #eee;
      --primary: #ffd700;
      --accent: #ff9800;
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
      transition: all 0.5s ease;
      scroll-behavior: smooth;
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
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
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
      color: var(--accent);
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
      background: linear-gradient(45deg, var(--primary), var(--accent));
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
      background: linear-gradient(45deg, var(--accent), var(--primary));
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
      bottom: 20px;
      right: 20px;
      z-index: 999;
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .floating-btns a {
      background-color: var(--primary);
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
      background-color: var(--accent);
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

    @media (max-width: 768px) {
      .container {
        margin: 20px;
        padding: 25px;
      }

      h1 {
        font-size: 36px;
      }

      h2 {
        font-size: 24px;
      }

      p, li {
        font-size: 16px;
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
      <p>Муркотять завжди поруч 😺</p>
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
    </ul>

    <h2>Interests</h2>
    <ul>
      <li>Dogs 🐶</li>
      <li>Sports</li>
      <li>Hand-to-hand combat 🥋 <a href="https://www.facebook.com/HandToHandCombatFederation/" target="_blank">Federation</a></li>
      <li>Cats 😸</li>
    </ul>

    <div class="footer">
      <p>Some cool felines are always purring near me 😺</p>
    </div>
  </div>

  <div class="floating-btns">
    <a href="https://www.linkedin.com/in/ivan-boiko/" target="_blank" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
    <a href="https://github.com/ivan-boiko" target="_blank" title="GitHub"><i class="fab fa-github"></i></a>
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
