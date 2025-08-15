<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Homepage with Spline Intro</title>
<style>
    html, body {
        margin: 0;
        padding: 0;
        height: 100%;
        overflow: hidden; /* Prevent scrolling initially */
        font-family: Arial, sans-serif;
    }

    /* Fullscreen intro */
    #intro {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: 10;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        background: #000; /* fallback background */
    }

    spline-viewer {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: 1;
    }

    #enterBtn {
        position: relative;
        z-index: 2;
        padding: 15px 30px;
        font-size: 1.2rem;
        background-color: forestgreen;
        color: white;
        border: none;
        border-radius: 8px;
        cursor: pointer;
        transition: background-color 0.3s ease;
    }

    #enterBtn:hover {
        background-color: #2e7d32;
    }

    /* Rest of the page */
    #mainContent {
        min-height: 200vh;
        background: linear-gradient(#fff, #ddd);
        padding: 40px;
    }

    /* Slide effect when unlocking scroll */
    .unlock-scroll {
        overflow: auto;
        scroll-behavior: smooth;
    }
</style>
</head>
<body>

<!-- INTRO FULLSCREEN SPLINE -->
<div id="intro">
    <script type="module" src="https://unpkg.com/@splinetool/viewer@1.10.44/build/spline-viewer.js"></script>
    <spline-viewer url="https://prod.spline.design/EBbJDLbOuItb8tLY/scene.splinecode"></spline-viewer>
    <button id="enterBtn">Enter Here</button>
</div>
<script>
  (function () {
    const intro = document.getElementById('intro');
    const btn = document.getElementById('enterBtn');
    const main = document.getElementById('mainContent');

    if (btn && intro && main) {
      btn.addEventListener('click', () => {
        // re-enable page scrolling
        document.body.style.overflow = 'auto';

        // fade out & then remove the fixed intro overlay
        intro.style.transition = 'opacity 500ms ease';
        intro.style.opacity = '0';
        setTimeout(() => { intro.style.display = 'none'; }, 500);

        // scroll to your main content
        main.scrollIntoView({ behavior: 'smooth' });
      });
    }
  })();
</script>

<!-- MAIN PAGE CONTENT -->
<div id="mainContent">
<div class="sw-logo-container">
  <div class="sw-logo">SW</div>
  <div class="sw-words fade-in" id="sw-word" aria-live="polite">Marketing</div>
</div>

<style>
  .sw-logo-container {
    display: flex;
    align-items: center;
    gap: 2rem;
    font-family: Impact, sans-serif;
    padding: 3rem;
    background: linear-gradient(to right, #f8f8f8, #eaeaea);
  }

  .sw-logo {
    font-size: 20rem;
    color: hsl(94, 100%, 20%);
    font-weight: bold;
    transform: skewX(-10deg);
    transition: transform 0.6s ease, text-shadow 0.6s ease;
    text-shadow:
      0 4px 6px rgba(0, 0, 0, 0.2),
      0 8px 20px rgba(0, 128, 0, 0.3),
      inset 0 0 10px rgba(255, 255, 255, 0.2);
  }

  .sw-logo:hover {
    transform: scale(1.05) skewX(-10deg);
    text-shadow:
      0 6px 12px rgba(0, 0, 0, 0.3),
      0 12px 30px rgba(0, 128, 0, 0.4),
      inset 0 0 15px rgba(255, 255, 255, 0.3);
  }

  .sw-words {
    font-size: 3rem;
    color: black;
    opacity: 0;
    transition: opacity 0.5s ease;
    font-style: ;
  }

  .sw-words.fade-in {
    opacity: 1;
  }
</style>

<script>
  const words = [
    "UX/IX",
    "HTML",
    "CSS",
    "Javascript",
    "Java",
    "SQL",
    "Power BI",
    "Front-end Developer",
    "Marketing",
    "Microsoft Azure Cloud Specialist",
    "Design",
    "Graphic Design & Animation",
    "Sales",
    "AI Automation and Development",
    "Cyber Security"
  ];

  let index = 0;
  const wordElement = document.getElementById("sw-word");

  function showNextWord() {
    wordElement.classList.remove("fade-in");
    setTimeout(() => {
      index = (index + 1) % words.length;
      wordElement.textContent = words[index];
      wordElement.classList.add("fade-in");
    }, 500);
  }

  setInterval(showNextWord, 3000);
</script>

<script>
  const words = [
    "UX/IX",
    "HTML",
    "CSS",
    "Javascript",
    "Java",
    "SQL",
    "Power BI",
    "Front-end Developer",
    "Marketing",
    "Microsoft Azure Cloud Specialist",
    "Design",
    "Graphic Design & Animation",
    "Sales",
    "AI Automation and Development",
    "Cyber Security"
  ];

  let index = 0;
  const wordElement = document.getElementById("sw-word");

  function showNextWord() {
    wordElement.classList.remove("fade-in");
    setTimeout(() => {
      index = (index + 1) % words.length;
      wordElement.textContent = words[index];
      wordElement.classList.add("fade-in");
    }, 500);
  }

  setInterval(showNextWord, 3000);
</script>

<script>
  const words = [
    "UX/IX",
    "HTML",
    "CSS",
    "Javascript",
    "Java",
    "SQL",
    "Power BI",
    "Front-end Developer",
    "Marketing",
    "Microsoft Azure Cloud Specialist",
    "Design",
    "Graphic Design & Animation",
    "Sales",
    "AI Automation and Development",
    "Cyber Security"
  ];

  let index = 0;
  const wordElement = document.getElementById("sw-word");

  function showNextWord() {
    wordElement.classList.remove("fade-in");
    setTimeout(() => {
      index = (index + 1) % words.length;
      wordElement.textContent = words[index];
      wordElement.classList.add("fade-in");
    }, 500);
  }

  setInterval(showNextWord, 3000);
</script>


<!-- PORTFOLIO THUMBNAILS -->
<div class="portfolio-container">
 
  <a class="thumbnail" href="https://swmarketingfirm.blogspot.com/p/choose-one-body-margin-0-font-family.html" target="_blank">
    <div class="icon"><i class="fas fa-file alt"></i></div>
    <div class="label">UX/IX Designs</div>
  </a>
  <a class="thumbnail" href="https://github.com/SWMarketingTech/SWFiles/tree/main" target="_blank">
    <div class="icon"><i class="fas fa-code"></i></div>
    <div class="label">Software Development</div>
  </a>
  <a class="thumbnail" href="https://www.dropbox.com/home/Sample%20Writings" target="_blank">
    <div class="icon"><i class="fas fa-pen-nib"></i></div>
    <div class="label">Professional Writings</div>
  </a>
  <a class="thumbnail" href="https://www.dropbox.com/home/Financial%20Work" target="_blank">
    <div class="icon"><i class="fas fa-chart-line"></i></div>
    <div class="label">Financial Projects</div>
  </a>
  <a class="thumbnail" href="https://www.dropbox.com/home/Data%20Analytics" target="_blank">
    <div class="icon"><i class="fas fa-database"></i></div>
    <div class="label">Data Analytics</div>
  </a>
  <a class="thumbnail" href="https://www.dropbox.com/home/Business%20Presentations" target="_blank">
    <div class="icon"><i class="fas fa-chalkboard"></i></div>
    <div class="label">Presentations</div>
  </a>
</div>

</div>

<script>
    const enterBtn = document.getElementById('enterBtn');
    const intro = document.getElementById('intro');

    enterBtn.addEventListener('click', () => {
        // Unlock scroll
        document.body.classList.add('unlock-scroll');

        // Smooth scroll to the next section
        document.getElementById('mainContent').scrollIntoView({ behavior: 'smooth' });

        // Hide intro after transition
        setTimeout(() => {
            intro.style.display = 'none';
        }, 1000);
    });
</script>

</body>
</html>

<!-- AI HELP BOT -->
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AI Help Pop-Up</title>
  <style>
    body {
      margin: 0;
      font-family: sans-serif;
    }

    .ai-help-button {
      position: fixed;
      bottom: 20px;
      left: 20px;
      background-color: #0078d4;
      color: white;
      padding: 10px 15px;
      border-radius: 8px;
      cursor: pointer;
      z-index: 1000;
    }

    .ai-popup-wrapper {
      position: fixed;
      bottom: 80px;
      left: 20px;
      display: none;
      z-index: 999;
    }

    .bubble-container {
      position: absolute;
      bottom: 110px;
      left: 0;
      display: flex;
      flex-direction: column;
      gap: 6px;
      pointer-events: auto;
    }

    .bubble {
      background-color: forestgreen;
      color: white;
      padding: 6px 10px;
      border-radius: 12px;
      font-size: 0.7rem;
      white-space: nowrap;
      cursor: pointer;
      text-align: center;
    }

    .ai-popup {
      width: 100px;
      height: 100px;
      background: white;
      border-radius: 20px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
    }

    .ai-popup video {
      position: absolute;
      width: 120%;
      height: 120%;
      object-fit: cover;
      object-position: center top;
      border-radius: 20px;
      pointer-events: auto;
      transform: scale(1.1);
      z-index: 1;
    }

    .ai-popup audio {
      display: none;
    }

    .ai-popup-close {
      position: absolute;
      top: 4px;
      right: 8px;
      font-size: 1.2rem;
      cursor: pointer;
      color: #0078d4;
      z-index: 1002;
    }

    .subtitle {
      position: absolute;
      bottom: 6px;
      left: 50%;
      transform: translateX(-50%);
      width: 90%;
      text-align: center;
      font-size: 0.65rem;
      font-weight: bold;
      color: #ffeb3b;
      text-shadow: 1px 1px 2px black;
      z-index: 1003;
      pointer-events: none;
    }
  </style>
</head>
<body>

  <div class="ai-help-button" onclick="togglePopup()">Need AI Help?</div>

  <div class="ai-popup-wrapper" id="aiPopupWrapper">
    <div class="bubble-container">
      <div class="bubble" onclick="handleBubbleClick('Contact SW')">Contact SW</div>
      <div class="bubble" onclick="handleBubbleClick('Portfolio Library')">Portfolio Library</div>
      <div class="bubble" onclick="handleBubbleClick('CRM APP (Prologue)')">CRM APP (Prologue)</div>
    </div>

    <div class="ai-popup" id="aiPopup">
      <div class="ai-popup-close" onclick="togglePopup()">✖</div>

      <video id="aiVideo" autoplay muted loop disablePictureInPicture controlsList="nodownload">
        <source src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/yt1z.net%20-%20World%20s%20first%20AI%20presenter%20unveiled%20in%20China%20(144p).mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>

      <audio id="aiVoiceover">
        <source src="https://github.com/SWMarketingTech/SWFiles/blob/main/Vocalized%20by%20Adam%20Elevenlabs%20-%20theaivoicegenerator.com%20-%202025-08-14.mp3?raw=true" type="audio/mpeg">
        Your browser does not support the audio tag.
      </audio>

      <div class="subtitle" id="subtitleText"></div>
    </div>
  </div>

  <script>
    const subtitles = [
      { time: 0, text: "Welcome to the SW Portfolio Showroom." },
      { time: 3, text: "I’ll be your AI Help Assistant." },
      { time: 6, text: "You can select an option or type in your search below." },
      { time: 10, text: "If I can't assist, your request will be forwarded to SW." },
      { time: 13, text: "They’ll reply promptly and professionally." }
    ];

    let subtitleInterval;

    function togglePopup() {
      const wrapper = document.getElementById("aiPopupWrapper");
      const video = document.getElementById("aiVideo");
      const voiceover = document.getElementById("aiVoiceover");
      const subtitleText = document.getElementById("subtitleText");

      if (wrapper.style.display === "none" || wrapper.style.display === "") {
        wrapper.style.display = "block";

        video.addEventListener('loadedmetadata', () => {
          video.currentTime = 8;
        }, { once: true });

        voiceover.currentTime = 0;
        voiceover.play();

        subtitleText.textContent = "";
        let index = 0;
        subtitleInterval = setInterval(() => {
          const currentTime = voiceover.currentTime;
          if (index < subtitles.length && currentTime >= subtitles[index].time) {
            subtitleText.textContent = subtitles[index].text;
            index++;
          }
        }, 500);
      } else {
        wrapper.style.display = "none";
        video.pause();
        video.currentTime = 0;
        voiceover.pause();
        voiceover.currentTime = 0;
        clearInterval(subtitleInterval);
        document.getElementById("subtitleText").textContent = "";
      }
    }

    function handleBubbleClick(label) {
      console.log(`Bubble clicked: ${label}`);
      // Add custom logic here if needed
    }
  </script>

</body>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
 body {
  font-family: 'Segoe UI', Tahoma, sans-serif;
  background-color: transparent !important;
  background-image: none !important;
  color: white;
  margin: 0;
  padding: 0;
}



  .portfolio-header {
    background-color: #145214;
    color: white
    overflow: visible;
    padding: 60px 0;
    text-align: center;
    font-size: 40px;
    font-weight: 700;
    border-bottom: 10px solid #ffffff;
  }

  .typewriter-text {
    display: inline-block;
    overflow: hidden;
    white-space: nowrap;
    border-right: 3px solid #fff;
    width: 0;
    animation: typing 2.5s steps(30, end) forwards, blink 0.7s step-end infinite;
    text-shadow: 3px 3px 6px rgba(0,0,0,0.8);
  }

  @keyframes typing {
    from { width: 0 }
    to { width: 23ch; }
  }

  @keyframes blink {
    50% { border-color: transparent; }
  }

  .portfolio-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 30px;
    padding: 40px 20px;
    max-width: 1200px;
    margin: auto;
  }

  .thumbnail {
    width: 220px;
    height: 220px;
    background-color: #2f4f2f;
    border-radius: 16px;
    box-shadow: 0 6px 12px rgba(0,0,0,0.4);
    transition: transform 0.3s ease, background-color 0.3s ease;
    cursor: pointer;
    text-decoration: none;
    color: white;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .thumbnail:hover {
    transform: translateY(-10px) scale(1.05);
    background-color: #3cb371;
  }

  .icon {
    font-size: 54px;
    margin-bottom: 14px;
    color: #ffffff;
    transition: color 0.3s;
  }

  .thumbnail:hover .icon {
    color: #fffacd;
  }

  .label {
    font-weight: 600;
    font-size: 17px;
    padding: 0 10px;
    text-align: center;
  }

  .contact-wrapper {
    background-color: #1b4e1b;
    padding: 60px 20px;
    margin-top: 60px;
    text-align: center;
    overflow: visible;
  }

  .contact-form {
    opacity: 0;
    transform: translateY(40px);
    transition: all 0.8s ease;
    max-width: 600px;
    margin: 0 auto;
    display: grid;
    gap: 20px;
    pointer-events: none;
  }

  .contact-wrapper:hover .contact-form {
    opacity: 1;
    transform: translateY(0);
    pointer-events: auto;
  }

  .contact-wrapper h2 {
    font-size: 32px;
    margin-bottom: 30px;
  }

  input, textarea {
    padding: 12px 14px;
    border: none;
    border-radius: 8px;
    font-size: 16px;
  }

  textarea {
    resize: vertical;
    min-height: 120px;
  }

  button {
    padding: 14px;
    background-color: #3cb371;
    border: none;
    border-radius: 8px;
    color: white;
    font-size: 18px;
    font-weight: bold;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }

  button:hover {
    background-color: #2e8b57;
  }

  .skills-section {
    background-color: #1b4e1b;
    color: white;
    padding: 60px 20px;
    max-width: 900px;
    margin: auto;
    font-family: 'Segoe UI', Tahoma, sans-serif;
  }

  .skills-section h2 {
    font-size: 28px;
    margin-bottom: 40px;
    text-align: center;
  }

  .skill {
    display: flex;
    align-items: center;
    margin-bottom: 20px;
    flex-wrap: wrap;
  }

  .skill-name {
    flex: 1 1 150px;
    font-weight: 600;
    font-size: 16px;
  }

  .bar {
    flex: 1 1 60%;
    background-color: #3a5f3a;
    height: 18px;
    border-radius: 10px;
    overflow: hidden;
    margin: 0 15px;
    position: relative;
  }

  .fill {
    height: 100%;
    background-color: #3cb371;
    width: 0;
    animation: fillBar 2s ease-out forwards;
  }

  .percent {
    font-family: monospace;
    min-width: 40px;
    font-size: 16px;
  }

  @keyframes fillBar {
    from { width: 0; }
  }

  @media (max-width: 600px) {
    .thumbnail {
      width: 100%;
      max-width: 280px;
    }

    .portfolio-container {
      flex-direction: column;
      align-items: center;
    }

    .skill {
      flex-direction: column;
      align-items: flex-start;
    }

    .bar {
      width: 100%;
      margin: 10px 0;
    }

    .percent {
      align-self: flex-end;
    }
  }
</style>

<script>
    const enterBtn = document.getElementById('enterBtn');
    const intro = document.getElementById('intro');
    const main = document.getElementById('main');

    enterBtn.addEventListener('click', () => {
      intro.style.transition = 'transform 1s ease-in-out';
      intro.style.transform = 'translateY(-100%)';
      setTimeout(() => {
        intro.style.display = 'none';
      }, 1000);
    });
  </script>

<!-- HEADER SECTION -->
<div class="blog-name container">
  <div class="container section" id="header" name="Header">
    <div class="widget Header" data-version="2" id="Header1">
      <div class="header-widget">
        <div>
          
<h1>
  <a href="https://swmarketingfirm.blogspot.com/" class="portfolio-link">
    <span class="sw-text">SW</span>  <span class="loading-counter"></span>
  </a>
</h1>
   
         

        </div>
        <p></p>
      </div>
    </div>
  </div>

  <nav role="navigation">
    <div class="clearboth no-items section" id="page_list_top" name="Page List (Top)">
    </div>
  </nav>
</div>
<style>
.portfolio-link {
  color: white;
  text-decoration: none;
  font-size: 28px;
  display: inline-block;
  transition: color 0.3s ease;
}

.portfolio-link:hover {
  color: #ddd;
}

.sw-text {
  font-family: 'Amasis MT Pro Black', Georgia, serif; /* Fallbacks included */
  color: #145214; /* Forest green */
  font-size: 43px;
  font-weight: bold;
  margin-right: 6px;
}

.loading-counter {
  font-family: monospace;
  font-size: 16px;
  color: #ffffff;
  margin-left: 10px;
  visibility: hidden;
}
  

<!-- STICKY HEADER STYLING -->
<style>
  .blog-name.container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 9999;
    background-color: rgba(20, 82, 20, 0.95); /* Forest green semi-transparent */
    padding: 20px 0;
    text-align: center;
    box-shadow: 0 3px 6px rgba(0, 0, 0, 0.3);
  }

  .blog-name.container h1 {
    margin: 0;
    padding: 0;
    font-size: 32px;
    font-weight: bold;
    line-height: 1.2;
  }

  .portfolio-link {
    color: white;
    text-decoration: none;
    font-size: 28px;
    display: inline-block;
    transition: color 0.3s ease;
  }

  .portfolio-link:hover {
    color: #ddd;
  }

  .sw-text {
    font-family: 'Amasis MT Pro Black', serif;
    color: #145214; /* Forest green */
    font-size: 38px;
    font-weight: bold;
    margin-right: 6px;
  }

  .loading-counter {
    font-family: monospace;
    font-size: 16px;
    color: #ffffff;
    margin-left: 10px;
    visibility: hidden;
  }

  /* Ensure space for fixed header */
  #main {
    padding-top: 100px;
  }
</style>

<!-- LOADING COUNTER SCRIPT -->
<script>
  const swLink = document.querySelector('.portfolio-link');
  const counter = document.querySelector('.loading-counter');

  swLink.addEventListener('mouseenter', () => {
    let count = 0;
    const target = 100;

    counter.style.visibility = 'visible';
    counter.innerText = "0%";

    const load = () => {
      if (count < target) {
        count++;
        counter.innerText = count + "%";
        setTimeout(load, 15);
      } else {
        counter.innerText = "100%";
      }
    };

    load();
  });

  swLink.addEventListener('mouseleave', () => {
    counter.style.visibility = 'hidden';
    counter.innerText = "";
  });
</script>

<!-- STYLE OVERRIDES -->
<style>
  .blog-name.container {
    background-color: transparent !important;
    padding: 0 !important;
    margin: 0 auto;
    text-align: center;
    position: relative;
    z-index: 10;
  }

  .blog-name.container h1 {
    margin: 0;
    padding: 20px 0;
    font-size: 32px;
    font-weight: bold;
    line-height: 1.2;
    transition: none !important;
  }

  .blog-name.container a {
    color: white; /* Change if needed */
    text-decoration: none;
  }

  .blog-name.container a:hover {
    color: #ccc;
  }

  .header-widget {
    background: transparent !important;
    box-shadow: none !important;
    padding: 0;
  }

  .container.section#header,
  .widget.Header {
    margin: 0;
    padding: 0;
  }

  nav {
    margin-top: 0;
    padding-top: 0;
  }

  /* Optional: Add subtle fade-in if you want */
  .blog-name.container h1 {
    animation: fadeIn 1s ease-in-out;
  }

  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(-10px); }
    to { opacity: 1; transform: translateY(0); }
  }
</style>




<!-- TECHNICAL SKILLS SECTION -->
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Skills Section</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background-color: #f5f5f5;
      font-family: 'Segoe UI', Tahoma, sans-serif;
    }

    .skills-section {
      background-color: transparent;
      color: #228B22; /* Forest green */
      padding: 60px 20px;
      max-width: 900px;
      margin: auto;
      font-family: 'Segoe UI', Tahoma, sans-serif;
      perspective: 1000px;
      transition: transform 0.2s ease;
    }

    .skills-header {
      font-size: 34px;
      font-weight: bold;
      margin-bottom: 10px;
      text-align: center;
      text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
      color: #228B22;
    }

    .skills-section h2 {
      font-size: 26px;
      margin-bottom: 40px;
      text-align: center;
      color: #228B22;
    }

    .skill {
      margin-bottom: 20px;
    }

    .skill-name {
      color: #228B22;
      font-weight: bold;
    }

    .bar {
      width: 100%;
      height: 20px;
      background-color: #eee;
      border-radius: 10px;
      overflow: hidden;
    }

    .fill {
      height: 100%;
      width: 0;
      background-color: #3cb371;
      transition: width 2s ease-in-out;
      border-radius: 10px;
    }

    .percent {
      margin-left: 10px;
      font-weight: bold;
      color: #228B22;
    }

    @media (max-width: 600px) {
      .skill {
        flex-direction: column;
        align-items: flex-start;
      }

      .bar {
        width: 100%;
        margin: 10px 0;
      }

      .percent {
        align-self: flex-end;
      }
    }
  </style>
</head>
<body>

  <!-- TECHNICAL SKILLS SECTION -->
  <div class="skills-section" id="skills-trigger">
    <h1 class="skills-header">What SW Specializes In...</h1>
    <h2>Technical Skills</h2>

    <div class="skill">
      <span class="skill-name">HTML &amp; CSS</span>
      <div class="bar"><div class="fill" data-width="90%"></div></div>
      <span class="percent" data-target="90">0%</span>
    </div>

    <div class="skill">
      <span class="skill-name">JavaScript</span>
      <div class="bar"><div class="fill" data-width="80%"></div></div>
      <span class="percent" data-target="80">0%</span>
    </div>

    <div class="skill">
      <span class="skill-name">Python</span>
      <div class="bar"><div class="fill" data-width="85%"></div></div>
      <span class="percent" data-target="85">0%</span>
    </div>

    <div class="skill">
      <span class="skill-name">SQL</span>
      <div class="bar"><div class="fill" data-width="75%"></div></div>
      <span class="percent" data-target="75">0%</span>
    </div>

    <div class="skill">
      <span class="skill-name">Power BI</span>
      <div class="bar"><div class="fill" data-width="88%"></div></div>
      <span class="percent" data-target="88">0%</span>
    </div>
  </div>

  <script>
    // Animate skills on hover
    function enableHoverSkillAnimation(sectionId) {
      const section = document.getElementById(sectionId);
      const skills = section.querySelectorAll(".skill");

      section.addEventListener("mouseenter", () => {
        skills.forEach(skill => {
          const fill = skill.querySelector(".fill");
          const percent = skill.querySelector(".percent");

          // Reset first
          fill.style.width = "0%";
          percent.innerText = "0%";

          const targetWidth = fill.dataset.width;
          const target = parseInt(percent.dataset.target);

          setTimeout(() => {
            // Animate fill
            fill.style.width = targetWidth;

            // Animate counter
            let count = 0;
            const updateCount = () => {
              if (count <= target) {
                percent.innerText = count + "%";
                count++;
                setTimeout(updateCount, 20);
              }
            };
            updateCount();
          }, 100);
        });
      });

      section.addEventListener("mouseleave", () => {
        skills.forEach(skill => {
          const fill = skill.querySelector(".fill");
          const percent = skill.querySelector(".percent");

          fill.style.width = "0%";
          percent.innerText = "0%";
        });
      });
    }

    enableHoverSkillAnimation("skills-trigger");

    // Add 3D tilt effect
    const section = document.getElementById("skills-trigger");

    section.addEventListener("mousemove", (e) => {
      const { width, height, left, top } = section.getBoundingClientRect();
      const x = e.clientX - left;
      const y = e.clientY - top;

      const rotateX = ((y / height) - 0.5) * 10;
      const rotateY = ((x / width) - 0.5) * -10;

      section.style.transform = `rotateX(${rotateX}deg) rotateY(${rotateY}deg)`;
    });

    section.addEventListener("mouseleave", () => {
      section.style.transform = `rotateX(0deg) rotateY(0deg)`;
    });
  </script>

</body>




<!-- SOFT SKILLS SECTION -->
<div class="skills-section" id="softskills-trigger">
  <h1 class="skills-header">Soft Skills</h1>
  <h2>What SW Delivers Interpersonally</h2>

  <div class="skill">
    <span class="skill-name">Communication</span>
    <div class="bar"><div class="fill" data-width="100%"></div></div>
    <span class="percent" data-target="100">0%</span>
  </div>

  <div class="skill">
    <span class="skill-name">Presentations</span>
    <div class="bar"><div class="fill" data-width="95%"></div></div>
    <span class="percent" data-target="95">0%</span>
  </div>

  <div class="skill">
    <span class="skill-name">Team Collaboration</span>
    <div class="bar"><div class="fill" data-width="92%"></div></div>
    <span class="percent" data-target="92">0%</span>
  </div>

  <div class="skill">
    <span class="skill-name">Problem Solving</span>
    <div class="bar"><div class="fill" data-width="90%"></div></div>
    <span class="percent" data-target="90">0%</span>
  </div>

  <div class="skill">
    <span class="skill-name">Adaptability</span>
    <div class="bar"><div class="fill" data-width="93%"></div></div>
    <span class="percent" data-target="93">0%</span>
  </div>
</div>

<script>
  function enableHoverSkillAnimation(sectionId) {
    const section = document.getElementById(sectionId);
    const skills = section.querySelectorAll(".skill");

    section.addEventListener("mouseenter", () => {
      skills.forEach(skill => {
        const fill = skill.querySelector(".fill");
        const percent = skill.querySelector(".percent");

        // Reset first
        fill.style.width = "0%";
        percent.innerText = "0%";

        const targetWidth = fill.dataset.width;
        const target = parseInt(percent.dataset.target);

        setTimeout(() => {
          // Animate fill
          fill.style.width = targetWidth;

          // Animate counter
          let count = 0;
          const updateCount = () => {
            if (count <= target) {
              percent.innerText = count + "%";
              count++;
              setTimeout(updateCount, 20);
            }
          };
          updateCount();
        }, 100); // Slight delay ensures the reset is visible
      });
    });

    section.addEventListener("mouseleave", () => {
      skills.forEach(skill => {
        const fill = skill.querySelector(".fill");
        const percent = skill.querySelector(".percent");

        // Reset everything
        fill.style.width = "0%";
        percent.innerText = "0%";
      });
    });
  }

  enableHoverSkillAnimation("skills-trigger");
  enableHoverSkillAnimation("softskills-trigger");
</script>

<!-- Message to the Audience -->

<section id="sw-portfolio-section" style="width: 100%; height: 300px; display: flex; align-items: center; justify-content: center; background-color: #fff; color: #000; font-family: 'Segoe UI', sans-serif; padding: 2rem;">
  <style>
    #sw-portfolio-section .type-container {
      font-size: 1.2rem;
      max-width: 700px;
      line-height: 1.6;
      letter-spacing: 0.5px;
      border-left: 3px solid #000;
      padding-left: 1rem;
      white-space: pre-wrap;
      min-height: 150px;
    }
  </style>

  <div class="type-container" id="autoText"></div>

  <script>
    const typeTarget = document.getElementById("autoText");
    const message = "Welcome to the SW Portfolio page. This isn't a formal site. It's just a bulletin board to put out different concepts and designs. This allows the audience to see a range of styles and capabilities. But honestly..................... there's nothing that can't be done here!";
    let interval;

    function autoType() {
      clearInterval(interval);
      typeTarget.textContent = "";
      let index = 0;
      interval = setInterval(() => {
        if (index < message.length) {
          typeTarget.textContent += message.charAt(index);
          index++;
        } else {
          clearInterval(interval);
        }
      }, 45);
    }

    document.getElementById("sw-portfolio-section").addEventListener("mouseenter", autoType);
  </script>
</section>

<!-- Think Bigger Webpage AD -->
<div class="think-bigger-wrapper">
  <section id="think-bigger-section">
    <style>
      .think-bigger-wrapper {
        opacity: 0;
        transform: scale(0.6);
        transition: opacity 1s ease-out, transform 1s ease-out;
        will-change: opacity, transform;
      }

      .think-bigger-wrapper.visible {
        opacity: 1;
        transform: scale(1);
      }

      #think-bigger-section {
        width: 100%;
        height: 100%;
        background-color: black;
        color: white;
        font-family: 'Segoe UI', sans-serif;
        overflow-x: hidden;
        padding: 4rem 1rem;
      }

      #think-bigger-section header {
        text-align: center;
        font-size: 6rem;
        font-weight: bold;
        color: white;
        text-shadow: 3px 3px 0 #444, -1px -1px 0 #888;
        letter-spacing: 2px;
        margin-bottom: 2rem;
      }

      #think-bigger-section .banner {
        display: flex;
        align-items: center;
        justify-content: center;
        position: relative;
        max-width: 1200px;
        margin: 0 auto;
      }

      .product-image {
        width: 800px;
        height: auto;
        border-radius: 10px;
        box-shadow: 0 0 30px rgba(255, 255, 255, 0.1);
        transition: transform 0.3s ease;
      }

      .product-description {
        position: absolute;
        left: 0;
        top: 50%;
        transform: translateY(-50%);
        width: 300px;
        background-color: rgba(0, 0, 0, 0.75);
        padding: 1rem;
        border-radius: 8px;
        opacity: 0;
        transition: opacity 0.3s ease;
        pointer-events: none;
      }

      .banner:hover .product-description {
        opacity: 1;
        pointer-events: auto;
      }

      .product-image:hover {
        transform: scale(1.03);
      }
    </style>

    <header><span>Think Bigger</span></header>

    <div class="banner">
      <img class="product-image" src="https://dlcdnwebimgs.asus.com/files/media/cf9d4ac3-7540-4386-a70a-abcc28e23c2b/v1/features/images/large/1x/kv.jpg" alt="Product Image">
      <div class="product-description">
        <h2>ZT Book Pro XL</h2>
        <p>
          Experience dual-screen productivity with cutting-edge design. Powered by Intel Core and NVIDIA graphics, this laptop redefines creative performance.
        </p>
      </div>
    </div>
  </section>
</div>

<script>
  const wrapper = document.querySelector(".think-bigger-wrapper");

  const observer = new IntersectionObserver(
    ([entry]) => {
      if (entry.isIntersecting) {
        wrapper.classList.add("visible");
      } else {
        wrapper.classList.remove("visible");
      }
    },
    { threshold: 0.3 }
  );

  observer.observe(wrapper);
</script>


<!-- CRM APP -->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>CRM App Showcase</title>
  <style>
    body {
      background: #f4f4f4;
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
    }

    #crm-section {
      position: relative;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 0;
      margin: 0;
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
      color: black;
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
      background-color: transparent;
      border: 2px solid rgba(0, 0, 0, 0);
      border-radius: 40px;
      box-shadow: 0 0 0 rgba(0, 0, 0, 0);
      display: flex;
      justify-content: center;
      align-items: center;
      animation: floatRotate 6s infinite ease-in-out;
      transform-style: preserve-3d;
      overflow: visible;
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

    .info-button:hover {
      background-color: darkgreen;
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
  </style>
</head>
<body>

  <section id="crm-section">
    <div class="crm-header">
      <img src="https://github.com/SWMarketingTech/SWFiles/blob/main/CRM%20APP%20Logo%202.jpg?raw=true" alt="CRM Logo" />
      CRM App
    </div>

    <div class="crm-content">
      <div class="phone-container">
        <div class="screen">
          <img src="https://github.com/SWMarketingTech/SWFiles/blob/main/nobackground%20cutout%20.png?raw=true" alt="CRM App Interface">
        </div>
      </div>

      <a class="info-button" href="https://github.com/SWMarketingTech/SWFiles/tree/main/CRMDaily" target="_blank">
        More Info
      </a>

      <div class="reader-effect" id="reader"></div>
    </div>
  </section>

  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const reader = document.getElementById('reader');
      const text = `Business is something that comes in all different shapes and sizes. If there's one thing man can't measure it's talent, but it doesn't hurt to try! Honestly though, with app it isn't anything out of the ordinary but just an attempt to see if I could make some hits where others have had misses. I wanted to see if I could use this tool to provide any level of assistance or increased provision to daily hustle and bustle of a businessman in the fast-paced sales and marketing world. With this app there are various improved enhancements regarding tracking teams and clientele.`;

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
  </script>

</body>


<!-- CONTACT FORM -->
<div class="contact-wrapper">
  <h2>Contact SW Marketing</h2>
  <form class="contact-form" action="mailto:swmarketingfirm@gmail.com" method="post" enctype="text/plain">
    <input type="text" name="Name" placeholder="Your Name" required>
    <input type="email" name="Email" placeholder="Your Email" required>
    <input type="tel" name="Phone" placeholder="Your Phone Number" required>
    <textarea name="Message" placeholder="Your Message..." required></textarea>
    <button type="submit">Send Message</button>
  </form>
</div>

<!-- SW Watermark -->
<div id="watermark-container">
  <img src="https://raw.githubusercontent.com/SWMarketingTech/SWFiles/main/SW%20The%20Logo.jpg" alt="SW Logo" />
</div>

<style>
  #watermark-container {
    position: fixed;
    bottom: 20px;
    right: 20px;
    width: 180px;
    height: 80px;
    z-index: 9999;
    pointer-events: none;
    justify-content: center;
    align-items: center;
    background: transparent;  
  }

  #watermark-container img {
    width: 250%;
    height: 200%;
    object-fit: contain;
    opacity: 0.94; /* Optional: make it semi-transparent */
  }
</style>


  
/* FULL TRANSPARENCY STYLES FOR MAIN PAGE AREA */
#main,
#page_body,
#Blog1,
.blog-posts,
.post-outer-container,
.post-outer,
.post,
.post-body,
.post-
  er,
.post-footer,
.comments,
.comment-form,
#comments,
#Blog1_comments-block-wrapper {
  background-color: transparent !important;
  box-shadow: none !important;
  border: none !important;
}

/* Optional: remove default margins/paddings */
#main,
#page_body,
.post-outer-container,
.post {
  margin: 0 !important;
  padding: 0 !important;
}

/* Make comment form + title area blend in */
.comment-form,
#comment-editor,
#comment-editor-src,
#comments h3.title,
#comment-post-message {
  background-color: transparent !important;
  color: white !important;
  border: none !important;
  box-shadow: none !important;
}

/* Optional: remove horizontal lines or borders from footers */
.post-footer-line,
.footer {
  background: none !important;
  border: none !important;
}

/* Optional: make sure embedded iframe has no background too */
.blogger-comment-from-post {
  background-color: transparent !important;
}

<style>
/* FORCE FULL PAGE TRANSPARENCY */
body,
html,
#main,
#page_body,
#Blog1,
.blog-posts,
.post-outer-container,
.post-outer,
.post,
.post-body,
.post-header,
.post-footer,
footer,
header,
#header,
#footer,
.centered-top,
.centered-top-container,
.centered-bottom,
.page_body {
  background-color: transparent !important;
  background-image: none !important;
  box-shadow: none !important;
  border: none !important;
}

<style>
  body {
    background-image: url('https://example.com/your-background.jpg');
    background-size: cover;
    background-attachment: fixed;
    background-repeat: no-repeat;
    background-position: center;
  }
</style>


<div>
<!-- STICKY HEADER -->
<div class="blog-name container">
  <div class="container section" id="header" name="Header">
    <div class="widget Header" data-version="2" id="Header1">
      <div class="header-widget">
        <div>
          <h1>
  <a href="https://swmarketingfirm.blogspot.com/" class="portfolio-link">
    <span class="sw-text"></span>  <span class="loading-counter"></span>
  </a>
</h1>
    
            
        </div>
        <p></p>
      </div>
    </div>
  </div>

  <nav role="navigation">
    <div class="clearboth no-items section" id="page_list_top" name="Page List (Top)">
    </div>
  </nav>
</div>
  
<style>
/* MAKE HEADER STICK TO TOP */
.blog-name.container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 9999;
  background-color: rgba(20, 82, 20, 0.95); /* Forest green semi-transparent */
  padding: 20px 0;
  text-align: center;
  box-shadow: 0 3px 6px rgba(0, 0, 0, 0.3);
}

/* Style the link inside the header */
.blog-name.container h1 {
  margin: 0;
  padding: 0;
  font-size: 32px;
  font-weight: bold;
}

.blog-name.container a {
  color: white;
  text-decoration: none;
  transition: color 0.3s ease;
}

.blog-name.container a:hover {
  color: #ccc;
}
