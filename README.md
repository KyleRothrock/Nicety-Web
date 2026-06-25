<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Premium mobile auto detailing, paint correction, ceramic coating, starlight headliners and more. We come to you in Wichita, KS. Call (316) 208-3234.">
<title>Nicety Auto Services — Premium Mobile Auto Care in Wichita, KS</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;600&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
 
:root {
--black: #0A0A0A;
--off-black: #111111;
--card: #161616;
--border: rgba(255,255,255,0.07);
--white: #F8F8F8;
--white-dim: rgba(248,248,248,0.55);
--blue: #3B82F6;
--blue-glow: rgba(59,130,246,0.35);
--blue-dim: rgba(59,130,246,0.12);
--yellow: #FACC15;
--display: 'Cormorant Garamond', serif;
--body: 'DM Sans', sans-serif;
}
 
html { scroll-behavior: smooth; }
 
body {
background: var(--black);
color: var(--white);
font-family: var(--body);
font-weight: 300;
line-height: 1.6;
-webkit-font-smoothing: antialiased;
}
 
.topbar {
background: rgba(10,10,10,0.95);
backdrop-filter: blur(12px);
border-bottom: 1px solid var(--border);
position: sticky;
top: 0;
z-index: 100;
padding: 14px 32px;
display: flex;
justify-content: space-between;
align-items: center;
}
.topbar-left {
font-family: var(--body);
font-size: 12px;
letter-spacing: 2px;
text-transform: uppercase;
color: var(--white-dim);
}
.topbar-right {
display: flex;
gap: 24px;
align-items: center;
}
.topbar-right a {
font-size: 13px;
color: var(--white-dim);
text-decoration: none;
transition: color 0.2s;
}
.topbar-right a:hover { color: var(--white); }
 
.hero {
min-height: 92vh;
display: flex;
flex-direction: column;
align-items: center;
justify-content: center;
text-align: center;
padding: 80px 24px 60px;
position: relative;
overflow: hidden;
}
.hero::before {
content: '';
position: absolute;
inset: 0;
background:
  radial-gradient(ellipse 70% 50% at 50% 20%, rgba(59,130,246,0.1) 0%, transparent 60%),
  radial-gradient(ellipse 50% 40% at 80% 80%, rgba(59,130,246,0.05) 0%, transparent 50%);
pointer-events: none;
}
.hero-logo {
width: 220px;
margin-bottom: 36px;
filter: brightness(1.05);
}
.hero-eyebrow {
font-size: 11px;
letter-spacing: 4px;
text-transform: uppercase;
color: var(--blue);
margin-bottom: 20px;
font-weight: 500;
}
.hero-title {
font-family: var(--display);
font-size: clamp(52px, 8vw, 96px);
font-weight: 300;
line-height: 1.0;
letter-spacing: -1px;
color: var(--white);
margin-bottom: 24px;
}
.hero-title em { font-style: italic; color: var(--blue); }
.hero-sub {
font-size: 16px;
color: var(--white-dim);
max-width: 480px;
margin: 0 auto 48px;
line-height: 1.7;
}
 
.btn-book {
display: inline-block;
padding: 22px 64px;
font-family: var(--body);
font-size: 16px;
font-weight: 600;
letter-spacing: 2.5px;
text-transform: uppercase;
text-decoration: none;
color: #fff;
background: var(--blue);
border-radius: 4px;
border: none;
cursor: pointer;
position: relative;
box-shadow:
  0 0 28px rgba(59,130,246,0.55),
  0 0 60px rgba(59,130,246,0.25),
  0 8px 32px rgba(59,130,246,0.3);
transition: transform 0.2s, box-shadow 0.2s;
margin-bottom: 48px;
}
.btn-book:hover {
transform: translateY(-2px);
box-shadow:
  0 0 40px rgba(59,130,246,0.7),
  0 0 80px rgba(59,130,246,0.35),
  0 12px 40px rgba(59,130,246,0.4);
}
 
.hero-contact {
display: flex;
gap: 40px;
flex-wrap: wrap;
justify-content: center;
}
.hero-contact a {
text-decoration: none;
display: flex;
flex-direction: column;
align-items: center;
gap: 4px;
}
.hero-contact .label {
font-size: 10px;
letter-spacing: 3px;
text-transform: uppercase;
color: var(--white-dim);
}
.hero-contact .value {
font-size: 22px;
font-weight: 600;
color: var(--white);
letter-spacing: 0.5px;
transition: color 0.2s;
}
.hero-contact a:hover .value { color: var(--blue); }
.hero-contact .value.blue { color: var(--blue); }
 
section { padding: 96px 24px; }
.section-inner { max-width: 1100px; margin: 0 auto; }
.section-eyebrow {
font-size: 10px;
letter-spacing: 4px;
text-transform: uppercase;
color: var(--blue);
font-weight: 500;
margin-bottom: 12px;
}
.section-title {
font-family: var(--display);
font-size: clamp(36px, 5vw, 58px);
font-weight: 300;
line-height: 1.1;
margin-bottom: 48px;
}
.section-title em { font-style: italic; color: var(--blue); }
 
.services-grid {
display: grid;
grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
gap: 2px;
}
.service-card {
background: var(--card);
border: 1px solid var(--border);
overflow: hidden;
position: relative;
transition: border-color 0.3s;
}
.service-card:hover { border-color: rgba(59,130,246,0.3); }
.service-card img {
width: 100%;
height: 200px;
object-fit: cover;
display: block;
filter: brightness(0.85);
transition: filter 0.3s, transform 0.4s;
}
.service-card:hover img { filter: brightness(1); transform: scale(1.03); }
.service-card-body { padding: 22px 24px 26px; }
.service-card-name {
font-family: var(--display);
font-size: 22px;
font-weight: 400;
margin-bottom: 8px;
letter-spacing: 0.3px;
}
.service-card-desc {
font-size: 13px;
color: var(--white-dim);
line-height: 1.65;
}
 
.reviews-section { background: var(--off-black); }
.reviews-track-wrap {
overflow-x: auto;
scrollbar-width: none;
cursor: grab;
-webkit-overflow-scrolling: touch;
}
.reviews-track-wrap::-webkit-scrollbar { display: none; }
.reviews-track {
display: flex;
gap: 16px;
padding-bottom: 12px;
width: max-content;
}
.review-card {
background: var(--card);
border: 1px solid var(--border);
border-radius: 4px;
padding: 28px 28px 24px;
width: 300px;
flex-shrink: 0;
}
.review-stars { color: var(--yellow); font-size: 16px; margin-bottom: 14px; letter-spacing: 2px; }
.review-text {
font-size: 13.5px;
color: var(--white-dim);
line-height: 1.7;
margin-bottom: 18px;
font-style: italic;
}
.review-author {
font-size: 12px;
font-weight: 600;
letter-spacing: 1px;
text-transform: uppercase;
color: var(--white);
}
.scroll-hint {
font-size: 11px;
letter-spacing: 2px;
color: rgba(255,255,255,0.2);
text-align: center;
margin-top: 20px;
text-transform: uppercase;
}
 
.ba-track-wrap {
overflow-x: auto;
scrollbar-width: none;
cursor: grab;
-webkit-overflow-scrolling: touch;
}
.ba-track-wrap::-webkit-scrollbar { display: none; }
.ba-track {
display: flex;
gap: 16px;
padding-bottom: 12px;
width: max-content;
}
.ba-card { width: 480px; flex-shrink: 0; }
.ba-pair {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 4px;
border-radius: 4px;
overflow: hidden;
}
.ba-img-wrap { position: relative; }
.ba-img-wrap img {
width: 100%;
height: 200px;
object-fit: cover;
display: block;
}
.ba-label {
position: absolute;
bottom: 10px;
left: 10px;
font-size: 10px;
letter-spacing: 2px;
text-transform: uppercase;
background: rgba(0,0,0,0.7);
color: var(--white);
padding: 4px 10px;
border-radius: 2px;
}
.ba-label.after { background: rgba(59,130,246,0.8); }
.ba-caption {
font-size: 12px;
color: var(--white-dim);
text-align: center;
margin-top: 10px;
letter-spacing: 1px;
}
 
.cta-section {
background: var(--blue-dim);
border-top: 1px solid rgba(59,130,246,0.2);
border-bottom: 1px solid rgba(59,130,246,0.2);
text-align: center;
padding: 80px 24px;
}
.cta-section .section-title { margin-bottom: 16px; }
.cta-sub {
font-size: 15px;
color: var(--white-dim);
margin-bottom: 40px;
max-width: 420px;
margin-left: auto;
margin-right: auto;
}
.cta-contact {
display: flex;
gap: 32px;
justify-content: center;
flex-wrap: wrap;
margin-top: 36px;
}
.cta-contact a {
font-size: 20px;
font-weight: 600;
color: var(--white);
text-decoration: none;
letter-spacing: 0.5px;
transition: color 0.2s;
}
.cta-contact a:hover { color: var(--blue); }
 
footer {
background: #080808;
border-top: 1px solid var(--border);
padding: 48px 24px;
text-align: center;
}
footer img { width: 140px; margin-bottom: 20px; opacity: 0.8; }
.footer-links {
display: flex;
gap: 24px;
justify-content: center;
flex-wrap: wrap;
margin-bottom: 20px;
}
.footer-links a {
font-size: 13px;
color: var(--white-dim);
text-decoration: none;
transition: color 0.2s;
}
.footer-links a:hover { color: var(--white); }
.footer-copy {
font-size: 11px;
color: rgba(255,255,255,0.2);
letter-spacing: 1px;
}
 
@media (max-width: 640px) {
.topbar { padding: 12px 16px; }
.topbar-left { font-size: 10px; }
section { padding: 64px 16px; }
.hero { padding: 60px 16px 48px; }
.hero-logo { width: 160px; }
.btn-book { padding: 18px 40px; font-size: 14px; }
.hero-contact .value { font-size: 17px; }
.ba-card { width: 320px; }
.review-card { width: 260px; }
}
</style>
</head>
<body>
 
<div class="topbar">
  <div class="topbar-left">📍 Wichita, KS & Surrounding Areas</div>
  <div class="topbar-right">
    <a href="tel:3162083234">(316) 208-3234</a>
    <a href="https://meetings-na2.hubspot.com/kyle-rothrock" target="_blank" style="color:#3B82F6; font-weight:500;">Book Now</a>
  </div>
</div>
 
<section class="hero">
  <img src="IMG_1648.jpeg" alt="Nicety Auto Services Logo" class="hero-logo">
  <div class="hero-eyebrow">Mobile Auto Care · Wichita, KS</div>
  <h1 class="hero-title">Your car deserves<br><em>Nicety.</em></h1>
  <p class="hero-sub">Professional detailing, paint correction, ceramic coating, and more — delivered to your home or office.</p>
  <a href="https://meetings-na2.hubspot.com/kyle-rothrock" target="_blank" class="btn-book">Book Now</a>
  <div class="hero-contact">
    <a href="tel:3162083234">
      <span class="label">Call or Text</span>
      <span class="value">(316) 208-3234</span>
    </a>
    <a href="mailto:nicetymobile@gmail.com">
      <span class="label">Email Us</span>
      <span class="value blue">nicetymobile@gmail.com</span>
    </a>
  </div>
</section>
 
<section id="services">
  <div class="section-inner">
    <div class="section-eyebrow">What We Do</div>
    <h2 class="section-title">Every service your<br>vehicle <em>deserves.</em></h2>
    <div class="services-grid">
 
      <div class="service-card">
        <img src="https://images.unsplash.com/photo-1607860108855-64acf2078ed9?w=600&q=80" alt="Mobile Detailing">
        <div class="service-card-body">
          <div class="service-card-name">Mobile Detailing</div>
          <div class="service-card-desc">Full interior & exterior detail at your home or office. We bring everything — you just unlock the car.</div>
        </div>
      </div>
 
      <div class="service-card">
        <img src="https://images.unsplash.com/photo-1617886903355-9354bb57751f?w=600&q=80" alt="Paint Correction">
        <div class="service-card-body">
          <div class="service-card-name">Paint Correction</div>
          <div class="service-card-desc">Remove swirl marks, scratches, and oxidation. Restore your paint to a deeper, truer shine than the day you bought it.</div>
        </div>
      </div>
 
      <div class="service-card">
        <img src="https://images.unsplash.com/photo-1558618666-fcd25c85cd64?w=600&q=80" alt="Ceramic Coating">
        <div class="service-card-body">
          <div class="service-card-name">Ceramic Coating</div>
          <div class="service-card-desc">Nano-ceramic protection that bonds to your paint — repels water, dirt, and UV damage for years.</div>
        </div>
      </div>
 
      <div class="service-card">
        <img src="https://images.unsplash.com/photo-1503376780353-7e6692767b70?w=600&q=80" alt="Starlight Headliner">
        <div class="service-card-body">
          <div class="service-card-name">Starlight Headliners</div>
          <div class="service-card-desc">Transform your interior with a custom fiber-optic starlight ceiling. The install everyone talks about.</div>
        </div>
      </div>
 
      <div class="service-card">
        <img src="https://images.unsplash.com/photo-1562141961-b8ab0ce9d10a?w=600&q=80" alt="Window Tint">
        <div class="service-card-body">
          <div class="service-card-name">Window Tint</div>
          <div class="service-card-desc">Premium films for heat rejection, UV protection, and a clean blacked-out look.</div>
        </div>
      </div>
 
      <div class="service-card">
        <img src="https://images.unsplash.com/photo-1611016186353-9af58c69a533?w=600&q=80" alt="Vehicle Wraps">
        <div class="service-card-body">
          <div class="service-card-name">Wraps</div>
          <div class="service-card-desc">Full and partial vehicle wraps in any color or finish — matte, gloss, satin, or chrome.</div>
        </div>
      </div>
 
      <div class="service-card">
        <img src="https://images.unsplash.com/photo-1545259741-2ea3ebf61fa3?w=600&q=80" alt="Audio Install">
        <div class="service-card-body">
          <div class="service-card-name">Audio Install</div>
          <div class="service-card-desc">Custom audio systems — head units, speakers, subwoofers, and amplifiers installed clean.</div>
        </div>
      </div>
 
    </div>
  </div>
</section>
 
<section class="reviews-section" id="reviews">
  <div class="section-inner">
    <div class="section-eyebrow">Customer Reviews</div>
    <h2 class="section-title">What Wichita<br><em>is saying.</em></h2>
    <div class="reviews-track-wrap" id="reviewsScroll">
      <div class="reviews-track">
 
        <div class="review-card">
          <div class="review-stars">★★★★★</div>
          <div class="review-text">"Kyle did an amazing job and would highly recommend them to everyone. They came and picked up my car and delivered it looking brand new!"</div>
          <div class="review-author">Shawna P.</div>
        </div>
 
        <div class="review-card">
          <div class="review-stars">★★★★★</div>
          <div class="review-text">"Man, I feel like i'm in a new vehicle fresh from the car dealership! Highly Recomment!!"</div>
          <div class="review-author">Mark M.</div>
        </div>
 
        <div class="review-card">
          <div class="review-stars">★★★★★</div>
          <div class="review-text">"Qaulity work and amazing attention to detail done in a timely fasion. Very good value would highly recommend to anyone."</div>
          <div class="review-author">Angelo C.</div>
        </div>
 
        <div class="review-card">
          <div class="review-stars">★★★★★</div>
          <div class="review-text">"Kyle from Nicety came out and did an excellent job on a full detail on my Ram and Ford. Going to be using this company again!"</div>
          <div class="review-author">Dakota C.</div>
        </div>
 
        <div class="review-card">
          <div class="review-stars">★★★★★</div>
          <div class="review-text">"Did an amazing job on my vehicle! Would totally recommend, Super nice and responsive as well!"</div>
          <div class="review-author">Jason S.</div>
        </div>
 
        <div class="review-card">
          <div class="review-stars">★★★★★</div>
          <div class="review-text">"Amazing customer service and results! I have two young kids who destroy my car but Kyle always brings it back to life! Efficient, kind, and reasonably priced!"</div>
          <div class="review-author">Skylar M.</div>
        </div>
 
      </div>
    </div>
    <div class="scroll-hint">← Scroll for more reviews →</div>
  </div>
</section>
 
<section id="gallery">
  <div class="section-inner">
    <div class="section-eyebrow">Before & After</div>
    <h2 class="section-title">See the Nicety<br><em>difference.</em></h2>
    <div class="ba-track-wrap" id="baScroll">
      <div class="ba-track">
 
        <div class="ba-card">
          <div class="ba-pair">
            <div class="ba-img-wrap">
              <img src="before1.png" alt="Before 1">
              <span class="ba-label">Before</span>
            </div>
            <div class="ba-img-wrap">
              <img src="after1.jpg" alt="After 1">
              <span class="ba-label after">After</span>
            </div>
          </div>
          <div class="ba-caption">Job 1 — Edit this caption</div>
        </div>
 
        <div class="ba-card">
          <div class="ba-pair">
            <div class="ba-img-wrap">
              <img src="before3.png" alt="Before 3">
              <span class="ba-label">Before</span>
            </div>
            <div class="ba-img-wrap">
              <img src="after3.png" alt="After 3">
              <span class="ba-label after">After</span>
            </div>
          </div>
          <div class="ba-caption">Job 3 — Edit this caption</div>
        </div>
 
        <div class="ba-card">
          <div class="ba-pair">
            <div class="ba-img-wrap">
              <img src="before5.png" alt="Before 5">
              <span class="ba-label">Before</span>
            </div>
            <div class="ba-img-wrap">
              <img src="after5.png" alt="After 5">
              <span class="ba-label after">After</span>
            </div>
          </div>
          <div class="ba-caption">Job 5 — Edit this caption</div>
        </div>
 
        <div class="ba-card">
          <div class="ba-pair">
            <div class="ba-img-wrap">
              <img src="before6.png" alt="Before 6">
              <span class="ba-label">Before</span>
            </div>
            <div class="ba-img-wrap">
              <img src="after6.png" alt="After 6">
              <span class="ba-label after">After</span>
            </div>
          </div>
          <div class="ba-caption">Job 6 — Edit this caption</div>
        </div>
 
        <div class="ba-card">
          <div class="ba-pair">
            <div class="ba-img-wrap">
              <img src="before7.png" alt="Before 7">
              <span class="ba-label">Before</span>
            </div>
            <div class="ba-img-wrap">
              <img src="after7.png" alt="After 7">
              <span class="ba-label after">After</span>
            </div>
          </div>
          <div class="ba-caption">Job 7 — Edit this caption</div>
        </div>
 
      </div>
    </div>
    <div class="scroll-hint">← Scroll to see more →</div>
  </div>
</section>
 
<section class="cta-section" id="book">
  <div class="section-inner">
    <div class="section-eyebrow">Ready to Book?</div>
    <h2 class="section-title">We come to<br><em>you.</em></h2>
    <p class="cta-sub">No shop drop-off. No waiting around. Just showroom results at your door.</p>
    <a href="https://meetings-na2.hubspot.com/kyle-rothrock" target="_blank" class="btn-book">Book Your Appointment</a>
    <div class="cta-contact">
      <a href="tel:3162083234">(316) 208-3234</a>
      <a href="mailto:nicetymobile@gmail.com">nicetymobile@gmail.com</a>
    </div>
  </div>
</section>
 
<footer>
  <img src="IMG_1648.jpeg" alt="Nicety Auto Services">
  <div class="footer-links">
    <a href="tel:3162083234">(316) 208-3234</a>
    <a href="mailto:nicetymobile@gmail.com">nicetymobile@gmail.com</a>
    <a href="https://www.facebook.com/share/18n3ppVXmS/?mibextid=wwXIfr" target="_blank">Facebook</a>
    <a href="#services">Services</a>
    <a href="#reviews">Reviews</a>
    <a href="#book">Book Now</a>
  </div>
  <div class="footer-copy">© 2026 Nicety Auto Services · Wichita, KS · All rights reserved.</div>
</footer>
 
<script>
function dragScroll(el) {
  let isDown = false, startX, scrollLeft;
  el.addEventListener('mousedown', e => { isDown = true; el.style.cursor = 'grabbing'; startX = e.pageX - el.offsetLeft; scrollLeft = el.scrollLeft; });
  el.addEventListener('mouseleave', () => { isDown = false; el.style.cursor = 'grab'; });
  el.addEventListener('mouseup', () => { isDown = false; el.style.cursor = 'grab'; });
  el.addEventListener('mousemove', e => { if (!isDown) return; e.preventDefault(); const x = e.pageX - el.offsetLeft; el.scrollLeft = scrollLeft - (x - startX) * 1.5; });
}
dragScroll(document.getElementById('reviewsScroll'));
dragScroll(document.getElementById('baScroll'));
</script>
 
</body>
</html>
