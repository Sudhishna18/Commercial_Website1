# Ex02 Commercial Website
# Name : Sudhishna P
# Register Number : 212224040336
# Date: 30.10.2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aroma Roasters | Fresh Coffee Delivered</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- HEADER + NAVIGATION -->
  <header class="site-header">
    <nav class="navbar">
      <a href="#home" class="logo">Aroma Roasters</a>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#about">About Us</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a href="#account" class="btn-small">My Account</a></li>
      </ul>
    </nav>
  </header>

  <main>

    <!-- HOMEPAGE -->
    <section id="home" class="hero">
      <div class="hero-text">
        <h1>Coffee roasted this week, at your door by Friday</h1>
        <p>Single-estate beans from Coorg, Chikmagalur and Yercaud, roasted in small batches and packed the same day.</p>
        <a href="#products" class="btn">Shop coffee</a>
      </div>
      <div class="hero-image">
        <img src="https://images.unsplash.com/photo-1447933601403-0c6688de566e?auto=format&fit=crop&w=800&q=70"
             alt="Freshly roasted coffee beans in a scoop" loading="eager">
      </div>
    </section>

    <!-- PRODUCTS / SERVICES -->
    <section id="products" class="section">
      <h2>Our products</h2>
      <div class="cards">
        <article class="card">
          <img src="https://images.unsplash.com/photo-1559056199-641a0ac8b55e?auto=format&fit=crop&w=600&q=70" alt="Bag of medium roast coffee beans" loading="lazy">
          <div class="card-body">
            <h3>Coorg Medium Roast</h3>
            <p>Chocolate and toasted nut notes. Good for filter coffee and moka pot.</p>
            <div class="card-footer"><span class="price">₹449 / 250 g</span><a href="#account" class="btn-small">Add to cart</a></div>
          </div>
        </article>
        <article class="card">
          <img src="https://images.unsplash.com/photo-1514432324607-a09d9b4aefdd?auto=format&fit=crop&w=600&q=70" alt="Dark roast espresso in a cup" loading="lazy">
          <div class="card-body">
            <h3>Espresso Dark Blend</h3>
            <p>Full body with low acidity. Made for espresso machines and milk drinks.</p>
            <div class="card-footer"><span class="price">₹499 / 250 g</span><a href="#account" class="btn-small">Add to cart</a></div>
          </div>
        </article>
        <article class="card">
          <img src="https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?auto=format&fit=crop&w=600&q=70" alt="Cup of coffee on a wooden table" loading="lazy">
          <div class="card-body">
            <h3>Monthly Subscription</h3>
            <p>Two bags of your choice delivered on the first of every month. Pause any time.</p>
            <div class="card-footer"><span class="price">₹849 / month</span><a href="#account" class="btn-small">Subscribe</a></div>
          </div>
        </article>
      </div>
    </section>

    <!-- ABOUT US -->
    <section id="about" class="section about">
      <div class="about-image">
        <img src="https://images.unsplash.com/photo-1442512595331-e89e73853f31?auto=format&fit=crop&w=700&q=70" alt="Barista pouring coffee in a cafe" loading="lazy">
      </div>
      <div class="about-text">
        <h2>About us</h2>
        <p>Aroma Roasters started in 2018 as a two-person roastery in Chennai. We buy directly from small farms and pay them above market price.</p>
        <p>Every bag shows the farm, altitude and roast date, so you know exactly what you are drinking.</p>
        <ul class="stats">
          <li><strong>40+</strong> partner farms</li>
          <li><strong>12,000</strong> happy customers</li>
          <li><strong>48 hrs</strong> bean to dispatch</li>
        </ul>
      </div>
    </section>

    <!-- CONTACT DETAILS -->
    <section id="contact" class="section contact">
      <h2>Contact us</h2>
      <div class="contact-wrap">
        <ul class="contact-info">
          <li><strong>Address</strong>12, Poonamallee High Road, Avadi, Chennai 600054</li>
          <li><strong>Phone</strong>+91 98765 43210</li>
          <li><strong>Email</strong>hello@aromaroasters.example</li>
          <li><strong>Hours</strong>Mon to Sat, 9 am to 7 pm</li>
        </ul>
        <form class="form" onsubmit="event.preventDefault(); alert('Thanks! We will reply within one working day.');">
          <label for="c-name">Name</label>
          <input id="c-name" type="text" required>
          <label for="c-email">Email</label>
          <input id="c-email" type="email" required>
          <label for="c-msg">Message</label>
          <textarea id="c-msg" rows="4" required></textarea>
          <button type="submit" class="btn">Send message</button>
        </form>
      </div>
    </section>

    <!-- USER ACCOUNT -->
    <section id="account" class="section account">
      <h2>Sign in to your account</h2>
      <p class="lead">Track orders, manage your subscription and save your delivery address.</p>
      <form class="form form-narrow" onsubmit="event.preventDefault(); alert('Login form submitted (demo only).');">
        <label for="a-email">Email</label>
        <input id="a-email" type="email" required>
        <label for="a-pass">Password</label>
        <input id="a-pass" type="password" required>
        <button type="submit" class="btn">Sign in</button>
        <p class="small">New here? <a href="#account">Create an account</a></p>
      </form>
    </section>

  </main>

  <!-- FOOTER -->
  <footer class="site-footer">
    <div class="footer-top">
      <span class="logo">Aroma Roasters</span>
      <ul class="social">
        <li><a href="https://facebook.com" target="_blank" rel="noopener">Facebook</a></li>
        <li><a href="https://instagram.com" target="_blank" rel="noopener">Instagram</a></li>
        <li><a href="https://x.com" target="_blank" rel="noopener">X</a></li>
        <li><a href="https://youtube.com" target="_blank" rel="noopener">YouTube</a></li>
      </ul>
    </div>
    <p class="copy">&copy; 2026 Aroma Roasters. All rights reserved.</p>
  </footer>

</body>
</html>
```
CSS
```
/* ---------- GLOBAL STYLES ---------- */
:root {
  --green: #1f3d2b;
  --green-light: #2f5d43;
  --amber: #e0a526;
  --paper: #f7f7f2;
  --ink: #1d1d1b;
  --muted: #5d625c;
  --radius: 8px;
}

* { margin: 0; padding: 0; box-sizing: border-box; }

html { scroll-behavior: smooth; scroll-padding-top: 72px; }

body {
  font-family: "Segoe UI", Roboto, Arial, sans-serif;
  line-height: 1.6;
  color: var(--ink);
  background: var(--paper);
}

img { display: block; max-width: 100%; }
a { text-decoration: none; color: inherit; }
ul { list-style: none; }

h1, h2, h3 { font-family: Georgia, "Times New Roman", serif; line-height: 1.2; }
h2 { font-size: 2rem; margin-bottom: 1.5rem; color: var(--green); }

a:focus-visible, button:focus-visible, input:focus-visible, textarea:focus-visible {
  outline: 3px solid var(--amber);
  outline-offset: 2px;
}

/* ---------- BUTTONS ---------- */
.btn, .btn-small {
  display: inline-block;
  background: var(--amber);
  color: var(--ink);
  font-weight: 600;
  border: none;
  border-radius: var(--radius);
  cursor: pointer;
  transition: background 0.3s, transform 0.3s;
}
.btn { padding: 0.8rem 1.6rem; font-size: 1rem; }
.btn-small { padding: 0.4rem 0.9rem; font-size: 0.9rem; }
.btn:hover, .btn-small:hover { background: #f0b93f; transform: translateY(-2px); }

/* ---------- HEADER / NAVBAR (Flexbox) ---------- */
.site-header {
  position: sticky;
  top: 0;
  z-index: 10;
  background: var(--green);
  color: #fff;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  max-width: 1100px;
  margin: 0 auto;
  padding: 0.9rem 1.5rem;
}

.logo { font-family: Georgia, serif; font-size: 1.4rem; font-weight: bold; }

.nav-links { display: flex; align-items: center; gap: 1.5rem; flex-wrap: wrap; }

.nav-links a:not(.btn-small) { position: relative; padding: 0.2rem 0; }
.nav-links a:not(.btn-small)::after {
  content: "";
  position: absolute;
  left: 0; bottom: 0;
  width: 0; height: 2px;
  background: var(--amber);
  transition: width 0.3s;
}
.nav-links a:not(.btn-small):hover::after { width: 100%; }

/* ---------- SECTIONS ---------- */
.section {
  max-width: 1100px;
  margin: 0 auto;
  padding: 4rem 1.5rem;
}

/* ---------- HOMEPAGE / HERO ---------- */
.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 2.5rem;
  padding: 4rem 1.5rem;
  background: var(--green);
  color: #fff;
}
.hero-text, .hero-image { flex: 1; max-width: 540px; }
.hero-text { margin-left: auto; }
.hero-image { margin-right: auto; }
.hero h1 { font-size: 2.8rem; margin-bottom: 1rem; }
.hero p { font-size: 1.1rem; margin-bottom: 1.8rem; color: #dfe8e1; }
.hero-image img {
  width: 100%;
  height: 360px;
  object-fit: cover;
  border-radius: var(--radius);
  background: var(--green-light);
}

/* ---------- PRODUCTS ---------- */
.cards { display: flex; gap: 1.5rem; flex-wrap: wrap; }

.card {
  flex: 1 1 280px;
  display: flex;
  flex-direction: column;
  background: #fff;
  border: 1px solid #e3e4dc;
  border-radius: var(--radius);
  overflow: hidden;
  transition: transform 0.3s, box-shadow 0.3s;
}
.card:hover { transform: translateY(-6px); box-shadow: 0 10px 24px rgba(0, 0, 0, 0.12); }

.card img { width: 100%; height: 200px; object-fit: cover; background: #d9dccf; }

.card-body { display: flex; flex-direction: column; flex: 1; padding: 1.2rem; }
.card-body h3 { font-size: 1.25rem; margin-bottom: 0.5rem; }
.card-body p { color: var(--muted); margin-bottom: 1rem; }

.card-footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: auto;
}
.price { font-weight: 700; color: var(--green); }

/* ---------- ABOUT ---------- */
.about { display: flex; align-items: center; gap: 3rem; flex-wrap: wrap; }
.about-image { flex: 1 1 320px; }
.about-image img { width: 100%; height: 340px; object-fit: cover; border-radius: var(--radius); background: #d9dccf; }
.about-text { flex: 1 1 320px; }
.about-text p { margin-bottom: 1rem; color: var(--muted); max-width: 60ch; }

.stats { display: flex; gap: 2rem; flex-wrap: wrap; margin-top: 1.5rem; }
.stats li { display: flex; flex-direction: column; color: var(--muted); font-size: 0.9rem; }
.stats strong { font-family: Georgia, serif; font-size: 1.8rem; color: var(--green); }

/* ---------- CONTACT ---------- */
.contact { border-top: 1px solid #e3e4dc; }
.contact-wrap { display: flex; gap: 3rem; flex-wrap: wrap; }
.contact-info { flex: 1 1 280px; display: flex; flex-direction: column; gap: 1.2rem; }
.contact-info strong { display: block; color: var(--green); }
.contact .form { flex: 1 1 320px; }

/* ---------- FORMS ---------- */
.form { display: flex; flex-direction: column; gap: 0.5rem; }
.form label { font-weight: 600; font-size: 0.95rem; }
.form input, .form textarea {
  padding: 0.7rem 0.8rem;
  font: inherit;
  border: 1px solid #c9ccc0;
  border-radius: var(--radius);
  background: #fff;
  transition: border-color 0.3s, box-shadow 0.3s;
}
.form input:hover, .form textarea:hover { border-color: var(--green-light); }
.form button { align-self: flex-start; margin-top: 0.8rem; }
.small { font-size: 0.9rem; color: var(--muted); margin-top: 0.5rem; }
.small a { color: var(--green); text-decoration: underline; }

/* ---------- USER ACCOUNT ---------- */
.account { border-top: 1px solid #e3e4dc; display: flex; flex-direction: column; align-items: center; text-align: center; }
.lead { color: var(--muted); margin-bottom: 1.5rem; max-width: 50ch; }
.form-narrow { width: 100%; max-width: 380px; text-align: left; }

/* ---------- FOOTER ---------- */
.site-footer { background: var(--green); color: #dfe8e1; padding: 2rem 1.5rem; }
.footer-top {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 1rem;
  max-width: 1100px;
  margin: 0 auto 1rem;
}
.footer-top .logo { color: #fff; }
.social { display: flex; gap: 1.2rem; flex-wrap: wrap; }
.social a { padding-bottom: 2px; border-bottom: 2px solid transparent; transition: border-color 0.3s, color 0.3s; }
.social a:hover { color: var(--amber); border-color: var(--amber); }
.copy { text-align: center; font-size: 0.85rem; border-top: 1px solid var(--green-light); padding-top: 1rem; }

/* ---------- RESPONSIVE ---------- */
@media (max-width: 760px) {
  .navbar { flex-direction: column; gap: 0.6rem; }
  .nav-links { justify-content: center; gap: 1rem; }
  .hero { flex-direction: column; text-align: center; }
  .hero-text { margin-left: 0; }
  .hero-image { margin-right: 0; width: 100%; }
  .hero h1 { font-size: 2.1rem; }
  .footer-top { justify-content: center; }
}

@media (prefers-reduced-motion: reduce) {
  * { transition: none !important; scroll-behavior: auto !important; }
}
```


## OUTPUT
<img width="1917" height="1197" alt="Screenshot 2026-10-30 123008" src="https://github.com/user-attachments/assets/c717ff2b-ed7d-43ae-a481-55d470b1323c" />
<img width="1917" height="1197" alt="Screenshot 2026-10-30 123052" src="https://github.com/user-attachments/assets/4fb0a573-3969-4e04-922b-db936aeabc81" />
<img width="1916" height="1197" alt="Screenshot 2026-10-30 123208" src="https://github.com/user-attachments/assets/d80db1e1-d8c4-49cd-b60d-b881fcef08ad" />
<img width="1916" height="1198" alt="Screenshot 2026-10-30 123252" src="https://github.com/user-attachments/assets/29a5a699-2aa6-4fb5-870c-5f93487cbc72" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
