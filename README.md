<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Portfolio Showcase</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #f4f4f4;
      color: #000;
    }

    /* ===== INTRO SCREEN ===== */
    #intro-screen {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: #111;
      color: white;
      text-align: center;
    }

    #intro-screen button {
      margin-top: 20px;
      padding: 14px 28px;
      font-size: 1.5rem;
      border: 2px solid #fff;
      background: transparent;
      color: #fff;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s ease;
    }
    #intro-screen button:hover {
      background: #fff;
      color: #111;
    }

    /* ===== CRM APP ===== */
    #crm-section {
      position: relative;
      display: flex;
      flex-direction: column;
      align-items: center;
      margin: 0;
      background: #f4f4f4;
    }

    .crm-header {
      position: sticky;
      top: 0;
      z-index: 1000;
      display: flex;
      align-items: center;
      background-color: rgba(255, 255, 255, 0.85);
      padding: 20px 40px;
      font-size: 2rem;
      font-weight: bold;
      border-bottom: 2px solid #ddd;
      width: 100%;
      backdrop-filter: blur(4px);
    }

    .crm-header img {
      width: 32px;
      height: 32px;
      margin-right: 12px;
    }

    .crm-content {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 60px 40px;
    }

    .phone-container {
      width: 360px;
      height: 720px;
      border-radius: 40px;
      display: flex;
      justify-content: center;
      align-items: center;
      animation: floatRotate 6s infinite ease-in-out;
      transform-style: preserve-3d;
      margin-bottom: 30px;
    }

    @keyframes floatRotate {
      0% { transform: rotateX(0deg) rotateY(0deg) translateY(0px); }
      50% { transform: rotateX(10deg) rotateY(10deg) translateY(-10px); }
      100% { transform: rotateX(0deg) rotateY(0deg) translateY(0px); }
    }

    .screen img {
      width: 100%;
      height: 100%;
      object-fit: contain;
      border-radius: 40px;
    }

    .info-button {
      padding: 12px 24px;
      font-size: 1rem;
      background-color: forestgreen;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      text-decoration: none;
      margin-bottom: 20px;
    }

    .reader-effect {
      font-size: 1.6rem;
      max-width: 800px;
      text-align: left;
      margin-top: 40px;
      line-height: 1.8;
      color: black;
      cursor: pointer;
    }

    .reader-effect span {
      opacity: 0.6;
      transition: color 0.3s ease, opacity 0.3s ease;
    }

    .reader-effect span.active {
      color: forestgreen;
      font-weight: bold;
      opacity: 1;
    }

    /* ===== UX PORTFOLIO ===== */
    #ux-portfolio {
      position: relative;
      background: #fff;
      padding-bottom: 100px;
      overflow: hidden;
    }

    #ux-portfolio .crm-header {
      position: sticky;
      top: 0;
      z-index: 1000;
      display: flex;
      align-items: center;
      background-color: rgba(255, 255, 255, 0.85);
      padding: 20px 40px;
      font-size: 2rem;
      font-weight: bold;
      border-bottom: 2px solid #ddd;
      width: 100%;
      backdrop-filter: blur(4px);
    }

    #ux-portfolio .crm-header img {
      width: 32px;
      height: 32px;
      margin-right: 12px;
      object-fit: contain;
    }

    #ux-portfolio .collage {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 18px;
      max-width: 1800px;
      margin: 20px auto 0;
      background: #fff;
    }

    #ux-portfolio .collage img {
      width: 130%;
      display: block;
      animation: floatUp 12s linear infinite;
    }

    #ux-portfolio .collage img:nth-child(1) { animation-delay: 0s; }
    #ux-portfolio .collage img:nth-child(2) { animation-delay: 3s; }
    #ux-portfolio .collage img:nth-child(3) { animation-delay: 6s; }
    #ux-portfolio .collage img:nth-child(4) { animation-delay: 9s; }
    #ux-portfolio .collage img:nth-child(5) { animation-delay: 1.5s; }
    #ux-portfolio .collage img:nth-child(6) { animation-delay: 4.5s; }
    #ux-portfolio .collage img:nth-child(7) { animation-delay: 7.5s; }
    #ux-portfolio .collage img:nth-child(8) { animation-delay: 10.5s; }

    @keyframes floatUp {
      0%   { transform: translateY(0); opacity: 1; }
      40%  { transform: translateY(-130%); opacity: 0; }
      41%  { transform: translateY(130%);  opacity: 0; }
      100% { transform: translateY(0);     opacity: 1; }
    }

    /* ===== CONTACT FORM ===== */
    #contact {
      padding: 60px 20px;
      background: #f9f9f9;
    }
    #contact h2 {
      text-align: center;
      font-size: 2rem;
      margin-bottom: 20px;
    }
    #contact form {
      max-width: 600px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
    }
    #contact input, #contact textarea {
      padding: 12px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 1rem;
    }
    #contact button {
      padding: 12px;
      background: forestgreen;
      color: #fff;
      font-size: 1rem;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }

    /* ===== AI HELP BOT ===== */
    #ai-bot {
      position: fixed;
      bottom: 20px;
      right: 20px;
      width: 260px;
      height: 360px;
      background: white;
      border-radius: 12px;
      box-shadow: 0 0 15px rgba(0,0,0,0.3);
      overflow: hidden;
      display: flex;
      flex-direction: column;
      font-size: 0.9rem;
    }
    #ai-bot-header {
      background: forestgreen;
      color: white;
      padding: 10px;
      text-align: center;
    }
    #ai-bot-messages {
      flex: 1;
      padding: 10px;
      overflow-y: auto;
    }
    #ai-bot-input {
      border: none;
      border-top: 1px solid #ddd;
      padding: 10px;
      width: 100%;
    }
  </style>
</head>
<body>

  <!-- INTRO -->
  <section id="intro-screen">
    <h1>Welcome</h1>
    <button onclick="document.getElementById('crm-section').scrollIntoView({behavior:'smooth'})">
      hier eintragen
    </button>
  </section>

  <!-- CRM APP -->
  <section id="crm-section">
    <div class="crm-header">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/CRM%20APP%20Logo%202.jpg" alt="CRM Logo" />
      CRM App
    </div>

    <div class="crm-content">
      <div class="phone-container">
        <div class="screen">
          <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/nobackground%20cutout%20.png" alt="CRM App Interface">
        </div>
      </div>

      <a class="info-button" href="https://github.com/SWMarketingTech/SWFiles/tree/main/CRMDaily" target="_blank">
        More Info
      </a>

      <div class="reader-effect" id="reader"></div>
    </div>
  </section>

  <!-- UX PORTFOLIO -->
  <section id="ux-portfolio">
    <header class="crm-header">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/Portfolio%20P%20Snippet.jpg" alt="SW Logo" />
      Portfolio
    </header>

    <div class="collage">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/Create%20a%20banking%20app%20(savibgs%20goal)%20mo%20background.png" alt="Savings App">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/Create%20a%20banking%20app%20(transactions%20screen)%20no%20background.png" alt="Transactions App">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/Create%20three%20banking%20(1st%20image)%20no%20background.png" alt="Banking App">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/put%20the%20red%20corvette%20iphone%20frame%20no%20frame.png" alt="Red Corvette App">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/put%20these%20two%20photos%20tesla%20iphone%20frame%20no%20background.png" alt="Tesla App">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/render%20the%20visual%20wi%20latest%20design%20(no%20background).jpg" alt="Latest Design">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/use%20square%20widgets%20ubest%20one%20(no%20backround).jpg" alt="Square Widgets">
      <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/put%20this%20photo%20in%20an%20fruit%20ad%20iphone%20frame%20no%20background.png" alt="Fruit Ad">
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <h2>Contact Me</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Your Message"></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <!-- AI HELP BOT -->
  <div id="ai-bot">
    <div id="ai-bot-header">AI Help Bot</div>
    <div id="ai-bot-messages"></div>
    <input id="ai-bot-input" placeholder="Ask me something...">
  </div>

  <script>
    // CRM Reader effect
    document.addEventListener('DOMContentLoaded', () => {
      const reader = document.getElementById('reader');
      const text = `Business is something that comes in all different shapes and sizes. If there's one thing man can't measure it's talent, but it doesn't hurt to try! Honestly though, with this app it isn't anything out of the ordinary. It is just an attempt to see if I could make some hits where others have had misses. I wanted to see if I could use this tool to provide any level of assistance or increased provision to daily the hustle and bustle of a businessman in the fast-paced sales and marketing world. With this app there are various improved enhancements regarding tracking teams and clientele.`;

      const words = text.split(' ');
      reader.innerHTML = '';
      words.forEach(word => {
        const span = document.createElement('span');
        span.textContent = word + ' ';
        reader.appendChild(span);
      });

      let index = 0;
      const spans = reader.querySelectorAll('span');
      let timer;

      function highlightWord() {
        if (index > 0) spans[index - 1].classList.remove('active');
        if (index < spans.length) {
          spans[index].classList.add('active');
          index++;
          timer = setTimeout(highlightWord, 350);
        }
      }

      function resetReader() {
        clearTimeout(timer);
        spans.forEach(span => span.classList.remove('active'));
        index = 0;
        highlightWord();
      }

      highlightWord();
      reader.addEventListener('mouseenter', resetReader);
    });

    // AI Bot simple echo
    const botInput = document.getElementById('ai-bot-input');
    const botMessages = document.getElementById('ai-bot-messages');
    botInput.addEventListener('keypress', (e) => {
      if (e.key === 'Enter' && botInput.value.trim() !== '') {
        const userMsg = document.createElement('div');
        userMsg.textContent = "You: " + botInput.value;
        botMessages.appendChild(userMsg);

        const botReply = document.createElement('div');
        botReply.textContent = "Bot: " + "I heard \"" + botInput.value + "\"";
        botMessages.appendChild(botReply);

        botInput.value = '';
        botMessages.scrollTop = botMessages.scrollHeight;
      }
    });
  </script>
</body>
</html>


