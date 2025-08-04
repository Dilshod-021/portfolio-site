<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <!-- <link rel="stylesheet" href="style.css" /> -->
  <title>Hero Section</title>
</head>
<body>
  <style>
         * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background:rgb(235, 235, 250);
      color: #333;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 60px;
    }

    .logo {
      display:block;
      position: relative;
      width: 60px;
      height: 60px;
      background: #8e44ad; /* Purple */
      border-radius: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: sans-serif;
      font-size: 40px;
      font-weight: bold;
      color: white;
    }
    .logo_text {
      font-size: 40px;
      font-weight: 700;
      line-height: 100%;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }   

    .logo::before {
      content: "";
      position: absolute;
      top: 0;
      right: 0;
      width: 34px;
      height: 33px;
      background: #ff69b4;
      border-radius: 10px 0 10px 0;
      z-index: 0;
    }
    
     .nav-links {
        display: flex;
        gap: 30px;
      }
  
      .nav-links a {
        text-decoration: none;
        color: #333;
        font-weight: 500;
      }
  
      .hero {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 60px;
      }
  
      .hero-text {
        max-width: 600px;
      }
  
      .hero-text h1 {
        font-size: 48px;
        margin-bottom: 10px;
      }
  
      .hero-text p {
        font-size: 20px;
        margin-bottom: 20px;
      }
  
      .hero-text button {
        background: #8e44ad;
        color: white;
        border: none;
        padding: 12px 30px;
        font-size: 16px;
        border-radius: 30px;
        cursor: pointer;
      }
  
      .hero-image {
        position: relative;
      }

      .hero-image img.person {
        position: relative;
        z-index: 2;
        max-width: 400px;
      }

    .main {
      background-color: rgb(240, 248, 255);
      max-width: 1440px;
      margin: 0 auto;
      padding: 0 165px;
      -webkit-box-shadow: -1px 2px 11px 0px rgba(0, 0, 0, 0.27);
-moz-box-shadow: -1px 2px 11px 0px rgba(0, 0, 0, 0.27);
box-shadow: -1px 2px 11px 0px rgba(0, 0, 0, 0.27);
    }

    .services_text{
      font-size: 18px;
      font-weight: 400;
      line-height: 100%;
      letter-spacing: 0%;
      width: 68px;
      height: 24px;
    }

    .services_text span {
      display: block;
      width: 50px;
      height: 2px;
      background-color: #8e44ad;
      margin-top: 10px;
    }

    .whatido{
      width: 246px;
      height: 96px;
      font-size: 36px;
      font-weight: 700;
      line-height: 100%;
      letter-spacing: 0%;
      margin-top: 20px;
      color: #333;
    }

.sections {
  display: flex;
  flex-direction: column;
  gap: 40px;
  margin: 40px 0;
}

.section {
  display: flex;
  align-items: center; /* rasm va matn vertikal markazda */
  gap: 30px;
  background-color: #fff;
  padding: 20px;
  border-radius: 20px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
  transition: transform 0.3s ease;
}

.section:hover {
  transform: translateY(-5px);
}

.section-image {
  width: 100px;
  height: 100px;
  object-fit: contain;
  flex-shrink: 0;
}

.section-text {
  flex: 1;
}

.section-text h2 {
  font-size: 24px;
  font-weight: 700;
  margin-bottom: 10px;
  position: relative;
}

.section-text h2::after {
  content: "";
  display: block;
  width: 40px;
  height: 3px;
  background-color: #8e44ad;
  margin-top: 10px;
}


    .projects-section {
  padding: 80px 20px;
  text-align: center;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

.section-label {
  color: #a884f6;
  font-weight: 600;
  font-size: 14px;
  margin-bottom: 10px;
}

.section-title {
  font-size: 36px;
  font-weight: 700;
  margin-bottom: 40px;
  color: #1a1a1a;
}

.projects-grid {
  display: flex;
  justify-content: center;
  gap: 40px;
  flex-wrap: wrap;
  margin-bottom: 30px;
}

.project-card {
  width: 500px;
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
  transition: transform 0.3s ease;
}

.project-card img {
  width: 100%;
  height: auto;
  display: block;
}

.project-card:hover {
  transform: translateY(-8px);
}

.explore-link {
  color: #7c3aed;
  text-decoration: none;
  font-weight: 600;
  font-size: 16px;
  transition: color 0.3s;
}

.explore-link:hover {
  color: #5b21b6;
}
.testimonial-section {
  padding: 100px 20px;
  text-align: center;
}

.section-label {
  color: #a884f6;
  font-weight: 600;
  font-size: 14px;
  margin-bottom: 10px;
}

.section-title {
  font-size: 36px;
  font-weight: 700;
  margin-bottom: 50px;
  color: #1a1a1a;
}

.testimonial-content {
  max-width: 800px;
  margin: 0 auto;
  position: relative;
}

.quote-icon {
  font-size: 40px;
  color: #a884f6;
  display: block;
  margin-bottom: 20px;
}

.testimonial-text {
  font-size: 18px;
  color: #444;
  line-height: 1.6;
  margin-bottom: 40px;
}

.author-info img {
  width: 80px;
  height: 80px;
  object-fit: cover;
  border-radius: 50%;
  margin-bottom: 10px;
  
}

.author-info h3 {
  font-size: 20px;
  margin: 5px 0 2px;
}

.author-position {
  font-size: 14px;
  color: #666;
}

.dots {
  display: flex;
  justify-content: center;
  gap: 10px;
  margin-top: 30px;
}

.dot {
  width: 10px;
  height: 10px;
  background: #ddd;
  border-radius: 50%;
  transition: background 0.3s ease;
  cursor: pointer;
}

.dot.active {
  background: #a884f6;
}

.contact-section {
  padding: 40px 60px;  /* 20px dan 60px ga oshirildi */
  max-width: 1200px;   /* 900px dan 1200px ga oshirildi */
  margin: 40px auto;   /* yuqoriga ham biroz bo‘sh joy qo‘shildi */
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #121212;
  box-sizing: border-box;
}


.contact-link {
  display: inline-block;
  color: #7b2ff7;
  font-weight: 500;
  font-size: 16px;
  border-bottom: 2px solid #7b2ff7;
  text-decoration: none;
  margin-bottom: 10px;
}

.contact-header h2 {
  font-weight: 700;
  font-size: 28px;
  line-height: 1.3;
  margin: 10px 0 30px;
  max-width: 600px;
}

.email-link {
  color: #7b2ff7;
  text-decoration: underline;
  float: right;
  font-size: 16px;
  font-weight: 500;
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 15px;
  max-width: 600px;
  margin-top: 10px;
}

.contact-form input[type="text"],
.contact-form input[type="email"] {
  border: none;
  border-bottom: 1px solid #ccc;
  padding: 10px 8px;
  font-size: 16px;
  outline: none;
  transition: border-color 0.3s ease;
}

.contact-form input[type="text"]:focus,
.contact-form input[type="email"]:focus {
  border-bottom-color: #7b2ff7;
}

.quote-btn {
  width: 140px;
  padding: 12px 0;
  background-color: #7b2ff7;
  color: white;
  font-weight: 600;
  border: none;
  border-radius: 30px;
  cursor: pointer;
  transition: background-color 0.3s ease;
  margin-top: 10px;
  align-self: flex-start;
}

.quote-btn:hover {
  background-color: #631ad9;
}

.friends-section {
  text-align: center;
  margin-top: 60px;
}

.friends-section h3 {
  font-weight: 600;
  font-size: 24px;
  margin-bottom: 20px;
}

.social-icons {
  display: flex;
  justify-content: center;
  gap: 25px;
}

.icon {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  background: linear-gradient(135deg, #fbb1f9, #ad51f1);
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-size: 22px;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.icon:hover {
  transform: scale(1.2);
}

/* Social iconlar uchun misol ikonalar */
/* O'zingizga mos SVG yoki font ikonalari bilan almashtiring */
.icon.dribbble::before {
  content: "";
  font-family: 'FontAwesome';
}

.icon.instagram::before {
  content: "";
  font-family: 'FontAwesome';
}

.icon.linkedin::before {
  content: "";
  font-family: 'FontAwesome';
}


  </style>
    <div class="main">
  <header>
    <div class="logo">
      <div class="logo-circle">
        <span class="logo_text">D</span>
      </div>
    </div>
    <nav class="nav-links">
      <a href="#">About</a>
      <a href="#">Services</a>
      <a href="#">Works</a>
      <a href="#">Blog</a>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-text">
      <p>Hello,</p>
      <h1>Dilshod Mansurjonov               </h1>
      <p>a freelance HTML layout maker</p>
      <button>Let’s Talk</button>
    </div>
    <div class="hero-image">
      <img src="./img/user-image 1.png" alt="Adam Zakob" class="person">
    </div>
  </section>
  <section class="services">
    <div class="services_text">Services 
        <br>
        <span></span>
    </div>
    <h1 class="whatido">What  actually 
I love to do</h1>
<div class="sections">
  <div class="section">
    <img src="./img/Group 3.png" alt="Layout Building" class="section-image">
    <div class="section-text">
      <h2>Layout Building</h2>
      <p>I enjoy turning designs into clean, responsive HTML/CSS layouts. Every section, every div — it’s all about structure, flow, and pixel-perfection.</p>
    </div>
  </div>
  <div class="section">
    <img src="./img/Group 3 (1).png" alt="Component Crafting" class="section-image">
    <div class="section-text">
      <h2>Component Crafting</h2>
      <p>Buttons, forms, cards — I love building reusable UI components that fit any project and keep the codebase clean.</p>
    </div>
  </div>
  <div class="section">
    <img src="./img/Group 31.png" alt="Clean Code Lover" class="section-image">
    <div class="section-text">
      <h2>Clean Code Lover</h2>
      <p>Writing semantic HTML and organized CSS isn’t a task — it’s my passion. I believe clean code = maintainable design.</p>
    </div>
  </div>
</div>

  </section>
  <section class="projects-section">
  <div class="container">
    <p class="section-label">Portfolio</p>
    <h2 class="section-title">All Creative Projects</h2>

    <div class="projects-grid">
      <div class="project-card">
        <img src="./img/Rectangle 5.png" alt="Project 1">
      </div>
      <div class="project-card">
        <img src="./img/Rectangle 6.png" alt="Project 2">
      </div>
    </div>

    <a href="#" class="explore-link">Explore More →</a>
  </div>
</section>
  <section class="testimonial-section">
  <div class="container">
    <p class="section-label">Testimonials</p>
    <h2 class="section-title">What People Says</h2>

    <div class="testimonial-content">
      <span class="quote-icon">❝</span>
      <p class="testimonial-text">
        Quote testimonials demonstrate support for your product or feature from a user who has experience with it.
        This can be significantly more effective than traditional advertising methods as most consumers will trust.
      </p>
      <div class="author-info">
        <img src="michal.jpg" alt="Michal John">
        <h3>Michal John</h3>
        <p class="author-position">CEO of MZP</p>
      </div>

      <div class="dots">
        <span class="dot active"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
      </div>
    </div>
  </div>
</section>
<section class="contact-section">
  <div class="contact-header">
    <a href="#" class="contact-link">Contact Me</a>
    <h2>
      Let me know if you want to talk <br />
      about a potential collaboration. <br />
      I'm available for freelance work.
    </h2>
    <a href="mailto:infoname@mail.com" class="email-link">dilshodmansurjonov04@mail.com</a>
  </div>

  <form class="contact-form">
    <input type="text" placeholder="What’s your name?" name="name" required />
    <input type="email" placeholder="Your email" name="email" required />
    <input type="text" placeholder="Tell me about your project" name="project" />
    <button type="submit" class="quote-btn">Get a Quote</button>
  </form>

  <div class="friends-section">
    <h3>Let’s be Friends</h3>
    <div class="social-icons">
      <a href="#" class="icon dribbble" aria-label="Dribbble"></a>
      <a href="#" class="icon instagram" aria-label="Instagram"></a>
      <a href="#" class="icon linkedin" aria-label="LinkedIn"></a>
    </div>
  </div>
</section>

  </div>
</body>
</html>
