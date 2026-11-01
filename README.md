[Uploading index.html…]()
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Abuli — Registrar &amp; Corporate Services | Commonwealth</title>
<meta name="description" content="Abuli · Registrar & corporate services across the Commonwealth. Entity formation, compliance, and governance." />
<style>
  :root{
    --navy:#14213d;
    --navy-2:#0e1a30;
    --gold:#c9a227;
    --gold-2:#e2bc4e;
    --ink:#232323;
    --paper:#faf8f3;
    --line:#e7e1d3;
    --muted:#6b6b66;
    --serif:Georgia,'Times New Roman',serif;
    --sans:-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,Helvetica,Arial,'PingFang SC','Microsoft YaHei',sans-serif;
  }
  *{box-sizing:border-box;margin:0;padding:0}
  html{scroll-behavior:smooth}
  body{font-family:var(--sans);color:var(--ink);background:var(--paper);line-height:1.7;-webkit-font-smoothing:antialiased}
  a{color:inherit;text-decoration:none}
  img{max-width:100%;display:block}

  .wrap{max-width:1120px;margin:0 auto;padding:0 24px}

  /* Nav */
  header{position:sticky;top:0;z-index:50;background:rgba(20,33,61,.96);backdrop-filter:blur(6px);color:#fff;border-bottom:1px solid rgba(255,255,255,.08)}
  nav{display:flex;align-items:center;justify-content:space-between;height:66px}
  .brand{font-family:var(--serif);font-size:1.25rem;letter-spacing:.5px;color:#fff}
  .brand b{color:var(--gold)}
  .nav-links{display:flex;gap:30px;font-size:.95rem}
  .nav-links a{color:#d9dce4;transition:color .2s}
  .nav-links a:hover{color:var(--gold)}
  .nav-cta{border:1px solid var(--gold);color:var(--gold);padding:8px 16px;border-radius:4px;transition:.2s}
  .nav-cta:hover{background:var(--gold);color:var(--navy)}
  .burger{display:none;background:none;border:none;color:#fff;font-size:1.5rem;cursor:pointer}

  /* Hero */
  .hero{background:linear-gradient(135deg,var(--navy-2),var(--navy));color:#fff;padding:96px 0 80px;position:relative;overflow:hidden}
  .hero::after{content:"";position:absolute;right:-120px;top:-120px;width:420px;height:420px;border-radius:50%;border:1px solid rgba(201,162,39,.25)}
  .hero::before{content:"";position:absolute;right:40px;top:40px;width:200px;height:200px;border-radius:50%;border:1px solid rgba(201,162,39,.15)}
  .hero .wrap{position:relative;z-index:2}
  .eyebrow{color:var(--gold);letter-spacing:3px;font-size:.85rem;text-transform:uppercase;margin-bottom:18px}
  h1{font-family:var(--serif);font-size:clamp(2.4rem,5.5vw,4rem);line-height:1.12;margin-bottom:20px;font-weight:600}
  h1 .hl{color:var(--gold)}
  .hero p.lead{font-size:clamp(1.05rem,2.2vw,1.3rem);max-width:640px;color:#d6d9e2;margin-bottom:34px}
  .hero-btns{display:flex;gap:16px;flex-wrap:wrap}
  .btn{display:inline-block;padding:14px 28px;border-radius:4px;font-weight:600;font-size:1rem;transition:.2s}
  .btn-solid{background:var(--gold);color:var(--navy)}
  .btn-solid:hover{background:var(--gold-2)}
  .btn-ghost{border:1px solid rgba(255,255,255,.4);color:#fff}
  .btn-ghost:hover{border-color:var(--gold);color:var(--gold)}
  .hero-meta{margin-top:48px;display:flex;gap:40px;flex-wrap:wrap;border-top:1px solid rgba(255,255,255,.12);padding-top:26px}
  .hero-meta .stat b{display:block;font-family:var(--serif);font-size:1.8rem;color:var(--gold)}
  .hero-meta .stat span{font-size:.85rem;color:#c7cbd5}

  /* Section base */
  section{padding:80px 0}
  .sec-head{margin-bottom:44px;max-width:680px}
  .kicker{color:var(--gold);letter-spacing:3px;font-size:.8rem;text-transform:uppercase;margin-bottom:12px;font-weight:600}
  .sec-head h2{font-family:var(--serif);font-size:clamp(1.8rem,3.4vw,2.5rem);color:var(--navy);line-height:1.2;margin-bottom:14px}
  .sec-head p{color:var(--muted)}

  /* About */
  .about-grid{display:grid;grid-template-columns:1.2fr 1fr;gap:48px;align-items:start}
  .about-text p{color:#4a4a46;margin-bottom:18px}
  .creds{background:#fff;border:1px solid var(--line);border-radius:8px;padding:26px}
  .creds h3{font-family:var(--serif);color:var(--navy);margin-bottom:16px;font-size:1.1rem}
  .creds ul{list-style:none}
  .creds li{display:flex;gap:12px;padding:10px 0;border-bottom:1px dashed var(--line);font-size:.95rem}
  .creds li:last-child{border-bottom:none}
  .creds li::before{content:"—";color:var(--gold);flex-shrink:0}

  /* Services */
  .services{background:#fff;border-top:1px solid var(--line);border-bottom:1px solid var(--line)}
  .svc-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px}
  .svc{background:var(--paper);border:1px solid var(--line);border-radius:8px;padding:28px;transition:.25s}
  .svc:hover{transform:translateY(-4px);border-color:var(--gold);box-shadow:0 12px 28px rgba(20,33,61,.08)}
  .svc .ic{font-family:var(--serif);font-size:1.6rem;color:var(--gold);margin-bottom:14px;line-height:1}
  .svc h3{font-family:var(--serif);color:var(--navy);font-size:1.15rem;margin-bottom:10px}
  .svc p{font-size:.92rem;color:var(--muted)}

  /* Portfolio */
  .pf-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px}
  .pf-card{background:#fff;border:1px solid var(--line);border-radius:8px;overflow:hidden;transition:.25s}
  .pf-card:hover{transform:translateY(-4px);box-shadow:0 12px 28px rgba(20,33,61,.08)}
  .pf-thumb{height:160px;display:flex;align-items:center;justify-content:center;color:rgba(255,255,255,.9);font-family:var(--serif);font-size:2rem}
  .pf-body{padding:22px}
  .pf-tag{display:inline-block;font-size:.72rem;letter-spacing:1px;text-transform:uppercase;color:var(--gold);font-weight:600;margin-bottom:8px}
  .pf-body h3{font-family:var(--serif);color:var(--navy);font-size:1.1rem;margin-bottom:8px}
  .pf-body p{font-size:.9rem;color:var(--muted)}

  /* Testimonials */
  .t-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:22px}
  .t-card{background:#fff;border:1px solid var(--line);border-left:3px solid var(--gold);border-radius:8px;padding:26px}
  .t-card p{font-family:var(--serif);font-style:italic;color:#3a3a36;margin-bottom:16px}
  .t-who{font-size:.9rem;color:var(--navy);font-weight:600}
  .t-who span{display:block;font-weight:400;color:var(--muted);font-size:.82rem}

  /* Contact */
  .contact{background:linear-gradient(135deg,var(--navy-2),var(--navy));color:#fff}
  .contact .sec-head h2{color:#fff}
  .contact .sec-head p{color:#c7cbd5}
  .contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:40px}
  .c-form{display:grid;gap:16px}
  .c-form input,.c-form textarea{width:100%;background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.2);border-radius:6px;padding:14px 16px;color:#fff;font-family:var(--sans);font-size:.95rem}
  .c-form input::placeholder,.c-form textarea::placeholder{color:#9aa0ad}
  .c-form input:focus,.c-form textarea:focus{outline:none;border-color:var(--gold)}
  .c-form button{border:none;cursor:pointer}
  .c-info{display:grid;gap:14px;align-content:start}
  .c-info .item{border-bottom:1px solid rgba(255,255,255,.12);padding:14px 0}
  .c-info .item b{display:block;color:var(--gold);font-size:.82rem;letter-spacing:1px;text-transform:uppercase;margin-bottom:4px}
  .c-info .item span{color:#e4e6ec}

  footer{background:var(--navy-2);color:#9aa0ad;padding:26px 0;font-size:.85rem;border-top:1px solid rgba(255,255,255,.08)}
  footer .wrap{display:flex;justify-content:space-between;flex-wrap:wrap;gap:12px}

  /* Responsive */
  @media(max-width:860px){
    .about-grid,.contact-grid{grid-template-columns:1fr}
    .svc-grid,.pf-grid{grid-template-columns:1fr 1fr}
    .nav-links{display:none;position:absolute;top:66px;left:0;right:0;background:var(--navy);flex-direction:column;padding:20px 24px;gap:18px}
    .nav-links.open{display:flex}
    .burger{display:block}
  }
  @media(max-width:560px){
    .svc-grid,.pf-grid,.t-grid{grid-template-columns:1fr}
    section{padding:60px 0}
  }
</style>
</head>
<body>

<header>
  <nav class="wrap">
    <a href="#top" class="brand"><b>Abuli</b> · Registrar</a>
    <div class="nav-links" id="navLinks">
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#contact" class="nav-cta">Contact</a>
    </div>
    <button class="burger" id="burger" aria-label="Menu">☰</button>
  </nav>
</header>

<main id="top">
  <!-- Hero -->
  <section class="hero">
    <div class="wrap">
      <div class="eyebrow">Registrar · Corporate Services · Commonwealth</div>
      <h1>Bringing order &amp; <span class="hl">governance</span> to your entity — across the Commonwealth.</h1>
      <p class="lead">I am Abuli, a registrar specialising in company &amp; entity formation, statutory compliance, and corporate governance for businesses operating in Commonwealth jurisdictions.</p>
      <div class="hero-btns">
        <a href="#portfolio" class="btn btn-solid">View Portfolio</a>
        <a href="#contact" class="btn btn-ghost">Get in Touch</a>
      </div>
      <div class="hero-meta">
        <div class="stat"><b>20+</b><span>Jurisdictions covered</span></div>
        <div class="stat"><b>500+</b><span>Entities registered</span></div>
        <div class="stat"><b>12</b><span>Years of practice</span></div>
      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about">
    <div class="wrap about-grid">
      <div class="about-text">
        <div class="sec-head" style="margin-bottom:20px">
          <div class="kicker">About</div>
          <h2>Registered to serve, meticulous by habit.</h2>
        </div>
        <p>As a registrar across Commonwealth jurisdictions, my work sits at the intersection of law, administration, and trust. Every entity I handle must be formed correctly, kept compliant, and governed cleanly — because for your business, the registry is where reputation begins.</p>
        <p>From incorporation and statutory registers to annual filings and governance frameworks, I provide a single, dependable point of accountability for your corporate records.</p>
        <p><em>Short intro to replace: tell visitors who you are, your background, and what drives your practice.</em></p>
      </div>
      <aside class="creds">
        <h3>Core Focus</h3>
        <ul>
          <li>Company &amp; entity formation</li>
          <li>Statutory registers &amp; records</li>
          <li>Annual returns &amp; compliance filings</li>
          <li>Corporate governance advisory</li>
          <li>Cross-border Commonwealth structuring</li>
          <li>Notarial &amp; apostille support</li>
        </ul>
      </aside>
    </div>
  </section>

  <!-- Services -->
  <section id="services" class="services">
    <div class="wrap">
      <div class="sec-head">
        <div class="kicker">Services</div>
        <h2>What I do</h2>
        <p>End-to-end registration and compliance support, tailored to the requirements of each Commonwealth jurisdiction.</p>
      </div>
      <div class="svc-grid">
        <div class="svc"><div class="ic">01</div><h3>Entity Formation</h3><p>Company, LLP, foundation and trust incorporation with accurate, jurisdiction-correct documentation.</p></div>
        <div class="svc"><div class="ic">02</div><h3>Statutory Compliance</h3><p>Timely annual returns, filings and filings calendars so you never miss a deadline.</p></div>
        <div class="svc"><div class="ic">03</div><h3>Corporate Governance</h3><p>Board records, resolutions and governance frameworks that keep decision-making clean and auditable.</p></div>
        <div class="svc"><div class="ic">04</div><h3>Register Maintenance</h3><p>Live statutory registers of members, directors and charges — accurate and inspection-ready.</p></div>
        <div class="svc"><div class="ic">05</div><h3>Cross-Border Structuring</h3><p>Guidance on where and how to hold entities across Commonwealth jurisdictions.</p></div>
        <div class="svc"><div class="ic">06</div><h3>Certification &amp; Apostille</h3><p>Notarisation, certification and apostille of corporate documents for international use.</p></div>
      </div>
    </div>
  </section>

  <!-- Portfolio -->
  <section id="portfolio">
    <div class="wrap">
      <div class="sec-head">
        <div class="kicker">Portfolio</div>
        <h2>Selected engagements</h2>
        <p>A snapshot of recent work. Replace each card with your own case studies, clients or projects.</p>
      </div>
      <div class="pf-grid">
        <article class="pf-card">
          <div class="pf-thumb" style="background:linear-gradient(135deg,#1a2f4e,#24406b)">A</div>
          <div class="pf-body">
            <span class="pf-tag">Formation</span>
            <h3>Case / Project title</h3>
            <p>One-line summary of the engagement, the jurisdiction and the outcome. Replace with your own details.</p>
          </div>
        </article>
        <article class="pf-card">
          <div class="pf-thumb" style="background:linear-gradient(135deg,#24406b,#1a2f4e)">B</div>
          <div class="pf-body">
            <span class="pf-tag">Compliance</span>
            <h3>Case / Project title</h3>
            <p>One-line summary of the engagement, the jurisdiction and the outcome. Replace with your own details.</p>
          </div>
        </article>
        <article class="pf-card">
          <div class="pf-thumb" style="background:linear-gradient(135deg,#1a2f4e,#24406b)">C</div>
          <div class="pf-body">
            <span class="pf-tag">Governance</span>
            <h3>Case / Project title</h3>
            <p>One-line summary of the engagement, the jurisdiction and the outcome. Replace with your own details.</p>
          </div>
        </article>
        <article class="pf-card">
          <div class="pf-thumb" style="background:linear-gradient(135deg,#24406b,#1a2f4e)">D</div>
          <div class="pf-body">
            <span class="pf-tag">Structuring</span>
            <h3>Case / Project title</h3>
            <p>One-line summary of the engagement, the jurisdiction and the outcome. Replace with your own details.</p>
          </div>
        </article>
        <article class="pf-card">
          <div class="pf-thumb" style="background:linear-gradient(135deg,#1a2f4e,#24406b)">E</div>
          <div class="pf-body">
            <span class="pf-tag">Apostille</span>
            <h3>Case / Project title</h3>
            <p>One-line summary of the engagement, the jurisdiction and the outcome. Replace with your own details.</p>
          </div>
        </article>
        <article class="pf-card">
          <div class="pf-thumb" style="background:linear-gradient(135deg,#24406b,#1a2f4e)">F</div>
          <div class="pf-body">
            <span class="pf-tag">Advisory</span>
            <h3>Case / Project title</h3>
            <p>One-line summary of the engagement, the jurisdiction and the outcome. Replace with your own details.</p>
          </div>
        </article>
      </div>
    </div>
  </section>

  <!-- Testimonials -->
  <section id="testimonials" style="background:#fff;border-top:1px solid var(--line);border-bottom:1px solid var(--line)">
    <div class="wrap">
      <div class="sec-head">
        <div class="kicker">Testimonials</div>
        <h2>What clients say</h2>
      </div>
      <div class="t-grid">
        <div class="t-card"><p>"Replacement testimonial — paste a client quote about your reliability, accuracy and service."</p><div class="t-who">Client Name <span>Company / Role</span></div></div>
        <div class="t-card"><p>"Replacement testimonial — paste a client quote about your reliability, accuracy and service."</p><div class="t-who">Client Name <span>Company / Role</span></div></div>
        <div class="t-card"><p>"Replacement testimonial — paste a client quote about your reliability, accuracy and service."</p><div class="t-who">Client Name <span>Company / Role</span></div></div>
        <div class="t-card"><p>"Replacement testimonial — paste a client quote about your reliability, accuracy and service."</p><div class="t-who">Client Name <span>Company / Role</span></div></div>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="contact">
    <div class="wrap">
      <div class="sec-head">
        <div class="kicker">Contact</div>
        <h2>Let's work together</h2>
        <p>Have an entity to form, or records to keep compliant? Get in touch — I'll respond promptly.</p>
      </div>
      <div class="contact-grid">
        <form class="c-form" onsubmit="return false;">
          <input type="text" placeholder="Your name" required />
          <input type="email" placeholder="Email address" required />
          <input type="text" placeholder="Subject" />
          <textarea rows="5" placeholder="How can I help?" required></textarea>
          <button class="btn btn-solid" type="submit">Send Message</button>
        </form>
        <div class="c-info">
          <div class="item"><b>Email</b><span>your.name@example.com</span></div>
          <div class="item"><b>Phone / WhatsApp</b><span>+000 0000 0000</span></div>
          <div class="item"><b>Location</b><span>Commonwealth jurisdiction / city</span></div>
          <div class="item"><b>Availability</b><span>Monday – Friday, 9:00–18:00</span></div>
        </div>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="wrap">
    <span>© <span id="year"></span> Abuli · Registrar &amp; Corporate Services</span>
    <span>Commonwealth · Corporate Records · Governance</span>
  </div>
</footer>

<script>
  // Mobile nav
  const burger=document.getElementById('burger');
  const links=document.getElementById('navLinks');
  burger.addEventListener('click',()=>links.classList.toggle('open'));
  links.querySelectorAll('a').forEach(a=>a.addEventListener('click',()=>links.classList.remove('open')));

  // Year
  document.getElementById('year').textContent=new Date().getFullYear();

  // Form: prevent default; optionally hook to a form service
  document.querySelector('.c-form').addEventListener('submit',function(e){
    e.preventDefault();
    alert('Form submitted! Connect this to your email service (e.g. Formspree, EmailJS) to actually receive messages.');
  });
</script>
</body>
</html>
<!-- （注：内容由AI生成） -->
