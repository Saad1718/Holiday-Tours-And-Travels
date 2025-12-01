# Holiday-Tours-And-Travels

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Paradise — Kerala Holiday Packages (Clone)</title>
  <meta name="description" content="Sample single-file responsive clone template for a Kerala tours & travels website." />
  <style>
    /* --------------------
       Simple, modern CSS (single-file)
       - responsive layout
       - grid cards for packages
       - hero with background image (replace with real image)
       - minimal, accessible markup
       -------------------- */
    :root{--accent:#0b8f6e;--dark:#0b2431;--muted:#667788}
    *{box-sizing:border-box}
    body{font-family:Inter,ui-sans-serif,system-ui,Segoe UI,Roboto,'Helvetica Neue',Arial;margin:0;color:#0b2431;line-height:1.45}
    a{color:var(--accent);text-decoration:none}
    img{max-width:100%;height:auto;display:block}

    header{background:#fff;position:sticky;top:0;z-index:40;border-bottom:1px solid #eef2f6}
    .container{max-width:1100px;margin:0 auto;padding:0 20px}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:14px 0}
    .brand{display:flex;align-items:center;gap:12px;font-weight:700}
    .brand .logo{width:48px;height:48px;border-radius:10px;background:linear-gradient(135deg,#0b8f6e,#046c52);display:flex;align-items:center;justify-content:center;color:#fff;font-size:18px}
    nav ul{list-style:none;display:flex;gap:18px;margin:0;padding:0;align-items:center}
    .btn{background:var(--accent);color:#fff;padding:10px 14px;border-radius:8px;border:0;cursor:pointer}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr;gap:24px;padding:48px 0;background-image:linear-gradient(rgba(11,34,49,0.35),rgba(11,34,49,0.35)),url('https://images.unsplash.com/photo-1506152983158-2e3b7f8f6e29?auto=format&fit=crop&w=1400&q=60');background-size:cover;background-position:center;color:#fff}
    .hero .wrap{padding:44px;border-radius:12px;background:linear-gradient(90deg,rgba(255,255,255,0.03),rgba(255,255,255,0.02))}
    .eyebrow{display:inline-block;background:rgba(255,255,255,0.08);padding:6px 10px;border-radius:999px;font-size:13px}
    .title{font-size:34px;margin:12px 0 8px}
    .lead{color:rgba(255,255,255,0.9);max-width:640px}
    .hero-cta{margin-top:18px;display:flex;gap:12px}

    /* Search area */
    .searchbar{background:#fff;padding:14px;border-radius:12px;display:flex;gap:8px;align-items:center;margin-top:14px}
    .searchbar input, .searchbar select{border:1px solid #e6eef4;padding:10px;border-radius:8px;flex:1}

    /* Packages */
    section{padding:56px 0}
    h2.section-title{font-size:22px;margin:0 0 14px}
    .grid-packages{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .card{background:#fff;border-radius:12px;overflow:hidden;box-shadow:0 6px 18px rgba(9,30,45,0.06);border:1px solid #eef2f6}
    .card .thumb{height:160px;background:#e9f6f0;display:block}
    .card .body{padding:14px}
    .tag{display:inline-block;padding:6px 8px;border-radius:8px;background:#effcf6;color:#046c52;font-weight:700;font-size:13px}
    .card h3{margin:8px 0 6px;font-size:16px}
    .meta{color:var(--muted);font-size:14px}
    .price{font-weight:800;font-size:18px}
    .actions{display:flex;gap:8px;margin-top:10px}

    /* Features */
    .features{display:flex;gap:18px;flex-wrap:wrap}
    .feature{background:#fff;padding:18px;border-radius:12px;flex:1;min-width:200px;box-shadow:0 6px 18px rgba(9,30,45,0.04)}

    /* Footer */
    footer{background:#06121a;color:#b6c6cd;padding:40px 0}
    footer a{color:#dff6ee}

    /* Responsiveness */
    @media (max-width:1000px){.grid-packages{grid-template-columns:repeat(2,1fr)}.title{font-size:28px}}
    @media (max-width:700px){.grid-packages{grid-template-columns:repeat(1,1fr)}.nav ul{display:none}.hero{padding:30px}.title{font-size:22px}}
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="logo">PK</div>
        <div>
          <div style="font-size:15px;">Paradise</div>
          <div style="font-size:12px;color:var(--muted);margin-top:2px">Kerala Holidays</div>
        </div>
      </div>
      <nav>
        <ul>
          <li><a href="#packages">Packages</a></li>
          <li><a href="#itineraries">Itineraries</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact" class="btn">Book Now</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container wrap">
        <span class="eyebrow">Best Seller</span>
        <h1 class="title">Kerala Holiday Packages — Backwaters, Hills & Beaches</h1>
        <p class="lead">Curated trips across Munnar, Alleppey houseboats, Thekkady wildlife and cosy coastal stays. Choose 2–10 day packages with hotels, transfers and optional add-ons.</p>

        <div class="searchbar" role="search" aria-label="Search packages">
          <input type="search" placeholder="Search by destination, e.g. Munnar, Alleppey" />
          <select aria-label="Days">
            <option>3 days</option>
            <option>4 days</option>
            <option selected>5 days</option>
            <option>7 days</option>
            <option>9 days</option>
          </select>
          <button class="btn">Find Packages</button>
        </div>
      </div>
    </section>

    <section class="container" id="packages">
      <h2 class="section-title">Popular Kerala Packages</h2>
      <div class="grid-packages" aria-live="polite">
        <!-- Card 1 -->
        <article class="card">
          <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1501785888041-af3ef285b470?auto=format&fit=crop&w=1200&q=60');background-size:cover;background-position:center"></div>
          <div class="body">
            <span class="tag">5 Days</span>
            <h3>Munnar — Alleppey Backwaters</h3>
            <p class="meta">Hills + Houseboat stay + Sightseeing</p>
            <div style="display:flex;justify-content:space-between;align-items:center;margin-top:12px">
              <div>
                <div class="price">₹12,499</div>
                <div style="font-size:13px;color:var(--muted)">Per person (starting)</div>
              </div>
              <div class="actions">
                <button class="btn">View</button>
                <a href="#contact" style="padding:10px 12px;border-radius:8px;background:#f3f7f6;border:1px solid #e6eef4">Enquire</a>
              </div>
            </div>
          </div>
        </article>

        <!-- Card 2 -->
        <article class="card">
          <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1526772662000-3f88f10405ff?auto=format&fit=crop&w=1200&q=60');background-size:cover;background-position:center"></div>
          <div class="body">
            <span class="tag">7 Days</span>
            <h3>Munnar — Thekkady — Kumarakom</h3>
            <p class="meta">Tea plantations, Wildlife & Backwaters</p>
            <div style="display:flex;justify-content:space-between;align-items:center;margin-top:12px">
              <div>
                <div class="price">₹18,299</div>
                <div style="font-size:13px;color:var(--muted)">Per person (starting)</div>
              </div>
              <div class="actions">
                <button class="btn">View</button>
                <a href="#contact" style="padding:10px 12px;border-radius:8px;background:#f3f7f6;border:1px solid #e6eef4">Enquire</a>
              </div>
            </div>
          </div>
        </article>

        <!-- Card 3 -->
        <article class="card">
          <div class="thumb" style="background-image:url('https://images.unsplash.com/photo-1505765050419-1a3f0859a7b1?auto=format&fit=crop&w=1200&q=60');background-size:cover;background-position:center"></div>
          <div class="body">
            <span class="tag">3 Days</span>
            <h3>Kovalam Beach Escape</h3>
            <p class="meta">Relaxing beach stay with Ayurvedic spa option</p>
            <div style="display:flex;justify-content:space-between;align-items:center;margin-top:12px">
              <div>
                <div class="price">₹6,799</div>
                <div style="font-size:13px;color:var(--muted)">Per person (starting)</div>
              </div>
              <div class="actions">
                <button class="btn">View</button>
                <a href="#contact" style="padding:10px 12px;border-radius:8px;background:#f3f7f6;border:1px solid #e6eef4">Enquire</a>
              </div>
            </div>
          </div>
        </article>

      </div>
    </section>

    <section class="container" id="itineraries">
      <h2 class="section-title">Why book with us?</h2>
      <div class="features" style="margin-top:12px">
        <div class="feature">
          <h4 style="margin:0 0 8px">Handpicked Hotels</h4>
          <p style="margin:0;color:var(--muted)">From budget stays to premium resorts — we choose based on reviews and location so you get a comfortable experience.</p>
        </div>
        <div class="feature">
          <h4 style="margin:0 0 8px">Expert Local Guides</h4>
          <p style="margin:0;color:var(--muted)">Knowledgeable drivers and guides who know the best viewpoints, hidden gems and local cuisine.</p>
        </div>
        <div class="feature">
          <h4 style="margin:0 0 8px">Flexible Itineraries</h4>
          <p style="margin:0;color:var(--muted)">Customize days and activities — add a houseboat night, spice plantation visit or wildlife safari.</p>
        </div>
      </div>
    </section>

    <section class="container" id="about" style="padding-bottom:40px">
      <h2 class="section-title">About the company</h2>
      <p style="color:var(--muted)">This is a sample single-file front-end template inspired by the Paradise Kerala website. Replace images and copy with your official content. The template focuses on accessibility, simple responsive layout and clear CTAs.</p>
    </section>

    <section class="container" id="contact" style="padding-bottom:80px">
      <h2 class="section-title">Get in touch & Book</h2>
      <form style="display:grid;grid-template-columns:1fr 1fr;gap:12px;max-width:820px;background:#fff;padding:18px;border-radius:12px;border:1px solid #eef2f6">
        <input placeholder="Full name" required />
        <input placeholder="Phone or WhatsApp" required />
        <input placeholder="Email (optional)" />
        <select>
          <option>Package of interest: 5 Days — Munnar/Alleppey</option>
          <option>7 Days — Munnar/Thekkady/Kumarakom</option>
          <option>3 Days — Kovalam Beach</option>
        </select>
        <textarea placeholder="Any special requests (houseboat, dietary, pickup)" style="grid-column:1/-1;padding:10px;border:1px solid #e6eef4;border-radius:8px"></textarea>
        <div style="grid-column:1/-1;display:flex;gap:10px;justify-content:flex-end">
          <button type="reset" style="padding:10px 14px;border-radius:8px;border:1px solid #e6eef4">Reset</button>
          <button type="submit" class="btn">Send Enquiry</button>
        </div>
      </form>
    </section>

  </main>

  <footer>
    <div class="container" style="display:flex;gap:20px;flex-wrap:wrap;align-items:flex-start;justify-content:space-between">
      <div style="max-width:420px">
        <h3 style="margin:0;color:#fff">Paradise — Kerala Holidays (Clone)</h3>
        <p style="margin-top:8px;color:#cfe9db">Address line • Phone: +91 99999 99999 • Email: info@example.com</p>
      </div>
      <div style="display:flex;gap:18px;flex-wrap:wrap">
        <div>
          <strong>Packages</strong>
          <ul style="list-style:none;padding:0;margin:8px 0 0;color:#b6c6cd">
            <li><a href="#packages">Munnar & Backwaters</a></li>
            <li><a href="#itineraries">Wildlife & Hill Stations</a></li>
            <li><a href="#contact">Group Tours</a></li>
          </ul>
        </div>
        <div>
          <strong>Follow</strong>
          <ul style="list-style:none;padding:0;margin:8px 0 0;color:#b6c6cd">
            <li><a href="#">Instagram</a></li>
            <li><a href="#">Facebook</a></li>
          </ul>
        </div>
      </div>
    </div>
  </footer>

</body>
</html>
