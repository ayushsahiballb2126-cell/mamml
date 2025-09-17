<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>MAMML | Cold Email & Inbox Infrastructure Agency</title>
  <link rel="stylesheet" href="style.css" />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet" />
  <script defer src="script.js"></script>
</head>
<body>
  <!-- ================= HEADER ================= -->
  <header class="header">
    <div class="container header-container">
      <a href="#" class="logo">
        <img src="/assets/logo.svg" alt="MAMML Logo">
      </a>
      <nav class="nav">
        <ul class="nav-links">
          <li><a href="#">Home</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#pricing">Pricing</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
      <a href="#calendly" class="btn btn-accent">Book a Call</a>
      <div class="hamburger"><span></span><span></span><span></span></div>
    </div>
  </header>

  <!-- ================= HERO ================= -->
  <section class="hero">
    <div class="container hero-content">
      <div class="hero-text">
        <h1>MAMML — Done-For-You Cold Email Outreach That Books Meetings.</h1>
        <p>Inbox setup, deliverability, and campaigns handled end-to-end.</p>
        <a href="#calendly" class="btn btn-accent">Book a Call</a>
      </div>
      <div class="hero-image">
        <img src="/assets/hero.jpg" alt="Cold Email Agency">
      </div>
    </div>
  </section>

  <!-- ================= METRICS ================= -->
  <section class="metrics">
    <div class="container metrics-container">
      <div class="metric">
        <span class="counter" data-target="250">0</span><span>+</span>
        <p>Calls Booked</p>
      </div>
      <div class="metric">
        <span class="counter" data-target="97">0</span><span>%</span>
        <p>Inbox Placement</p>
      </div>
      <div class="metric">
        <span class="counter" data-target="48">0</span><span>h</span>
        <p>Setup Guarantee</p>
      </div>
    </div>
  </section>

  <!-- ================= SERVICES ================= -->
  <section id="services" class="services">
    <div class="container">
      <h2>Our Services</h2>
      <div class="services-grid">
        <div class="service-card">📩 <h3>Inbox Setup & Domain Warm-Up</h3></div>
        <div class="service-card">✉️ <h3>Cold Email Copy & Sequencing</h3></div>
        <div class="service-card">🚀 <h3>Campaign Management</h3></div>
        <div class="service-card">📊 <h3>Reporting & Analytics</h3></div>
      </div>
    </div>
  </section>

  <!-- ================= PROCESS ================= -->
  <section class="process">
    <div class="container">
      <h2>How It Works</h2>
      <div class="process-steps">
        <div class="step"><span>1</span><p>Strategy Call</p></div>
        <div class="step"><span>2</span><p>Inbox Setup</p></div>
        <div class="step"><span>3</span><p>Campaign Launch</p></div>
        <div class="step"><span>4</span><p>Meetings Booked</p></div>
      </div>
    </div>
  </section>

  <!-- ================= CALENDLY CTA ================= -->
  <section id="calendly" class="calendly">
    <div class="container">
      <h2>Book a Call With MAMML Today</h2>
      <iframe src="https://calendly.com/your-link" width="100%" height="600" frameborder="0"></iframe>
    </div>
  </section>

  <!-- ================= ENQUIRY FORM ================= -->
  <section id="contact" class="contact">
    <div class="container">
      <h2>Get in Touch</h2>
      <form id="contactForm">
        <input type="text" name="name" placeholder="Name *" required />
        <input type="email" name="email" placeholder="Email *" required />
        <input type="text" name="company" placeholder="Company" />
        <textarea name="message" placeholder="Message *" required></textarea>
        <!-- Honeypot field -->
        <input type="text" name="honeypot" class="honeypot" />
        <button type="submit" class="btn btn-accent">Send Message</button>
        <p id="formMessage"></p>
      </form>
    </div>
  </section>

  <!-- ================= FOOTER ================= -->
  <footer class="footer">
    <div class="container footer-container">
      <div class="footer-left">
        <img src="/assets/logo.svg" alt="MAMML Logo">
        <p>Premium Cold Email & Inbox Infrastructure Agency</p>
      </div>
      <div class="footer-right">
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#pricing">Pricing</a></li>
          <li><a href="#about">About</a></li>
        </ul>
        <p>📧 hello@mamml.com</p>
      </div>
    </div>
    <div class="footer-bottom">© 2025 MAMML. All Rights Reserved.</div>
  </footer>
</body>
</html>
:root {
  --accent: #c9a75b; /* muted gold */
  --text: #2E2E2E;
  --bg: #f9f9f9;
}

* { box-sizing: border-box; margin: 0; padding: 0; }

body {
  font-family: 'Inter', sans-serif;
  color: var(--text);
  background: #fff;
  line-height: 1.6;
}

.container { width: 90%; max-width: 1200px; margin: 0 auto; }

/* HEADER */
.header {
  background: #fff;
  padding: 1rem 0;
  position: sticky; top: 0; z-index: 1000;
  border-bottom: 1px solid #eee;
}
.header-container {
  display: flex; align-items: center; justify-content: space-between;
}
.logo img { height: 40px; }
.nav-links { display: flex; list-style: none; gap: 2rem; }
.nav-links a { text-decoration: none; color: var(--text); font-weight: 600; }
.nav-links a:hover { color: var(--accent); }
.btn { padding: 0.7rem 1.5rem; border-radius: 5px; text-decoration: none; display: inline-block; transition: 0.3s; }
.btn-accent { background: var(--accent); color: #fff; }
.btn-accent:hover { opacity: 0.8; }
.hamburger { display: none; flex-direction: column; cursor: pointer; gap: 5px; }
.hamburger span { width: 25px; height: 3px; background: var(--text); }

/* HERO */
.hero { padding: 4rem 0; background: var(--bg); }
.hero-content { display: flex; align-items: center; gap: 2rem; flex-wrap: wrap; }
.hero-text { flex: 1; animation: fadeIn 1s ease; }
.hero-text h1 { font-size: 2rem; margin-bottom: 1rem; }
.hero-text p { margin-bottom: 1.5rem; }
.hero-image img { max-width: 100%; border-radius: 10px; }

/* METRICS */
.metrics { background: #fff; padding: 3rem 0; text-align: center; }
.metrics-container { display: flex; justify-content: space-around; flex-wrap: wrap; gap: 2rem; }
.metric span { font-size: 2rem; font-weight: 700; color: var(--accent); display: inline-block; }
.metric p { margin-top: 0.5rem; }

/* SERVICES */
.services { padding: 4rem 0; text-align: center; }
.services-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 2rem; margin-top: 2rem; }
.service-card { background: var(--bg); padding: 2rem; border-radius: 10px; transition: 0.3s; font-size: 1.1rem; }
.service-card:hover { transform: translateY(-5px); box-shadow: 0 5px 20px rgba(0,0,0,0.05); }

/* PROCESS */
.process { padding: 4rem 0; text-align: center; background: #fff; }
.process-steps { display: grid; grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); gap: 2rem; margin-top: 2rem; }
.step span { display: block; font-size: 2rem; color: var(--accent); font-weight: 700; }

/* CALENDLY */
.calendly { padding: 4rem 0; text-align: center; background: var(--bg); }

/* CONTACT */
.contact { padding: 4rem 0; text-align: center; }
form { display: flex; flex-direction: column; gap: 1rem; max-width: 500px; margin: auto; }
form input, form textarea { padding: 1rem; border: 1px solid #ddd; border-radius: 5px; font-family: inherit; }
.honeypot { display: none; }
#formMessage { margin-top: 1rem; font-size: 0.9rem; }

/* FOOTER */
.footer { background: #111; color: #fff; padding: 2rem 0; }
.footer-container { display: flex; justify-content: space-between; flex-wrap: wrap; gap: 2rem; }
.footer-container ul { list-style: none; }
.footer-container a { color: #fff; text-decoration: none; }
.footer-container a:hover { color: var(--accent); }
.footer-bottom { text-align: center; margin-top: 1rem; font-size: 0.85rem; }

/* MOBILE */
@media (max-width: 768px) {
  .nav { display: none; }
  .hamburger { display: flex; }
  .nav.active { display: block; position: absolute; top: 70px; right: 20px; background: #fff; padding: 1rem; border: 1px solid #ddd; }
  .nav-links { flex-direction: column; gap: 1rem; }
}

/* ANIMATIONS */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
// ================= Scroll Animations =================
function initScrollReveal() {
  const elements = document.querySelectorAll(".hero-text, .service-card, .step, .metric");
  const observer = new IntersectionObserver((entries, obs) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.style.opacity = "1";
        entry.target.style.transform = "translateY(0)";
        obs.unobserve(entry.target);
      }
    });
  }, { threshold: 0.1 });

  elements.forEach(el => {
    el.style.opacity = "0";
    el.style.transform = "translateY(30px)";
    el.style.transition = "all 0.6s ease-out";
    observer.observe(el);
  });
}

// ================= Counters =================
function initCounters() {
  const counters = document.querySelectorAll(".counter");
  const speed = 100; // lower = faster
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        counters.forEach(counter => {
          const updateCount = () => {
            const target = +counter.getAttribute("data-target");
            const count = +counter.innerText;
            const increment = Math.ceil(target / speed);
            if (count < target) {
              counter.innerText = count + increment;
              setTimeout(updateCount, 30);
            } else {
              counter.innerText = target;
            }
          };
          updateCount();
        });
        observer.disconnect();
      }
    });
  }, { threshold: 0.5 });
  observer.observe(document.querySelector(".metrics"));
}

// ================= Mobile Nav =================
function initMobileNav() {
  const hamburger = document.querySelector(".hamburger");
  const nav = document.querySelector(".nav");
  hamburger.addEventListener("click", () => {
    nav.classList.toggle("active");
  });
}

// ================= Contact Form =================
function initContactForm() {
  const form = document.getElementById("contactForm");
  const message = document.getElementById("formMessage");

  form.addEventListener("submit", e => {
    e.preventDefault();
    const honeypot = form.querySelector(".honeypot").value;
    if (honeypot) return; // Bot detected

    const name = form.name.value.trim();
    const email = form.email.value.trim();
    const msg = form.message.value.trim();

    if (!name || !email || !msg) {
      message.textContent = "Please fill in all required fields.";
      message.style.color = "red";
      return;
    }
    if (!/^[^@\s]+@[^@\s]+\.[^@\s]+$/.test(email)) {
      message.textContent = "Invalid email format.";
      message.style.color = "red";
      return;
    }

    // Simulated success (replace with SendGrid API integration later)
    message.textContent = "Message sent successfully!";
    message.style.color = "green";
    form.reset();
  });
}

// ================= Init =================
document.addEventListener("DOMContentLoaded", () => {
  initScrollReveal();
  initCounters();
  initMobileNav();
  initContactForm();
});

