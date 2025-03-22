#<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Nauaev_ | Портфолио</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Montserrat', sans-serif;
      background: linear-gradient(135deg, #1e1e2f, #3b3b5e);
      color: #f0f0f0;
      text-align: center;
      line-height: 1.6;
    }
    header {
      background: rgba(0, 0, 0, 0.8);
      padding: 20px;
      font-size: 28px;
      font-weight: 600;
      text-shadow: 1px 1px 3px rgba(0,0,0,0.5);
      position: sticky;
      top: 0;
      z-index: 100;
    }
    section {
      padding: 50px 10%;
    }
    h2 {
      font-size: 32px;
      margin-bottom: 20px;
      text-transform: uppercase;
      letter-spacing: 1.5px;
    }
    .about-section {
      display: flex;
      flex-direction: column;
      gap: 40px;
      align-items: center;
    }
    .about-item {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      max-width: 1000px;
      background: rgba(255, 255, 255, 0.05);
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(0,0,0,0.3);
    }
    .about-item img {
      width: 280px;
      height: 280px;
      object-fit: cover;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(0,0,0,0.4);
      transition: transform 0.3s ease;
    }
    .about-item img:hover {
      transform: scale(1.05);
    }
    .about-text {
      max-width: 500px;
      text-align: left;
      padding: 10px;
    }
    .work-list {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 20px;
    }
    .work-list a {
      display: inline-block;
      padding: 20px;
      width: 260px;
      text-align: center;
      font-size: 16px;
      color: #fff;
      text-decoration: none;
      background: linear-gradient(135deg, #ff416c, #ff4b2b);
      border-radius: 10px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .work-list a:hover {
      transform: scale(1.05);
      box-shadow: 0 0 20px rgba(255, 75, 43, 0.7);
    }
    .custom-button {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 5px;
    }
    .top-text {
      font-size: 14px;
      font-weight: 600;
      letter-spacing: 1px;
    }
    .bottom-text {
      font-size: 20px;
      font-weight: 600;
    }
    form {
      background: rgba(255, 255, 255, 0.1);
      padding: 25px;
      border-radius: 15px;
      max-width: 450px;
      margin: auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
      box-shadow: 0 0 20px rgba(0,0,0,0.3);
    }
    input, textarea {
      width: 100%;
      padding: 12px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      background: rgba(255, 255, 255, 0.1);
      color: #fff;
    }
    button {
      width: 100%;
      padding: 12px;
      background: #ff416c;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-size: 18px;
      font-weight: 600;
      transition: background 0.3s ease;
    }
    button:hover {
      background: #ff4b2b;
    }
    footer {
      background: rgba(0, 0, 0, 0.9);
      padding: 20px;
      margin-top: 40px;
      font-size: 14px;
    }
  </style>
  <script>
    function sendToWhatsApp() {
      let name = document.getElementById("name").value.trim();
      let phone = document.getElementById("phone").value.trim();
      let message = document.getElementById("message").value.trim();
      let phoneNumber = "7022894952";

      if (!name || !phone || !message) {
        alert("Пожалуйста, заполните все поля!");
        return;
      }

      let text = `Заявка с сайта:\n👤 Имя: ${name}\n📞 Телефон: ${phone}\n✉️ Сообщение: ${message}`;
      let url = `https://wa.me/${phoneNumber}?text=${encodeURIComponent(text)}`;

      window.open(url, "_blank");
    }
  </script>
</head>
<body>
  <header>Nauaev_</header>

<!-- Секция "Обо мне" -->
<section id="about">
    <h2>Обо мне</h2>
    <div class="about-section">
        <!-- Блок 1 -->
        <div class="about-item">
            <div class="about-text">
                <p>Привет! Меня зовут <strong>Нурали</strong>, и я создаю не просто фото и видео, а <strong>истории, которые цепляют</strong>. Мобилографией я занимаюсь уже <strong>1,5 года</strong>, и за это время превратил обычный телефон в мощный инструмент для съемки контента, который <strong>работает и приносит результат</strong>.</p>
            </div>
            <img src="https://i.postimg.cc/mZzP4wPX/IMG-2334.jpg" alt="Фото 1">
        </div>
        <!-- Блок 2 -->
        <div class="about-item">
            <img src="https://i.postimg.cc/dV4srk7Z/IMG-0928.jpg" alt="Фото 2">
            <div class="about-text">
                <p>Я не просто нажимаю на кнопку "Запись". Я:</p>
                <ul>
                    <li>🎥 <strong>Раскрываю характер</strong> бизнеса или личного бренда через динамичные видео.</li>
                    <li>🔥 Создаю <strong>атмосферные и цепляющие</strong> кадры, которые хочется пересматривать.</li>
                    <li>📈 Помогаю предпринимателям <strong>выделяться в соцсетях</strong> и привлекать клиентов.</li>
                </ul>
            </div>
        </div>
        <!-- Блок 3 -->
        <div class="about-item">
            <div class="about-text">
                <h3>Почему выбирают меня?</h3>
                <ul>
                    <li>✅ <strong>Креатив + тренды</strong> – делаю контент, который реально заходит в соцсетях.</li>
                    <li>✅ <strong>Эмоции в кадре</strong> – твой бренд, товар или личность заиграет по-новому.</li>
                    <li>✅ <strong>Гибкость и скорость</strong> – съемка и монтаж без затягиваний.</li>
                </ul>
                <p>Готов создать для тебя <strong>визуальный контент, который выделит среди конкурентов</strong>. Пора показать миру твой стиль!</p>
            </div>
            <img src="https://i.postimg.cc/mg2RLLdL/DFCB500-A-C7-A2-42-DB-8-D39-CAE6-A1-B665-A9.jpg" alt="Фото 3">
        </div>
    </div>
</section>

  <section id="works">
    <h2>Мои работы</h2>
    <div class="work-list">
      <a href="https://www.instagram.com/reel/C-kmaZQsheB/" class="custom-button">
        <span class="top-text">marikartem_show</span>
        <span class="bottom-text">Tree of Life</span>
      </a>
      <a href="https://www.instagram.com/prokat.aktau_/">Prokat Aktau</a>
      <a href="https://www.instagram.com/reel/C87FRQFM7gA/" class="custom-button">
        <span class="top-text">marikartem_show</span>
        <span class="bottom-text">krasnoffparty</span>
      </a>
      <a href="https://www.instagram.com/flower_restobar_aktau/" class="custom-button">
        <span class="top-text">Flower restobar</span>
      </a>
      <a href="https://www.instagram.com/nauaev_/">Мой профиль</a>
    </div>
  </section>

  <section id="contact">
    <h2>Оставить заявку</h2>
    <form onsubmit="sendToWhatsApp(); return false;">
      <input type="text" id="name" placeholder="Ваше имя" required>
      <input type="tel" id="phone" placeholder="Ваш номер телефона" required>
      <textarea id="message" rows="4" placeholder="Ваше сообщение" required></textarea>
      <button type="submit">Отправить в WhatsApp</button>
    </form>
  </section>

  <footer>&copy; 2025 Nauaev_. Все права защищены.</footer>
</body>
</html>