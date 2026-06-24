# Nicety-Web
Business Services Website
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

/* ── TOP BAR ── */
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

/* ── HERO ── */
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
.hero-title em {
font-style: italic;
color: var(--blue);
}
.hero-sub {
font-size: 16px;
color: var(--white-dim);
max-width: 480px;
margin: 0 auto 48px;
line-height: 1.7;
}

/* BOOK NOW — the main event */
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

/* CONTACT INFO HERO */
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

/* ── SECTION BASE ── */
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

/* ── SERVICES ── */
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
< truncated lines 227-469 >
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

<!-- REVIEWS -->
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
<div class="review-text">"Amazing customer service and results! I have two young kids who destroy my car but Kyle always brubgs it back to like! Efficient, kind, and reasonably priced!"</div>
<div class="review-author">Skylar M.</div>
</div>

</div>
</div>
<div class="scroll-hint">← Scroll for more reviews →</div>
</div>
</section>

<!-- BEFORE & AFTER -->
<section id="gallery">
<div class="section-inner">
<div class="section-eyebrow">Before & After</div>
<h2 class="section-title">See the Nicety<br><em>difference.</em></h2>
<div class="ba-track-wrap" id="baScroll">
<div class="ba-track">

<div class="ba-card">
<div class="ba-pair">
<div class="ba-img-wrap">
<img src="before1.jpg" alt="Before 1" onerror="this.src='https://images.unsplash.com/photo-1520340356584-f9917d1eea6f?w=400&q=70'">
<span class="ba-label">Before</span>
</div>
<div class="ba-img-wrap">
<img src="after1.jpg" alt="After 1" onerror="this.src='https://images.unsplash.com/photo-1607860108855-64acf2078ed9?w=400&q=70'">
<span class="ba-label after">After</span>
</div>
</div>
<div class="ba-caption">Paint Correction · Add your photo here</div>
</div>

<div class="ba-card">
<div class="ba-pair">
<div class="ba-img-wrap">
<img src="before2.jpg" alt="Before 2" onerror="this.src='https://images.unsplash.com/photo-1520340356584-f9917d1eea6f?w=400&q=70'">
<span class="ba-label">Before</span>
</div>
<div class="ba-img-wrap">
<img src="after2.jpg" alt="After 2" onerror="this.src='https://images.unsplash.com/photo-1558618666-fcd25c85cd64?w=400&q=70'">
<span class="ba-label after">After</span>
</div>
</div>
<div class="ba-caption">Ceramic Coating · Add your photo here</div>
</div>

<div class="ba-card">
<div class="ba-pair">
<div class="ba-img-wrap">
<img src="before3.jpg" alt="Before 3" onerror="this.src='https://images.unsplash.com/photo-1520340356584-f9917d1eea6f?w=400&q=70'">
<span class="ba-label">Before</span>
</div>
<div class="ba-img-wrap">
<img src="after3.jpg" alt="After 3" onerror="this.src='https://images.unsplash.com/photo-1607860108855-64acf2078ed9?w=400&q=70'">
<span class="ba-label after">After</span>
</div>
</div>
<div class="ba-caption">Interior Detail · Add your photo here</div>
</div>

<div class="ba-card">
<div class="ba-pair">
<div class="ba-img-wrap">
<img src="before4.jpg" alt="Before 4" onerror="this.src='https://images.unsplash.com/photo-1520340356584-f9917d1eea6f?w=400&q=70'">
<span class="ba-label">Before</span>
</div>
<div class="ba-img-wrap">
<img src="after4.jpg" alt="After 4" onerror="this.src='https://images.unsplash.com/photo-1617886903355-9354bb57751f?w=400&q=70'">
<span class="ba-label after">After</span>
</div>
</div>
<div class="ba-caption">Full Detail · Add your photo here</div>
</div>

<div class="ba-card">
<div class="ba-pair">
<div class="ba-img-wrap">
<img src="before5.jpg" alt="Before 5" onerror="this.src='https://images.unsplash.com/photo-1520340356584-f9917d1eea6f?w=400&q=70'">
<span class="ba-label">Before</span>
</div>
<div class="ba-img-wrap">
<img src="after5.jpg" alt="After 5" onerror="this.src='https://images.unsplash.com/photo-1503376780353-7e6692767b70?w=400&q=70'">
<span class="ba-label after">After</span>
</div>
</div>
<div class="ba-caption">Starlight Headliner · Add your photo here</div>
</div>

</div>
</div>
<div class="scroll-hint">← Scroll to see more →</div>
</div>
</section>

<!-- CTA -->
<section class="cta-section" id="book">
<div class="section-inner">
<div class="section-eyebrow">Ready to Book?</div>
<h2 class="section-title">We come to<br><em>you.</em></h2>
<p class="cta-sub">No shop drop-off. No waiting around. Just showroom results at your door.</p>
<a href="#" class="btn-book" id="bookingLink">Book Your Appointment</a>
<div class="cta-contact">
<a href="tel:3162083234">(316) 208-3234</a>
<a href="mailto:nicetymobile@gmail.com">nicetymobile@gmail.com</a>
</div>
</div>
</section>

<!-- FOOTER -->
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
// Drag to scroll for reviews
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
