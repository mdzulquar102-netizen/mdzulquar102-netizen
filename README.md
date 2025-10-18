<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Md Zulquarnain Ansari — Electrical Engineer</title>

<!-- Font Awesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
<!-- Google Font -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">

<style>
:root{
  --bg: #ffffff;
  --text: #0b0b0b;
  --muted: #525252;
  --accent: #00d4ff;
  --card: #ffffff;
  --glass: rgba(255,255,255,0.6);
  --shadow: rgba(10,10,10,0.08);
  --glass-2: rgba(0,0,0,0.04);
}
[data-theme="dark"]{
  --bg: #0b0e12;
  --text: #e8f0ff;
  --muted: #bfcadb;
  --accent: #6ef2ff;
  --card: #0f1418;
  --glass: rgba(255,255,255,0.04);
  --glass-2: rgba(255,255,255,0.03);
  --shadow: rgba(0,0,0,0.6);
}

*{box-sizing:border-box}
html,body{height:100%;margin:0;font-family:"Poppins",system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;background:var(--bg);color:var(--text);-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;overflow-x:hidden}

/* Header */
header{position:fixed;left:0;right:0;top:0;height:72px;display:flex;align-items:center;justify-content:space-between;padding:14px 6%;z-index:1200;background:linear-gradient(180deg,var(--glass),transparent);backdrop-filter:blur(8px) saturate(1.05);border-bottom:1px solid var(--glass-2);box-shadow:0 6px 18px var(--shadow);}
.brand{display:flex;gap:12px;align-items:center;}
.brand .logo{width:46px;height:46px;border-radius:10px;display:grid;place-items:center;font-weight:800;color:var(--bg);background:linear-gradient(135deg,var(--accent),#6a8cff);box-shadow:0 6px 20px rgba(0,0,0,0.12);}
.brand .name{line-height:1;}
.brand h1{font-size:16px;margin:0;font-weight:700;letter-spacing:0.6px}
.brand p{margin:0;font-size:12px;color:var(--muted)}

nav a{margin-left:22px;text-decoration:none;color:var(--muted);font-weight:600;font-size:14px;position:relative;padding:6px 0;}
nav a:hover{color:var(--text)}
nav a::after{content:'';position:absolute;height:2px;left:0;right:0;bottom:-6px;background:linear-gradient(90deg,var(--accent),transparent);transform:scaleX(0);transform-origin:left;transition:transform .32s;}
nav a:hover::after{transform:scaleX(1)}

.controls{display:flex;align-items:center;gap:14px}
.theme-toggle{width:54px;height:30px;border-radius:20px;padding:4px;background:var(--glass-2);display:flex;align-items:center;cursor:pointer;border:1px solid var(--glass-2);}
.theme-toggle .knob{width:22px;height:22px;border-radius:50%;background:var(--card);box-shadow:0 6px 16px rgba(0,0,0,0.12);transition:transform .28s}
[data-theme="dark"] .theme-toggle{background:rgba(255,255,255,0.03)}
[data-theme="dark"] .theme-toggle .knob{transform:translateX(24px)}

/* Floating socials */
.floating-socials{position:fixed;right:18px;bottom:20%;display:flex;flex-direction:column;gap:14px;z-index:1000;}
.floating-socials a{width:46px;height:46px;border-radius:12px;background:var(--card);display:grid;place-items:center;box-shadow:0 8px 18px rgba(0,0,0,0.08);color:var(--text);text-decoration:none;font-size:18px;transition:transform .28s, box-shadow .28s;}
.floating-socials a:hover{transform:translateY(-8px) rotate(-6deg);box-shadow:0 14px 30px rgba(0,0,0,0.18)}

/* Hero */
.hero{min-height:100vh;padding:120px 6% 80px;display:flex;align-items:center;gap:40px;position:relative;overflow:hidden;}
.hero-grid{display:grid;grid-template-columns:1fr 420px;gap:36px;align-items:center;width:100%}
.intro{max-width:900px;}
.eyebrow{display:inline-block;background:linear-gradient(90deg,var(--accent),#6a8cff);color:var(--bg);padding:6px 12px;border-radius:999px;font-weight:700;font-size:13px;margin-bottom:18px}
.headline{font-size:44px;line-height:1.03;margin:0 0 14px;font-weight:800;letter-spacing:0.6px}
.sub{color:var(--muted);font-size:16px;margin-bottom:22px;max-width:66%}
.cta-row{display:flex;gap:14px;align-items:center}
.btn{padding:12px 18px;border-radius:10px;border:0;font-weight:700;cursor:pointer;background:linear-gradient(90deg,var(--accent),#7ce0ff);color:var(--bg);box-shadow:0 12px 30px rgba(0,0,0,0.12);transition:transform .22s,box-shadow .22s;}
.btn.secondary{background:transparent;color:var(--text);border:1px solid var(--glass-2);box-shadow:none}
.btn:hover{transform:translateY(-6px);box-shadow:0 20px 40px rgba(0,0,0,0.16)}

.hero-card{width:420px;height:420px;border-radius:18px;background:linear-gradient(180deg,var(--card),var(--glass));box-shadow:0 24px 60px rgba(0,0,0,0.12);display:grid;place-items:center;position:relative;overflow:hidden;border:1px solid var(--glass-2);}
.hero-card img{width:100%;height:100%;object-fit:cover;filter:contrast(.98) saturate(1.05)}
.vignette{position:absolute;inset:0;background:radial-gradient(circle at 10% 10%, rgba(0,0,0,0.06), transparent 20%);pointer-events:none}

/* Sections */
section{padding:100px 6%;position:relative}
.container{max-width:1200px;margin:0 auto}

/* Skills */
.skills{display:flex;gap:14px;flex-wrap:wrap;justify-content:center;margin-top:20px}
.skill-pill{padding:10px 18px;border-radius:999px;border:1px solid var(--glass-2);font-weight:700;color:var(--text);background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent)}

/* Feedback Form */
form{max-width:720px;margin:20px auto 0;display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
form .full{grid-column:1/3}
input,textarea{padding:14px;border-radius:10px;border:1px solid var(--glass-2);background:transparent;color:var(--text);outline:none;font-size:15px;resize:vertical}
button[type="submit"]{grid-column:1/3;padding:12px;border-radius:12px;background:linear-gradient(90deg,var(--accent),#76e6ff);border:0;font-weight:800;color:var(--bg);cursor:pointer;transition:transform .22s}
button[type="submit"]:hover{transform:translateY(-6px)}

#formMsg{opacity:0;text-align:center;color:var(--accent);margin-top:12px;font-weight:700;transition:opacity .5s ease-in-out;}

/* Social Row */
.social-row{display:flex;gap:14px;justify-content:center;margin-top:16px}
.social-row a{width:56px;height:56px;border-radius:14px;display:grid;place-items:center;background:var(--card);text-decoration:none;color:var(--text);box-shadow:0 10px 30px var(--shadow);transition:transform .32s}
.social-row a:hover{transform:translateY(-8px) rotate(-6deg)}

footer{padding:34px 6%;text-align:center;color:var(--muted);border-top:1px solid var(--glass-2);margin-top:40px}

@media(max-width:880px){.hero-grid{grid-template-columns:1fr;gap:26px}.hero{padding-top:110px}.hero-card{width:100%;height:360px}form{grid-template-columns:1fr}.brand .name{display:none}nav{display:none}}
</style>
</head>
<body>
<div id="root" data-theme="light">

<header>
  <div class="brand">
    <div class="logo">ZA</div>
    <div class="name"><h1>Md Zulquarnain</h1><p>Electrical Engineer</p></div>
  </div>
  <nav>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#contact">Contact</a>
    <a href="#feedback">Feedback</a>
  </nav>
  <div class="controls"><div class="theme-toggle" id="themeToggle" role="button" tabindex="0"><div class="knob"></div></div></div>
</header>

<!-- Floating Socials -->
<div class="floating-socials">
  <a title="Instagram" href="https://www.instagram.com/_.mohd.zulquar._?igsh=MWh2M3h5dDNnNnQ0cw==" target="_blank"><i class="fab fa-instagram"></i></a>
  <a title="LinkedIn" href="https://www.linkedin.com/in/md-zulquarnain-ansari-835a31269" target="_blank"><i class="fab fa-linkedin"></i></a>
  <a title="WhatsApp" href="https://wa.me/919065913711" target="_blank"><i class="fab fa-whatsapp"></i></a>
  <a title="Call" href="tel:+919065913711"><i class="fas fa-phone"></i></a>
  <a title="GitHub" href="https://github.com/mdzulquar102-netizen" target="_blank"><i class="fab fa-github"></i></a>
</div>

<!-- Hero -->
<section class="hero">
<div class="container hero-grid">
  <div class="intro">
    <span class="eyebrow">Electrical Engineer · Automation · Embedded</span>
    <h2 class="headline">Md Zulquarnain Ansari</h2>
    <p class="sub">I build hardware-first solutions that merge embedded software with efficient power design. My work spans automation, Arduino projects, and experimental energy ideas — designed to solve real-world problems.</p>
    <div class="cta-row">
      <a class="btn" href="#feedback">Give Feedback</a>
      <a class="btn secondary" href="https://github.com/mdzulquar102-netizen" target="_blank">View GitHub</a>
    </div>
  </div>
  <div class="hero-card">
    <img src="https://drive.google.com/file/d/17PP_Xd2S3ctp3j41rfOdVsTNABPD1e6L/view?usp=sharing" alt="Md Zulquarnain Ansari"/>
    <div class="vignette"></div>
  </div>
</div>
</section>

<!-- About -->
<section id="about">
<div class="container">
<h2>About Me</h2>
<p>Hi — I'm <strong>Md Zulquarnain Ansari</strong>, a B.Tech Electrical Engineer with a <strong>Diploma in Electrical Engineering</strong>. I focus on automation (Arduino/ESP32), embedded C development, and exploring sustainable energy solutions from waste. I enjoy turning prototypes into practical, deployable systems, Robotics.</p>
</div>
</section>

<!-- Skills -->
<section id="skills">
<div class="container">
<h2>Skills</h2>
<div class="skills">
  <div class="skill-pill">C Programming</div>
  <div class="skill-pill">Arduino</div>
  <div class="skill-pill">ESP32</div>
</div>
</div>
</section>

<!-- Contact -->
<section id="contact">
<div class="container">
<h2>Contact Details</h2>
<div class="social-row">
  <a href="https://www.instagram.com/_.mohd.zulquar._?igsh=MWh2M3h5dDNnNnQ0cw==" target="_blank"><i class="fab fa-instagram"></i></a>
  <a href="https://www.linkedin.com/in/md-zulquarnain-ansari-835a31269" target="_blank"><i class="fab fa-linkedin"></i></a>
  <a href="https://wa.me/919065913711" target="_blank"><i class="fab fa-whatsapp"></i></a>
  <a href="tel:+919065913711"><i class="fas fa-phone"></i></a>
  <a href="https://github.com/mdzulquar102-netizen" target="_blank"><i class="fab fa-github"></i></a>
</div>
</div>
</section>

<!-- Feedback -->
<section id="feedback">
<div class="container">
<h2>Give Your Feedback</h2>
<p>Please share your name, email, phone (optional), and message. I’ll read every submission.</p>
<form id="feedbackForm" action="https://formspree.io/f/xyznorvj" method="POST">
  <input name="name" type="text" placeholder="Your Name" required />
  <input name="email" type="email" placeholder="Your Email" required />
  <input name="phone" type="tel" placeholder="Phone (optional)" />
  <textarea name="message" rows="5" class="full" placeholder="Your Message..." required></textarea>
  <button type="submit">Send Feedback</button>
</form>
<p id="formMsg">Thanks! Your feedback has been sent.</p>
</div>
</section>

<footer>
© <span id="year"></span> Md Zulquarnain Ansari — Built with care · <a href="https://github.com/mdzulquar102-netizen" target="_blank">GitHub</a>
</footer>

<script>
/* Theme toggle */
(function(){
  const root = document.getElementById('root');
  const toggle = document.getElementById('themeToggle');
  const stored = localStorage.getItem('mdz_theme');
  const prefersDark = window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches;
  if(stored) root.setAttribute('data-theme', stored);
  else root.setAttribute('data-theme', prefersDark ? 'dark' : 'light');
  toggle.addEventListener('click', ()=>{ root.setAttribute('data-theme', root.getAttribute('data-theme') === 'dark' ? 'light' : 'dark'); });
  toggle.addEventListener('keypress', (e)=>{ if(e.key==='Enter') toggle.click() });
  document.getElementById('year').textContent = new Date().getFullYear();
})();

/* Feedback form animation */
document.getElementById('feedbackForm').addEventListener('submit', function(e){
  const formMsg = document.getElementById('formMsg');
  formMsg.style.opacity = '1';
  setTimeout(()=> formMsg.style.opacity='0', 5000);
});
</script>

</div>
</body>
</html>
