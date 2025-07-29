<!-- Font Awesome Icons -->
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
    color: white;
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

<!-- SLIDESHOW BULLETIN BOARD -->
<div id="slideshow-board" style="margin-top: 50px;">
  <h2 style="text-align: center;">📌 SW Bulletin Board</h2>
  <div class="slideshow-container">

    <div class="mySlides fade">
      <div class="slide-text">🎉 New AI Video Generator Project Coming Soon!</div>
    </div>

    <div class="mySlides fade">
      <div class="slide-text">📎 Portfolio updated with financial dashboard samples</div>
    </div>

    <div class="mySlides fade">
      <div class="slide-text">🧠 Tip of the Day: Simplify user journeys in data dashboards</div>
    </div>

  </div>

  <div style="text-align:center; margin-top: 10px;">
    <span class="dot"></span> 
    <span class="dot"></span> 
    <span class="dot"></span> 
  </div>
</div>

<style>
.slideshow-container {
  max-width: 1200px;
  height: 200px;
  position: relative;
  margin: 30px auto;
  border: 2px solid #ffffff;
  border-radius: 12px;
  background-color: #1b4e1b;
  padding: 20px;
  box-shadow: 0 0 20px rgba(0,0,0,0.4);
}

.mySlides {
  display: none;
  text-align: center;
}

.slide-text {
  font-size: 1.2rem;
  padding: 20px;
  color: #fffacd;
  font-weight: 600;
  text-shadow: 2px 2px 4px #000;
}

.fade {
  animation: fadeEffect 1.5s;
}

@keyframes fadeEffect {
  from {opacity: .4} 
  to {opacity: 1}
}

.dot {
  height: 12px;
  width: 12px;
  margin: 0 4px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.4s ease;
}

.active {
  background-color: #fffacd;
}

</style>

<script>
let slideIndex = 0;
showSlides();

function showSlides() {
  const slides = document.getElementsByClassName("mySlides");
  const dots = document.getElementsByClassName("dot");

  for (let i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }

  slideIndex++;
  if (slideIndex > slides.length) {slideIndex = 1}

  for (let i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }

  slides[slideIndex - 1].style.display = "block";
  dots[slideIndex - 1].className += " active";
  setTimeout(showSlides, 5000); // Change slide every 5 seconds
}
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

<style>
  .skills-section {
    background-color: #1b4e1b;
    color: white;
    padding: 60px 20px;
    max-width: 900px;
    margin: auto;
    font-family: 'Segoe UI', Tahoma, sans-serif;
  }

  .skills-header {
    font-size: 34px;
    font-weight: bold;
    margin-bottom: 10px;
    text-align: center;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.4);
  }

  .skills-section h2 {
    font-size: 26px;
    margin-bottom: 40px;
    text-align: center;
  }

.skill {
  margin-bottom: 20px;
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
  color: #fff;
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

<!-- SLIDE-IN RECTANGLE UNDER SOFT SKILLS -->

  <h2>CRM Daily App Preview (currently in development)</h2>

<div class="slide-hover-zone">
  <div class="slide-box-under" id="greenBoxUnder"></div>
</div>

<style>
  .slide-hover-zone {
    position: relative;
    height: 120px;
    margin-top: 40px;
    overflow: visible;
  }

  .slide-box-under {
    position: absolute;
    top: 0;
    left: -220px;
    width: 800px;
    height: 200px;
    background-color: #145214;
    transition: left 0.6s ease;
    border-radius: 0 10px 10px 0;
    box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.4);
    z-index: 10;
  }

  .slide-hover-zone:hover .slide-box-under {
    left: 0;
  }
</style>

<script>
  document.getElementById('softskills-trigger').addEventListener('mouseenter', () => {
    const skills = document.querySelectorAll("#softskills-trigger .skill");
    const fills = document.querySelectorAll("#softskills-trigger .fill");
    const counters = document.querySelectorAll("#softskills-trigger .percent");

    skills.forEach((skill, index) => {
      skill.classList.add("active");

      const fill = fills[index];
      const counter = counters[index];
      const targetWidth = fill.getAttribute("data-width");
      fill.style.width = targetWidth;

      const target = +counter.getAttribute("data-target");
      let count = 0;
      counter.innerText = "0%";

      const updateCount = () => {
        const speed = 20;
        if (count < target) {
          count++;
          counter.innerText = count + "%";
          setTimeout(updateCount, speed);
        } else {
          counter.innerText = target + "%";
        }
      };

      updateCount();
    });
  });

  document.getElementById('softskills-trigger').addEventListener('mouseleave', () => {
    document.querySelectorAll("#softskills-trigger .skill").forEach(skill => skill.classList.remove("active"));
    document.querySelectorAll("#softskills-trigger .fill").forEach(fill => fill.style.width = "0");
    document.querySelectorAll("#softskills-trigger .percent").forEach(percent => percent.innerText = "0%");
  });
</script>

<style>

  
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

/* PREVENT CONTENT FROM BEING HIDDEN UNDER HEADER */
#main {
  padding-top: 100px; /* Adjust to match header height */
}

<!-- IMAGE DISPLAYED TO THE RIGHT OF SOFT SKILLS -->
<div class="skills-image-wrapper">
  <div class="skills-left">
    <!-- This space is intentionally left for the soft skills list (already present) -->
  </div>
  <div class="skills-right">
    <img src="https://via.placeholder.com/200x400?text=Calendar+Image" alt="Calendar Image" />
  </div>
</div>
