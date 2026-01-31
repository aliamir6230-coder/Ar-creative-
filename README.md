# Ar-creative-<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Amir | Freelance Video Editor</title>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
<style>
/* ===== General ===== */
*{margin:0;padding:0;box-sizing:border-box;}
body{font-family:'Montserrat',sans-serif;line-height:1.6;color:#333;background:#f4f4f4;}
a{text-decoration:none;color:inherit;}
img{max-width:100%;display:block;}
section{padding:60px 20px;}
h1,h2,h3{margin-bottom:20px;}

/* ===== Header ===== */
header{position:fixed;top:0;width:100%;background:rgba(255,255,255,0.95);padding:20px 50px;display:flex;justify-content:space-between;align-items:center;box-shadow:0 2px 8px rgba(0,0,0,0.1);z-index:1000;transition:0.3s;}
header.scrolled{background:#4a90e2;color:#fff;}
nav a{margin-left:25px;font-weight:600;transition:0.3s;}
nav a:hover{color:#4a90e2;}

/* ===== Hero ===== */
.hero{height:100vh;background:linear-gradient(to right,#4a90e2,#357ABD);color:#fff;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;padding:0 20px;}
.hero h1{font-size:3em;margin-bottom:20px;}
.hero p{font-size:1.2em;margin-bottom:30px;max-width:600px;}
.hero a{background:#fff;color:#4a90e2;padding:15px 35px;border-radius:50px;font-weight:bold;box-shadow:0 5px 15px rgba(0,0,0,0.2);transition:0.3s;}
.hero a:hover{transform:translateY(-3px);box-shadow:0 8px 20px rgba(0,0,0,0.3);}

/* ===== Portfolio ===== */
.portfolio-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:25px;}
.project{position:relative;overflow:hidden;border-radius:12px;cursor:pointer;box-shadow:0 4px 15px rgba(0,0,0,0.1);transition:transform 0.3s;}
.project img{display:block;width:100%;height:auto;}
.project:hover{transform:scale(1.05);}
.project-overlay{position:absolute;top:0;left:0;width:100%;height:100%;background:rgba(0,0,0,0.7);color:#fff;opacity:0;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;padding:20px;transition:opacity 0.3s;}
.project:hover .project-overlay{opacity:1;}

/* Lightbox */
.lightbox{position:fixed;top:0;left:0;width:100%;height:100%;background:rgba(0,0,0,0.9);display:flex;justify-content:center;align-items:center;opacity:0;pointer-events:none;transition:opacity 0.3s;z-index:2000;}
.lightbox img{max-width:90%;max-height:80%;}
.lightbox.active{opacity:1;pointer-events:auto;}

/* ===== Services ===== */
.services{display:flex;flex-wrap:wrap;gap:25px;justify-content:center;}
.service{background:#fff;padding:25px;border-radius:12px;width:250px;text-align:center;box-shadow:0 4px 15px rgba(0,0,0,0.1);transition:transform 0.3s;}
.service:hover{transform:translateY(-5px);}

/* ===== Testimonials ===== */
.testimonial-container{max-width:800px;margin:0 auto;display:flex;flex-direction:column;gap:20px;}
.testimonial{background:#fff;padding:25px;border-radius:12px;box-shadow:0 4px 15px rgba(0,0,0,0.1);transition:transform 0.3s;}
.testimonial:hover{transform:translateY(-5px);}
.testimonial p{font-style:italic;margin-bottom:10px;}
.testimonial strong{display:block;text-align:right;}

/* ===== Counters ===== */
.counters{display:flex;justify-content:center;flex-wrap:wrap;gap:50px;margin-top:50px;}
.counter{background:#fff;padding:25px;border-radius:12px;width:150px;text-align:center;box-shadow:0 4px 15px rgba(0,0,0,0.1);}
.counter span{font-size:2em;font-weight:bold;color:#4a90e2;display:block;}

/* ===== Contact ===== */
.contact-form{max-width:500px;margin:0 auto;display:flex;flex-direction:column;gap:15px;}
.contact-form input,.contact-form textarea{padding:15px;border-radius:8px;border:1px solid #ccc;font-size:1em;}
.contact-form button{padding:15px;border:none;background:#4a90e2;color:#fff;font-weight:bold;border-radius:50px;cursor:pointer;transition:0.3s;}
.contact-form button:hover{background:#357ABD;}

/* ===== Floating Hire Me Button ===== */
.hire-btn{position:fixed;bottom:30px;right:30px;background:#4a90e2;color:#fff;padding:15px 25px;border-radius:50px;font-weight:bold;box-shadow:0 5px 15px rgba(0,0,0,0.2);z-index:1000;transition:0.3s;}
.hire-btn:hover{transform:translateY(-3px);box-shadow:0 8px 20px rgba(0,0,0,0.3);}

/* ===== Footer ===== */
footer{background:#333;color:#fff;text-align:center;padding:30px 20px;}

/* ===== Smooth Scroll ===== */
html{scroll-behavior:smooth;}

/* ===== Responsive ===== */
@media(max-width:768px){header{flex-direction:column;align-items:flex-start;}nav{margin-top:10px;}.hero h1{font-size:2.5em;}.hero p{font-size:1em;}}
</style>
</head>
<body>

<!-- Header -->
<header id="header">
<h2>Amir</h2>
<nav>
<a href="#portfolio">Portfolio</a>
<a href="#services">Services</a>
<a href="#testimonials">Testimonials</a>
<a href="#contact">Contact</a>
</nav>
</header>

<!-- Hero Section -->
<section class="hero">
<h1>Hi, I’m Amir</h1>
<p>Freelance Video Editor creating engaging and professional video content for clients.</p>
<a href="#portfolio">View My Work</a>
</section>

<!-- Portfolio Section -->
<section id="portfolio">
<h2>My Work</h2>
<div class="portfolio-grid">
<div class="project">
<img src="project1.jpg" alt="Project 1">
<div class="project-overlay">
<h3>Project Name 1</h3>
<p>Editing, color grading, and motion graphics project.</p>
</div>
</div>
<div class="project">
<img src="project2.jpg" alt="Project 2">
<div class="project-overlay">
<h3>Project Name 2</h3>
<p>Short film or YouTube content edited professionally.</p>
</div>
</div>
<!-- Add more projects -->
</div>
</section>

<!-- Counters Section -->
<section id="stats">
<h2 style="text-align:center;">My Achievements</h2>
<div class="counters">
<div class="counter"><span class="count" data-target="50">0</span> Projects</div>
<div class="counter"><span class="count" data-target="30">0</span> Happy Clients</div>
<div class="counter"><span class="count" data-target="5">0</span> Years Experience</div>
</div>
</section>

<!-- Services Section -->
<section id="services">
<h2>What I Offer</h2>
<div class="services">
<div class="service">Video Editing</div>
<div class="service">Motion Graphics & VFX</div>
<div class="service">Color Grading</div>
<div class="service">YouTube / Social Media Videos</div>
</div>
</section>

<!-- Testimonials Section -->
<section id="testimonials">
<h2>What My Clients Say</h2>
<div class="testimonial-container">
<div class="testimonial">
<p>"Amir is a brilliant video editor. The videos exceeded all expectations!"</p>
<strong>- Client Name</strong>
</div>
<div class="testimonial">
<p>"Highly professional and creative. Amir delivered on time and beautifully."</p>
<strong>- Client Name</strong>
</div>
</div>
</section>

<!-- Contact Section -->
<section id="contact">
<h2>Let’s Work Together</h2>
<form class="contact-form">
<input type="text" placeholder="Your Name" required>
<input type="email" placeholder="Your Email" required>
<textarea rows="5" placeholder="Your Message" required></textarea>
<button type="submit">Send Message</button>
</form>
</section>

<!-- Floating Hire Me Button -->
<a href="#contact" class="hire-btn">Hire Me</a>

<!-- Footer -->
<footer>
© 2026 Amir | <a href="#portfolio" style="color:#fff;">Back to Top</a>
</footer>

<!-- Lightbox -->
<div class="lightbox" id="lightbox"><img src="" alt="Lightbox"></div>

<script>
// Header scroll effect
window.addEventListener('scroll',()=>{const h=document.getElementById('header');window.scrollY>50?h.classList.add('scrolled'):h.classList.remove('scrolled');});

// Lightbox
const projects=document.querySelectorAll('.project');
const lightbox=document.getElementById('lightbox');
const lightboxImg=lightbox.querySelector('img');
projects.forEach(p=>p.addEventListener('click',()=>{lightbox.classList.add('active');lightboxImg.src=p.querySelector('img').src;}));
lightbox.addEventListener('click',()=>{lightbox.classList.remove('active');});

// Counters animation
const counters=document.querySelectorAll('.count');
counters.forEach(counter=>{
let updateCount=()=>{
let target=+counter.getAttribute('data-target');
let count=+counter.innerText;
let increment=target/200;
if(count<target){counter.innerText=Math.ceil(count+increment);setTimeout(updateCount,10);}else{counter.innerText=target;}
};
updateCount();
});
</script>

</body>
</html>
