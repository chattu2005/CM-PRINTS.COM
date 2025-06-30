<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CM PRINTS & STATIONERY</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-900 text-white">

  <!-- Header Section -->
  <header class="bg-gray-800 shadow-lg fixed w-full z-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between h-16 items-center">
        
        <!-- Logo -->
        <div class="flex-shrink-0 text-xl font-bold tracking-wide text-yellow-400"> <img width="100 px"src="LOGO CM PTINTS & STATIONERY.png" alt="">
          CM PRINTS & STATIONERY
        </div>
        
        <!-- Desktop Nav -->
        <nav class="hidden md:flex space-x-6 text-sm font-medium">
          <a href="#" class="hover:text-yellow-400 transition">Home</a>
          <a href="#" class="hover:text-yellow-400 transition">Services</a>
          <a href="#" class="hover:text-yellow-400 transition">Products</a>
          <a href="#" class="hover:text-yellow-400 transition">Contact</a>
        </nav>

        <!-- Call Now Button -->
        <div class="hidden md:block">
          <a href="tel:+91 9330713861" class="bg-yellow-500 hover:bg-yellow-400 text-black px-4 py-2 rounded-lg text-sm font-semibold transition">
            Call Now
          </a>
        </div>

        <!-- Mobile Menu Icon -->
        <div class="md:hidden">
          <button id="mobile-menu-button" class="focus:outline-none">
            <svg class="w-6 h-6 text-yellow-400" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16"/>
            </svg>
          </button>
        </div>

      </div>
    </div>

    <!-- Mobile Menu -->
    <div id="mobile-menu" class="md:hidden hidden bg-gray-700">
      <nav class="flex flex-col space-y-2 py-4 px-4">
        <a href="#" class="hover:text-yellow-400 transition">Home</a>
        <a href="#" class="hover:text-yellow-400 transition">Services</a>
        <a href="#" class="hover:text-yellow-400 transition">Products</a>
        <a href="#" class="hover:text-yellow-400 transition">Contact</a>
        <a href="tel:+91 9330713861" class="bg-yellow-500 text-black px-4 py-2 mt-2 rounded-md text-center font-semibold hover:bg-yellow-400 transition">
          Call Now
        </a>
      </nav>
    </div>
  </header>

   <!-- === Dark‑theme Hero Styles === -->
  <style>
    :root {
      --clr-bg: #0f1117;         /* page background */
      --clr-primary: #facc15;    /* golden accent */
      --clr-text: #f3f4f6;       /* base text */
      --clr-muted: #9ca3af;      /* muted text */
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { background: var(--clr-bg); color: var(--clr-text); font-family: system-ui, sans-serif; }

    /* ===== Hero Section ===== */
    .hero {
      min-height: 100vh;                        /* full viewport height */
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 0 1.5rem;
      text-align: center;
      position: relative;
      overflow: hidden;
    }
    /* background image + dark overlay */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background:
        linear-gradient(rgba(6, 35, 121, 0.356), rgba(15, 27, 31, 0.9)),
        url("https://images.unsplash.com/photo-1525547719571-a2d4ac8945e2?w=700&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8Y29tcHV0ZXJ8ZW58MHx8MHx8fDA%3D");
      background-size: cover;
      background-position: center;
      z-index: -1;
    }

    .hero h1 {
      font-size: clamp(2.25rem, 6vw + 1rem, 4rem);
      font-weight: 800;
      line-height: 1.15;
    }
    .hero p {
      max-width: 38rem;
      margin: 1rem auto 2rem;
      font-size: clamp(1rem, 1.25vw + .65rem, 1.3rem);
      color: var(--clr-muted);
    }

    .cta {
      display: inline-block;
      padding: 1rem 2.5rem;
      border-radius: .65rem;
      font-weight: 700;
      font-size: 1rem;
      color: #ca2424ea;
      background: var(--clr-primary);
      transition: background .25s;
    }
    .cta:hover { background: #61e93f; }

    /* optional subtle scroll cue */
    .scroll-cue {
      position: absolute;
      bottom: 1.25rem;
      left: 50%;
      translate: -50% 0;
      font-size: .85rem;
      letter-spacing: .05em;
      color: var(--clr-muted);
      animation: bounce 2.5s infinite;
    }
    @keyframes bounce {
      0%, 20%, 50%, 80%, 100% { transform: translate(-50%, 0); }
      40%                      { transform: translate(-50%, -8px); }
      60%                      { transform: translate(-50%, -4px); }
    }

    /* small screens tweak */
    @media (max-width: 480px) {
      .hero h1 { font-size: 2rem; }
    }
  </style>
</head>

<body>

  <!-- ===== HERO SECTION ===== -->
  <section class="hero" id="home">
    <div>
      <h1>Your One‑Stop Print &amp; Stationery Item</h1>
      <p>Fast, high‑quality prints, comprehensive stationery, and friendly service—all in one place.</p>
      <a href="tel:+91 9330713861" class="cta">Call&nbsp;&nbsp;Now</a>
    </div>
    <span class="scroll-cue">▼ Scroll</span>
  </section>


  <script>
    // Toggle mobile menu
    const btn = document.getElementById('mobile-menu-button');
    const menu = document.getElementById('mobile-menu');

    btn.addEventListener('click', () => {
      menu.classList.toggle('hidden');
    });
  </script>


<!-- ========== Our Services Section ========== -->
<style>
  :root {
    /* (reuse the same palette used in header/hero) */
    --clr-bg:       #5974c5;
    --clr-surface:  #253458;
    --clr-primary:  #facc15;
    --clr-text:     #f3f4f6;
    --clr-text-muted:#9ca3af;
  }

  .services {
    background: var(--clr-bg);
    padding: 4.5rem 1.25rem;
    text-align: center;
  }
  .services h2 {
    font-size: clamp(1.75rem, 3vw + .5rem, 2.5rem);
    font-weight: 800;
    margin-bottom: .75rem;
  }
  .services p.lead {
    color: var(--clr-text-muted);
    max-width: 38rem;
    margin: 0 auto 2.75rem;
    font-size: 1rem;
    line-height: 1.6;
  }

  /* ===== Card Grid ===== */
  .service-grid {
    display: grid;
    gap: 1.75rem;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    max-width: 1100px;
    margin-inline: auto;
  }

  .service-card {
    background: var(--clr-surface);
    border-radius: .85rem;
    padding: 2.25rem 1.75rem;
    box-shadow: 0 4px 10px rgba(0,0,0,.35);
    transition: transform .3s ease, box-shadow .3s ease;
  }
  .service-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 8px 18px rgba(0,0,0,.45);
  }

  .service-card svg {
    width: 40px;
    height: 40px;
    margin-bottom: 1rem;
    fill: var(--clr-primary);
  }
  .service-card h3 {
    font-size: 1.125rem;
    font-weight: 700;
    margin-bottom: .5rem;
  }
  .service-card p {
    font-size: .95rem;
    color: var(--clr-text-muted);
    line-height: 1.55;
  }
</style>

<section class="services" id="services">
  <h2>Our Services</h2>
  <p class="lead">Fast, affordable and high‑quality solutions for every printing and stationery need.</p>

  <div class="service-grid">

    <!-- Service 1 -->
    <div class="service-card">
      <!-- Xerox icon -->
       <img src="https://images.unsplash.com/photo-1650094980833-7373de26feb6?w=700&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8eGVyb3h8ZW58MHx8MHx8fDA%3D" alt="">
      <svg viewBox="0 0 24 24"><path d="M4 16h16v2H4v-2zm2-6h12v2H6v-2zm0-4h12v2H6V6z"/></svg>
      <h3>Xerox / Photocopy</h3>
      <p>Crisp black‑and‑white or colour copies while you wait, at the best price in town.</p>
    </div>

    <!-- Service 2 -->
    <div class="service-card">
      <!-- Printer icon -->
       <img src="data:image/webp;base64,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" alt="">
      <svg viewBox="0 0 24 24"><path d="M6 9V4h12v5h2a2 2 0 012 2v6h-4v3H8v-3H4v-6a2 2 0 012-2h0zM8 5v3h8V5H8zm8 11H8v4h8v-4z"/></svg>
      <h3>Colour &amp; B/W Prints</h3>
      <p>High‑resolution prints up to A4 on premium or regular paper—perfect for projects &amp; photos.</p>
    </div>

    <!-- Service 3 -->
    <div class="service-card">
      <!-- Notebook icon -->
       <img src="data:image/webp;base64,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" alt="">
      <svg viewBox="0 0 24 24"><path d="M6 2h9a2 2 0 012 2v16a2 2 0 01-2 2H6a2 2 0 01-2-2V4a2 2 0 012-2zm0 2v16h9V4H6zm10 2h2v12h-2V6z"/></svg>
      <h3>Stationery Supplies</h3>
      <p>All school &amp; office essentials—pens, notebooks, art tools, files, and more.</p>
    </div>

    <!-- Service 4 -->
    <div class="service-card">
      <!-- Laminator icon -->
       <img src="https://th.bing.com/th/id/OIP.ThKReNo4K-ZlINO-ZQHs4wHaG6?w=160&h=180&c=7&r=0&o=7&pid=1.7&rm=3" alt="">
      <svg viewBox="0 0 24 24"><path d="M3 17h18v2H3v-2zm2-9h14a2 2 0 012 2v3H3v-3a2 2 0 012-2zm2-4h10v2H7V4z"/></svg>
      <h3>Lamination</h3>
      <p>Protect important documents or give your project a professional finish.</p>
    </div>

    <!-- Service 5 -->
    <div class="service-card">
      <!-- Scanner icon -->
       <img src="https://media.istockphoto.com/id/157618089/photo/using-copier.webp?a=1&b=1&s=612x612&w=0&k=20&c=UgadhH9uUqWjq2oxFnVm2MZtYsfKX9hNbwt5wjTsXoY=" alt="">
      <svg viewBox="0 0 24 24"><path d="M4.2 4.4l14.5 5-1 2.4-14.5-5 1-2.4zm-1.2 7h18v2H3v-2zm0 4h18v4H3v-4z"/></svg>
      <h3>Document Scanning</h3>
      <p>Get clear, high‑resolution PDFs sent straight to your email or phone—instantly.</p>
    </div>

    <!-- Service 6 -->
    <div class="service-card">
      <!-- Invitation icon -->
       <img src="https://images.unsplash.com/photo-1658863025658-4a259cc68fc9?w=700&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8NHx8Q3VzdG9tJTIwRGVzaWducyUyMCUyNiUyMEludml0YXRpb25zfGVufDB8fDB8fHww" alt="">
      <svg viewBox="0 0 24 24"><path d="M4 4h16v2H4V4zm0 4h16v10H4V8zm8 2l6 4h-12l6-4z"/></svg>
      <h3>Custom Designs &amp; Invitations</h3>
      <p>Bespoke wedding cards, business cards, banners &amp; more—designed and printed in‑house.</p>
    </div>

     <!-- Service 7 -->
    <div class="service-card">
      <!-- Aadhar card -->
       <img src="https://www.pgurus.com/wp-content/uploads/2022/12/Aadhar-Card-holders-urged-to-update-details-1.jpg" alt="">
      <h3>Aadhar Card Update/ Print </h3>
      <p>Need to update or print your Aadhar card? We provide fast, reliable, and hassle-free Aadhar card services. Whether it's correcting your name, address, date of birth, mobile number, or simply printing a new copy — we've got you covered.</p>
    </div>

     <!-- Service 8 -->
    <div class="service-card">
      <!-- Pan Card icon -->
       <img src="https://www.indezon.in/images/pan-card.png" alt="">
      <h3>Pan Card Services </h3>
      <p>We offer complete PAN Card services with quick processing and reliable support. Whether you're applying for a new PAN, updating/correcting existing details, or reprinting a lost/damaged card, we make the process smooth and hassle-free.</p>
    </div>

     <!-- Service 9 -->
    <div class="service-card">
      <!-- Voter Card icon -->
       <img src="https://www.shutterstock.com/shutterstock/photos/2438950119/display_1500/stock-vector-indian-voter-identification-card-vector-illustration-on-transprent-background-2438950119.jpg" alt="">
      <h3>Voter ID Card </h3>
      <p>Get your Voter ID made or updated with our fast and trusted services. Whether you're applying for a new Voter ID, making corrections, or reprinting a lost card, we’re here to help at every step.</p>
    </div>

     <!-- Service 10 -->
    <div class="service-card">
      <!-- Electricity bill icon -->
       <img src="https://i1.wp.com/technofizi.net/wp-content/uploads/2017/08/Bill-1.jpg?fit=1317%2C752&ssl=1" alt="">
      <h3>Electricity bill Payment </h3>
      <p>Pay your electricity bills quickly and securely with our convenient service. We support all major electricity boards and ensure real-time bill processing with instant receipts.</p>
    </div>

     <!-- Service 11 -->
    <div class="service-card">
      <!-- Mobile Recharge icon -->
       <img src="https://biznext.in/blog/wp-content/uploads/2024/04/Important-Features-of-Mobile-Recharge-Software-1024x536.webp" alt="">
      <h3>Mobile Recharge </h3>
      <p>Get fast and reliable mobile recharges for all major networks — prepaid or postpaid. We offer instant top-ups with flexible payment options.</p>
    </div>

     <!-- Service 12 -->
    <div class="service-card">
      <!-- Online From icon -->
       <img src="https://www.upform.com/blog/wp-content/uploads/2022/12/word-image-911-2-1024x683.png" alt="">
      <h3>Online From Filling </h3>
      <p>We provide expert assistance in filling out all types of online forms with accuracy and care. Whether it's for government schemes, exams, jobs, or official documents — we make the process easy for you.</p>
    </div>

     <!-- Service 13 -->
    <div class="service-card">
      <!-- Banking icon -->
       <img src="https://tse1.mm.bing.net/th/id/OIP.-OcggKhXncgeXVWtXdHamgHaEM?rs=1&pid=ImgDetMain&o=7&rm=3" alt="">
      <h3>Banking Services (AEPS,Cash Withdrawal, Blance Chack) </h3>
      <p>Now access essential banking services without visiting the bank! Using Aadhaar Enabled Payment System (AEPS), we provide secure and instant banking solutions right at our center.</p>
    </div>

     <!-- Service 14 -->
    <div class="service-card">
      <!-- IRTC icon -->
       <img src="https://5.imimg.com/data5/KJ/RQ/GLADMIN-61219190/travel-booking-air-train-bus-500x500.png" alt="">
      <h3>Railway/ Bus/ Flight Ticket Booking </h3>
      <p>Travel made easy! We offer hassle-free ticket booking services for trains, buses, and flights — all in one place. Get the best fares with confirmed bookings and instant support.</p>
    </div>

     <!-- Service 15 -->
    <div class="service-card">
      <!-- Insurance icon -->
       <img src="https://blog.geojit.com/wp-content/uploads/2020/12/iStock-1226082621-1920x1280.jpg" alt="">
      <h3>Insurance Services </h3>
      <p>Protect what matters most with our reliable insurance services. We help you choose and apply for the right plans — whether it’s life, health, vehicle, or general insurance — all under one roof.</p>
    </div>

     <!-- Service 16 -->
    <div class="service-card">
      <!-- passport size icon -->
       <img src="https://tse1.mm.bing.net/th/id/OIP.9NVomQn_Od73lWaKiTrrLAHaD4?rs=1&pid=ImgDetMain&o=7&rm=3" alt="">
      <h3>Passport Size Photo </h3>
      <p>Get high-quality passport size photos instantly for all your official and personal needs. Perfect for ID cards, forms, exams, passports, visas, and more.</p>
    </div>

     <!-- Service 17 -->
    <div class="service-card">
      <!-- EPF/ ESI icon -->
       <img src="https://admin.tfs-app.com/images/blogs/d508fcd1f73f4e128841142c784e6227.jpg?ver=12242022012044" alt="">
      <h3>EPF/ ESI Services </h3>
      <p>We offer expert support for all your EPF (Employees' Provident Fund) and ESI (Employees' State Insurance) needs — ensuring smooth processing and complete documentation.</p>
    </div>

     <!-- Service 18 -->
    <div class="service-card">
      <!-- DATA Entry icon -->
       <img src="https://www.suntecindia.com/blog/wp-content/uploads/2022/10/Data-Entry-Services-1024x536.png" alt="">
      <h3>DATA Entry Services </h3>
      <p>Fast, accurate, and reliable data entry solutions for all your personal and business needs.</p>
    </div>


  </div>
</section>


<!-- ========== Gallery / Featured Products Section ========== -->
<style>
  :root {
    /* —— reuse the same palette —— */
    --clr-bg:        #0f1117;
    --clr-surface:   #1a1d24;
    --clr-primary:   #facc15;
    --clr-text:      #f3f4f6;
    --clr-text-muted:#9ca3af;
  }

  .gallery {
    background: var(--clr-bg);
    padding: 4.75rem 1.25rem;
  }
  .gallery h2 {
    text-align: center;
    font-size: clamp(1.75rem, 3vw + .5rem, 2.5rem);
    font-weight: 800;
    margin-bottom: .75rem;
  }
  .gallery p.lead {
    text-align: center;
    color: var(--clr-text-muted);
    max-width: 38rem;
    margin: 0 auto 2.75rem;
    font-size: 1rem;
    line-height: 1.6;
  }

  /* ===== Masonry‑like Grid ===== */
  .gallery-grid {
    column-gap: 1.5rem;
    column-count: 1;             /* mobile */
  }
  @media (min-width: 600px)  { .gallery-grid { column-count: 2; } }
  @media (min-width: 900px)  { .gallery-grid { column-count: 3; } }

  .gallery-item {
    position: relative;
    margin-bottom: 1.5rem;
    border-radius: .85rem;
    overflow: hidden;
    box-shadow: 0 4px 12px rgba(0,0,0,.35);
    transition: transform .35s ease, box-shadow .35s ease;
    break-inside: avoid;         /* prevent column split */
  }
  .gallery-item:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 22px rgba(0,0,0,.5);
  }

  .gallery-item img {
    display: block;
    width: 100%;
    height: auto;
    object-fit: cover;
    transition: transform .35s ease;
  }
  .gallery-item:hover img { transform: scale(1.05); }

  /* Caption overlay */
  .caption {
    position: absolute;
    inset: 0;
    background: linear-gradient(to bottom, rgba(0,0,0,0) 40%, rgba(0,0,0,.75) 95%);
    color: var(--clr-text);
    display: flex;
    align-items: flex-end;
    padding: 1rem;
    opacity: 0;
    transition: opacity .35s ease;
  }
  .gallery-item:hover .caption { opacity: 1; }

  .caption h3 { font-size: 1rem; font-weight: 700; }
  .caption span.price {
    display: inline-block;
    margin-top: .25rem;
    font-size: .85rem;
    color: var(--clr-primary);
  }
</style>

<section class="gallery" id="products">
  <h2>Featured Products</h2>
  <p class="lead">A hand‑picked selection of our best‑selling stationery and print essentials.</p>

  <div class="gallery-grid">

    <!-- Item 1 -->
    <figure class="gallery-item">
      <img src="https://gcth-supplies.co.uk/wp-content/uploads/2022/02/A5-NOte.png"
           alt="Premium Spiral Notebook">
      <figcaption class="caption">
        <div>
          <h3>Spiral Notebook A5</h3>
          <span class="price">₹89</span>
        </div>
      </figcaption>
    </figure>

    <!-- Item 2 -->
    <figure class="gallery-item">
      <img src="https://reprographics.com/wp-content/uploads/2019/02/Various_color_prints.jpg"
           alt="Colour Print Sample">
      <figcaption class="caption">
        <div>
          <h3>Full‑Colour Prints (A4)</h3>
          <span class="price">From ₹10/page</span>
        </div>
      </figcaption>
    </figure>

    <!-- Item 3 -->
    <figure class="gallery-item">
      <img src="OCTANE Gel Pen.jpg"
           alt="OCTANE Gel Pens">
      <figcaption class="caption">
        <div>
          <h3>OCTANE Gel Pen Gel Pen Set</h3>
          <span class="price">₹99</span>
        </div>
      </figcaption>
    </figure>

    <!-- Item 4 -->
    <figure class="gallery-item">
      <img src="Flair ball pen.jpg"
           alt="Business Card Printing">
      <figcaption class="caption">
        <div>
          <h3>Flair ball pen</h3>
          <span class="price">₹80 </span>
        </div>
      </figcaption>
    </figure>

    <!-- Item 5 -->
    <figure class="gallery-item">
      <img src="ROLEX Mathematical Box.jpg"
           alt="Art Supplies Pack">
      <figcaption class="caption">
        <div>
          <h3>ROLEX Mathematical Box</h3>
          <span class="price">₹85</span>
        </div>
      </figcaption>
    </figure>

    <!-- Item 6 -->
    <figure class="gallery-item">
      <img src="Kangaro_No.10.jpg"
           alt="Laminated Document Sample">
      <figcaption class="caption">
        <div>
          <h3>Kangaro_No.10</h3>
          <span class="price">₹450 </span>
        </div>
      </figcaption>
    </figure>

  </div>
</section>


<!-- ========== Why Choose Us Section ========== -->
<style>
  :root {
    /* —— reuse the global palette —— */
    --clr-bg:        #0f1117;
    --clr-surface:   #1a1d24;
    --clr-primary:   #facc15;
    --clr-text:      #f3f4f6;
    --clr-text-muted:#9ca3af;
  }

  .why {
    background: var(--clr-surface);
    padding: 4.5rem 1.25rem;
  }

  .why-inner {
    max-width: 1150px;
    margin: 0 auto;
    display: grid;
    gap: 2.5rem;
    align-items: center;
  }
  /* 2‑col on large screens */
  @media (min-width: 900px) {
    .why-inner { grid-template-columns: 1fr 1fr; }
  }

  /* Headline */
  .why h2 {
    font-size: clamp(1.75rem, 3vw + .5rem, 2.5rem);
    font-weight: 800;
    margin-bottom: 1rem;
  }
  .why p.lead {
    color: var(--clr-text-muted);
    max-width: 32rem;
    font-size: 1rem;
    line-height: 1.6;
    margin-bottom: 2.25rem;
  }

  /* Feature list */
  .features {
    display: grid;
    gap: 1.5rem;
  }
  .feature {
    display: flex;
    gap: 1.1rem;
    align-items: flex-start;
  }
  .feature svg {
    flex-shrink: 0;
    width: 36px;
    height: 36px;
    fill: var(--clr-primary);
  }
  .feature h3 {
    font-size: 1.05rem;
    font-weight: 700;
    margin-bottom: .25rem;
  }
  .feature p {
    font-size: .95rem;
    color: var(--clr-text-muted);
    line-height: 1.5;
  }

  /* Image block */
  .why-img {
    position: relative;
    overflow: hidden;
    border-radius: 1rem;
    box-shadow: 0 6px 18px rgba(0,0,0,.5);
  }
  .why-img img {
    display: block;
    width: 100%;
    height: auto;
    object-fit: cover;
    transition: transform .4s ease;
  }
  .why-img:hover img { transform: scale(1.05); }
</style>

<section class="why" id="why-us">
  <div class="why-inner">

    <!-- Text + features -->
    <div class="why-content">
      <h2>Why Choose Us</h2>
      <p class="lead">We combine cutting‑edge equipment, expert craftsmanship, and friendly service to deliver unbeatable printing &amp; stationery solutions.</p>

      <div class="features">
        <!-- Feature 1 -->
        <div class="feature">
          <svg viewBox="0 0 24 24"><path d="M12 2l4 4h-3v9h-2V6H8l4-4zm-8 14h16v2H4v-2zm0 4h16v2H4v-2z"/></svg>
          <div>
            <h3>Fast Turnaround</h3>
            <p>Most jobs completed while you wait — no more long delays.</p>
          </div>
        </div>

        <!-- Feature 2 -->
        <div class="feature">
          <svg viewBox="0 0 24 24"><path d="M12 2a9.712 9.712 0 00-9.333 7H12V2zm0 20a9.712 9.712 0 009.333-7H12v7zM2 12a9.976 9.976 0 001.287 4.9l4.9-4.9H2zm19.713 0a9.976 9.976 0 00-1.287-4.9l-4.9 4.9h6.187zM4.287 7.1A9.976 9.976 0 002 12h6.187l-3.9-3.9zm15.426 9.8A9.976 9.976 0 0022 12h-6.187l3.9 3.9z"/></svg>
          <div>
            <h3>Affordable Pricing</h3>
            <p>Transparent rates and combo deals keep your costs low.</p>
          </div>
        </div>

        <!-- Feature 3 -->
        <div class="feature">
          <svg viewBox="0 0 24 24"><path d="M20 6h-2V4a2 2 0 00-2-2H8a2 2 0 00-2 2v2H4a2 2 0 00-2 2v10h6v2h8v-2h6V8a2 2 0 00-2-2zM8 4h8v2H8V4zm12 12h-4v-4H8v4H4V8h16v8z"/></svg>
          <div>
            <h3>Premium Quality</h3>
            <p>Top‑grade papers, inks, and materials for a flawless finish every time.</p>
          </div>
        </div>

        <!-- Feature 4 -->
        <div class="feature">
          <svg viewBox="0 0 24 24"><path d="M12 12a5 5 0 10-5-5 5 5 0 005 5zm-7 9a7 7 0 0114 0z"/></svg>
          <div>
            <h3>Friendly Experts</h3>
            <p>Our team is eager to advise and help you pick the perfect solution.</p>
          </div>
        </div>
      </div>
    </div>

    <!-- Image -->
    <div class="why-img">
      <img src="shop.jpg"
           alt="CM Prints & Stationery team at work">
    </div>

  </div>
</section>


<!-- ========== Featured Products / Offers Section ========== -->
<style>
  :root {
    /* —— reuse the global palette —— */
    --clr-bg:         #0f1117;
    --clr-surface:    #1a1d24;
    --clr-primary:    #facc15;
    --clr-text:       #f3f4f6;
    --clr-text-muted: #9ca3af;
  }

  .offers {
    background: var(--clr-bg);
    padding: 4.75rem 1.25rem;
  }
  .offers h2 {
    text-align: center;
    font-size: clamp(1.75rem, 3vw + .5rem, 2.5rem);
    font-weight: 800;
    margin-bottom: .75rem;
  }
  .offers p.lead {
    text-align: center;
    color: var(--clr-text-muted);
    max-width: 38rem;
    margin: 0 auto 2.5rem;
    font-size: 1rem;
    line-height: 1.6;
  }

  /* ===== Card Grid ===== */
  .offer-grid {
    display: grid;
    gap: 1.75rem;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    max-width: 1100px;
    margin-inline: auto;
  }

  .offer-card {
    background: var(--clr-surface);
    border-radius: .85rem;
    overflow: hidden;
    position: relative;
    display: flex;
    flex-direction: column;
    box-shadow: 0 4px 12px rgba(0,0,0,.35);
    transition: transform .35s ease, box-shadow .35s ease;
  }
  .offer-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 22px rgba(0,0,0,.5);
  }

  .offer-card img {
    width: 100%;
    height: 160px;
    object-fit: cover;
  }

  .offer-content {
    padding: 1.25rem 1rem 1.5rem;
    flex: 1 1 auto;
    display: flex;
    flex-direction: column;
  }
  .offer-content h3 {
    font-size: 1.05rem;
    font-weight: 700;
    margin-bottom: .5rem;
  }

  /* Prices */
  .price-wrap { margin-bottom: 1rem; }
  .price      { font-size: 1rem; font-weight: 700; }
  .price.old  { color: var(--clr-text-muted); text-decoration: line-through; font-weight: 400; margin-right: .5rem; }
  .price.new  { color: var(--clr-primary); }

  /* CTA button */
  .btn-buy {
    align-self: flex-start;
    padding: .6rem 1.4rem;
    border-radius: .5rem;
    background: var(--clr-primary);
    color: #000;
    font-weight: 600;
    font-size: .9rem;
    transition: background .25s;
  }
  .btn-buy:hover { background: #fde047; }

  /* Badge */
  .badge {
    position: absolute;
    top: .75rem;
    left: .75rem;
    padding: .25rem .6rem;
    background: var(--clr-primary);
    color: #000;
    font-size: .75rem;
    font-weight: 700;
    border-radius: 999px;
  }
</style>

<section class="offers" id="offers">
  <h2>Featured Products&nbsp;&amp;&nbsp;Offers</h2>
  <p class="lead">Snap up these limited‑time deals before they're gone!</p>

  <div class="offer-grid">

    <!-- Offer 1 -->
    <div class="offer-card">
      <span class="badge">SAVE&nbsp;30%</span>
      <img src="https://m.media-amazon.com/images/I/51K6h4oxFbL._SL1001_.jpg"
           alt="Premium Notebook Pack">
      <div class="offer-content">
        <h3>Premium Notebook Pack (3×)</h3>
        <div class="price-wrap">
          <span class="price old">₹299</span>
          <span class="price new">₹209</span>
        </div>
        <a href="tel:+91 9330713861" class="btn-buy">Buy&nbsp;Now</a>
      </div>
    </div>

    <!-- Offer 2 -->
    <div class="offer-card">
      <span class="badge">NEW</span>
      <img src="https://cdn11.bigcommerce.com/s-7edce/images/stencil/1280w/products/935/230605/Design-somerz-Rainbow-Gel-Pen-038mm-set-of-10-colors_7572__84514.1684490456.jpg?c=2"
           alt="Rainbow Gel Pen Set">
      <div class="offer-content">
        <h3>Rainbow Gel Pen Set (12‑pcs)</h3>
        <div class="price-wrap">
          <span class="price old">₹189</span>
          <span class="price new">₹149</span>
        </div>
        <a href="tel:+91 9330713861" class="btn-buy">Buy&nbsp;Now</a>
      </div>
    </div>

    <!-- Offer 3 -->
    <div class="offer-card">
      <span class="badge">HOT&nbsp;DEAL</span>
      <img src="https://media.karousell.com/media/photos/products/2017/05/21/sony_color_print_pack_dppf_120pc_1495342527_bd9f5a5e.jpg"
           alt="Colour Print Pack">
      <div class="offer-content">
        <h3>Colour Print Pack (50 pages)</h3>
        <div class="price-wrap">
          <span class="price old">₹750</span>
          <span class="price new">₹525</span>
        </div>
        <a href="tel:+91 9330713861" class="btn-buy">Buy&nbsp;Now</a>
      </div>
    </div>

    <!-- Offer 4 -->
    <div class="offer-card">
      <span class="badge">SAVE&nbsp;25%</span>
      <img src="https://i.redd.it/nhveuv9rbej11.jpg"
           alt="Office Starter Bundle">
      <div class="offer-content">
        <h3>Office Starter Bundle</h3>
        <div class="price-wrap">
          <span class="price old">₹999</span>
          <span class="price new">₹749</span>
        </div>
        <a href="tel:+91 9330713861" class="btn-buy">Buy&nbsp;Now</a>
      </div>
    </div>

  </div>
</section>


<!-- ========== Customer Testimonials Section ========== -->
<style>
  :root {
    /* —— global palette —— */
    --clr-bg:         #0f1117;
    --clr-surface:    #1a1d24;
    --clr-primary:    #facc15;
    --clr-text:       #f3f4f6;
    --clr-text-muted: #9ca3af;
  }

  .testimonials {
    background: var(--clr-bg);
    padding: 4.5rem 1.25rem;
  }
  .testimonials h2 {
    text-align: center;
    font-size: clamp(1.75rem, 3vw + .5rem, 2.5rem);
    font-weight: 800;
    margin-bottom: .75rem;
  }
  .testimonials p.lead {
    text-align: center;
    color: var(--clr-text-muted);
    max-width: 38rem;
    margin: 0 auto 2.5rem;
    font-size: 1rem;
    line-height: 1.6;
  }

  /* ===== Card Grid ===== */
  .reviews-grid {
    display: grid;
    gap: 1.75rem;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    max-width: 1100px;
    margin: 0 auto;
  }

  .review-card {
    background: var(--clr-surface);
    border-radius: .9rem;
    padding: 2rem 1.5rem 2.25rem;
    display: flex;
    flex-direction: column;
    box-shadow: 0 4px 12px rgba(0,0,0,.35);
    transition: transform .35s ease, box-shadow .35s ease;
  }
  .review-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 22px rgba(0,0,0,.5);
  }

  /* Avatar */
  .avatar {
    width: 58px;
    height: 58px;
    border-radius: 50%;
    object-fit: cover;
    border: 3px solid var(--clr-primary);
    margin-bottom: 1rem;
  }

  /* Reviewer name */
  .review-card h3 {
    font-size: 1.05rem;
    font-weight: 700;
    margin-bottom: .35rem;
  }

  /* Star rating */
  .stars {
    display: flex;
    gap: .15rem;
    margin-bottom: 1rem;
  }
  .stars svg {
    width: 18px; height: 18px;
    fill: var(--clr-primary);
  }

  /* Review text */
  .review-card p {
    font-size: .95rem;
    color: var(--clr-text-muted);
    line-height: 1.55;
    flex: 1 1 auto;
    position: relative;
  }
  /* decorative opening quote */
  .review-card p::before {
    content: "“";
    font-size: 2.5rem;
    line-height: 0;
    color: var(--clr-primary);
    position: absolute;
    top: -.2rem;
    left: -.3rem;
  }
</style>

<section class="testimonials" id="testimonials">
  <h2>What Our Customers Say</h2>
  <p class="lead">Real feedback from happy students, professionals, and artists who trust CM Prints &amp; Stationery.</p>

  <div class="reviews-grid">
    <!-- Review 1 -->
    <div class="review-card">
      <img class="avatar" src="Samrat.jpg"
           alt="Customer profile">
      <h3>Samrat Mondal</h3>
      <div class="stars">
        <!-- 5 stars -->
        <svg viewBox="0 0 24 24"><path d="M12 17.3l6.2 3.7-1.6-6.9 5.4-4.7-7-.6L12 2 9 8.8l-7 .6 5.4 4.7-1.6 6.9z"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
      </div>
      <p>Lightning‑fast Xerox service! Needed 200 copies for my project and got them in under 15 minutes. Great quality and price.</p>
    </div>

    <!-- Review 2 -->
    <div class="review-card">
      <img class="avatar" src="Rahul.png"
           alt="Customer profile">
      <h3>Rahul Bijali</h3>
      <div class="stars">
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
      </div>
      <p>Their custom invitation cards blew us away—premium paper, vivid colours, and delivered earlier than promised. Highly recommended!</p>
    </div>

    <!-- Review 3 -->
    <div class="review-card">
      <img class="avatar" src="Sayan.png"
           alt="Customer profile">
      <h3>Sayan Ghosh</h3>
      <div class="stars">
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
        <svg viewBox="0 0 24 24"><use href="#star"/></svg>
      </div>
      <p>Love the stationery range here—picked up notebooks, gel pens, and an art kit. The staff even helped me choose the right sketch pencils.</p>
    </div>
  </div>

  <!-- ===== reusable SVG symbol (1 star) ===== -->
  <svg width="0" height="0" style="position:absolute;visibility:hidden;">
    <symbol id="star" viewBox="0 0 24 24">
      <path d="M12 17.3l6.2 3.7-1.6-6.9 5.4-4.7-7-.6L12 2 9 8.8l-7 .6 5.4 4.7-1.6 6.9z"/>
    </symbol>
  </svg>
</section>


<!-- ========== Location & Contact Section ========== -->
<style>
  :root {
    /* —— global palette —— */
    --clr-bg:         #0f1117;
    --clr-surface:    #1a1d24;
    --clr-primary:    #facc15;
    --clr-text:       #f3f4f6;
    --clr-text-muted: #9ca3af;
  }

  .contact {
    background: var(--clr-surface);
    padding: 4.75rem 1.25rem;
  }

  .contact-inner {
    max-width: 1200px;
    margin: 0 auto;
    display: grid;
    gap: 2.5rem;
  }
  /* two‑column layout on desktops */
  @media (min-width: 950px) {
    .contact-inner { grid-template-columns: 1fr 1fr; }
  }

  .contact h2 {
    font-size: clamp(1.75rem, 3vw + .5rem, 2.5rem);
    font-weight: 800;
    margin-bottom: .75rem;
    text-align: center;
  }
  .contact p.lead {
    text-align: center;
    color: var(--clr-text-muted);
    margin: 0 auto 2rem;
    max-width: 38rem;
    line-height: 1.6;
  }

  /* ===== Map ===== */
  .map-wrapper {
    position: relative;
    overflow: hidden;
    border-radius: 1rem;
    box-shadow: 0 6px 18px rgba(0,0,0,.45);
  }
  .map-wrapper iframe {
    width: 100%;
    height: 100%;
    min-height: 350px;
    border: 0;
  }

  /* ===== Contact Details & Form ===== */
  .contact-box {
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }

  /* Details list */
  .details {
    display: grid;
    gap: 1.25rem;
  }
  .details-item {
    display: flex;
    gap: 1rem;
    align-items: flex-start;
  }
  .details-item svg {
    flex-shrink: 0;
    width: 28px; height: 28px;
    fill: var(--clr-primary);
    margin-top: .15rem;
  }
  .details-item span {
    color: var(--clr-text-muted);
    font-size: .95rem;
    line-height: 1.55;
  }

  /* Form */
  .contact-form {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }
  .contact-form input,
  .contact-form textarea {
    width: 100%;
    padding: .75rem 1rem;
    background: #11131a;
    border: 1px solid #2a2d34;
    border-radius: .55rem;
    font-size: .95rem;
    color: var(--clr-text);
  }
  .contact-form input::placeholder,
  .contact-form textarea::placeholder { color: var(--clr-text-muted); }
  .contact-form textarea { min-height: 140px; resize: vertical; }

  .btn-send {
    width: fit-content;
    padding: .7rem 1.6rem;
    border: 0;
    border-radius: .55rem;
    background: var(--clr-primary);
    color: #000;
    font-weight: 600;
    font-size: .9rem;
    cursor: pointer;
    transition: background .25s;
  }
  .btn-send:hover { background: #fde047; }
</style>

<section class="contact" id="contact">
  <h2>Find Us &amp; Get in Touch</h2>
  <p class="lead">Drop by our shop, call us, or send a quick message—we’re always ready to help.</p>

  <div class="contact-inner">

    <!-- Embedded Google Map -->
    <div class="map-wrapper">
      <!-- Replace the src URL with your shop’s exact Google Maps embed link -->
      <iframe
        loading="lazy"
        allowfullscreen
        src="JFP2+QW Kolkata, West Bengal"
      ></iframe>
    </div>

    <!-- Details + Quick Contact Form -->
    <div class="contact-box">

      <!-- Contact Details -->
      <div class="details">
        <div class="details-item">
          <svg viewBox="0 0 24 24"><path d="M12 2C8 2 2 4 2 8c0 6 10 14 10 14s10-8 10-14c0-4-6-6-10-6zm0 9.5a1.5 1.5 0 110-3 1.5 1.5 0 010 3z"/></svg>
          <span>grount floor, kali mandir, Saptarshi apartment, Kalipark, Bablatala, Gopalpur I, Kolkata, West Bengal 700052</span>
        </div>
        <div class="details-item">
          <svg viewBox="0 0 24 24"><path d="M4 4h16v2H4V4zm0 4h16v2H4V8zm0 4h16v2H4v-2zm0 4h16v2H4v-2z"/></svg>
          <span>Mon‑Sat 8 AM – 10 PM</span>
        </div>
        <div class="details-item">
          <svg viewBox="0 0 24 24"><path d="M6.6 10.8C8.2 13.8 10.2 15.8 13.2 17.4l2.2-2.2c.3-.3.8-.4 1.2-.2 1.3.4 2.7.7 4.1.7.6 0 1 .4 1 .9V21c0 .5-.4 1-.9 1C10.7 22 2 13.3 2 2.9 2 2.4 2.5 2 3 2h4.5c.5 0 .9.4.9 1 0 1.4.2 2.8.7 4.1.1.4 0 .9-.3 1.2l-2.2 2.5z"/></svg>
          <span><a href="tel:+91 9330713861" style="color:inherit;">+91 9330713861</a></span>
        </div>
        <div class="details-item">
          <svg viewBox="0 0 24 24"><path d="M2 4l10 7 10-7v14H2V4zm10 9L2 6v12h20V6l-10 7z"/></svg>
          <span><a href="mailto:chattu1904@gmail.com" style="color:inherit;">chattu1904@gmail.com</a></span>
        </div>
      </div>

      <!-- Quick Contact Form (non‑functional demo) -->
      <form class="contact-form" onsubmit="event.preventDefault(); alert('Thank you! We will get back to you soon.');">
        <input type="text"     name="name"    placeholder="Your Name"    required>
        <input type="email"    name="email"   placeholder="Your Email"   required>
        <textarea              name="message" placeholder="Your Message" required></textarea>
        <button class="btn-send" type="submit">Send&nbsp;Message</button>
      </form>

    </div>
  </div>
</section>


<!-- ========== Mobile App / WhatsApp CTA Section ========== -->
<style>
  :root {
    /* —— global palette —— */
    --clr-bg:         #0f1117;
    --clr-surface:    #1a1d24;
    --clr-primary:    #facc15;
    --clr-text:       #f3f4f6;
    --clr-text-muted: #9ca3af;
  }

  .app-cta {
    background: var(--clr-bg);
    padding: 4.5rem 1.25rem;
    overflow: hidden;
  }

  .app-wrap {
    max-width: 1150px;
    margin: 0 auto;
    display: grid;
    gap: 2.5rem;
    align-items: center;
  }
  /* two‑column on desktops */
  @media (min-width: 900px) {
    .app-wrap { grid-template-columns: 1fr 1fr; }
  }

  /* Text block */
  .app-text h2 {
    font-size: clamp(1.75rem, 3vw + .5rem, 2.5rem);
    font-weight: 800;
    margin-bottom: 1rem;
  }
  .app-text p {
    color: var(--clr-text-muted);
    font-size: 1rem;
    line-height: 1.6;
    margin-bottom: 2rem;
    max-width: 32rem;
  }

  /* Button row */
  .btn-row {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
  }
  .cta-btn {
    display: inline-flex;
    align-items: center;
    gap: .55rem;
    padding: .75rem 1.4rem;
    border-radius: .65rem;
    font-size: .9rem;
    font-weight: 700;
    background: var(--clr-primary);
    color: #000;
    transition: background .25s;
    text-decoration: none;
  }
  .cta-btn:hover { background: #fde047; }

  /* Alt style for dark button (WhatsApp) */
  .wa-btn {
    background: #25D366;
    color: #000;
  }
  .wa-btn:hover { background: #29e770; }

  .cta-btn svg {
    width: 20px; height: 20px;
    fill: currentColor;
  }

  /* Phone mockup */
  .phone-frame {
    position: relative;
    overflow: hidden;
    border-radius: 1.25rem;
    box-shadow: 0 6px 20px rgba(0,0,0,.5);
  }
  .phone-frame img {
    width: 100%;
    height: auto;
    display: block;
  }
</style>

<section class="app-cta" id="download">
  <div class="app-wrap">

    <!-- Left: copy + buttons -->
    <div class="app-text">
      <h2>Prints &amp; Stationery — On Your Phone</h2>
      <p>Order prints, track jobs, and chat with us instantly. Get the CM Prints &amp; Stationery mobile app or message us on WhatsApp now.</p>

      <div class="btn-row">
        <!-- Google Play (placeholder icon) -->
        <a class="cta-btn" href="#playstore">
          <svg viewBox="0 0 24 24"><path d="M3 2l15 10L3 22V2zm2 3.5v13l9.5-6.5L5 5.5z"/></svg>
          Google Play
        </a>

        <!-- App Store (placeholder icon) -->
        <a class="cta-btn" href="#appstore">
          <svg viewBox="0 0 24 24"><path d="M18 16.08c0-3.84 3.13-5.36 3.29-5.45-1.8-2.6-4.6-2.96-5.6-3-2.4-.24-4.7 1.4-5.9 1.4-1.2 0-3-.9-4.9-.88-2.52.03-4.8 1.46-6.1 3.7-2.6 4.58-.66 11.34 1.8 15.06 1.2 1.78 2.6 3.76 4.46 3.68 1.8-.07 2.48-1.18 4.64-1.18 2.16 0 2.76 1.18 4.8 1.14 2-.04 3.26-1.78 4.44-3.57 1.4-2 1.98-3.92 2-4.02-1.94-.94-3.66-2.46-3.66-4.96z"/></svg>
          App Store
        </a>

        <!-- WhatsApp -->
        <a class="cta-btn wa-btn" href="https://wa.me/+91 9330713861" target="_blank">
          <svg viewBox="0 0 24 24"><path d="M12.04 2C6.51 2 2 6.52 2 12.07c0 1.97.51 3.84 1.46 5.49L2 22l4.62-1.41c1.6.88 3.41 1.34 5.42 1.34h.01C17.57 22 22 17.58 22 12.07 22 6.52 17.57 2 12.04 2zm5.37 15.24c-.23.64-1.35 1.22-1.85 1.29-.47.07-1.05.1-1.69-.11-.39-.12-.9-.29-1.55-.57-2.73-1.18-4.51-3.99-4.66-4.18-.13-.18-1.11-1.48-1.11-2.83 0-1.35.71-2.02.96-2.27.23-.23.51-.29.68-.29.17 0 .34.01.49.01.15 0 .35-.05.55.42.21.5.72 1.75.79 1.88.07.13.11.29.03.47-.08.18-.12.29-.24.46-.12.17-.25.39-.36.52-.12.13-.24.27-.1.52.14.25.61 1 .91 1.37 1.26 1.6 2.34 2.1 2.69 2.34.35.23.56.19.75-.11.19-.29.86-1.01 1.1-1.36.24-.34.48-.29.81-.17.33.11 2.1.99 2.46 1.17.36.17.6.25.69.39.08.14.08.72-.15 1.36z"/></svg>
          WhatsApp
        </a>
      </div>
    </div>

    <!-- Right: phone mockup -->
    <div class="phone-frame">
      <img src="https://images.unsplash.com/photo-1539883371145-41f40e2c6bb2?auto=format&fit=crop&w=700&q=80"
           alt="CM Prints App Mock‑up">
    </div>

  </div>
</section>


<!-- ========== Newsletter / Coupon Signup Section ========== -->
<style>
  :root {
    /* —— global dark palette —— */
    --clr-bg:         #0f1117;
    --clr-surface:    #1a1d24;
    --clr-surface-alt:#181b22;
    --clr-primary:    #facc15;
    --clr-text:       #f3f4f6;
    --clr-text-muted: #9ca3af;
  }

  .signup {
    background: var(--clr-bg);
    padding: 4.75rem 1.25rem;
  }
  .signup-wrap {
    max-width: 900px;
    margin: 0 auto;
    background: var(--clr-surface);
    border-radius: 1.1rem;
    box-shadow: 0 6px 22px rgba(0,0,0,.5);
    padding: 3rem 2rem;
    text-align: center;
  }

  .signup h2 {
    font-size: clamp(1.75rem, 3vw + .5rem, 2.4rem);
    font-weight: 800;
    margin-bottom: .75rem;
  }
  .signup p.lead {
    color: var(--clr-text-muted);
    font-size: 1rem;
    line-height: 1.6;
    margin-bottom: 2rem;
    max-width: 34rem;
    margin-inline: auto;
  }

  /* === Form === */
  .signup-form {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    justify-content: center;
  }
  .signup-form input[type="email"] {
    flex: 1 1 260px;
    min-width: 0;
    padding: .85rem 1.1rem;
    background: var(--clr-surface-alt);
    border: 1px solid #2a2d34;
    border-radius: .65rem;
    font-size: .95rem;
    color: var(--clr-text);
  }
  .signup-form input::placeholder { color: var(--clr-text-muted); }

  .btn-subscribe {
    flex: 0 0 auto;
    padding: .9rem 1.7rem;
    border: 0;
    border-radius: .65rem;
    background: var(--clr-primary);
    color: #000;
    font-weight: 700;
    font-size: .9rem;
    cursor: pointer;
    transition: background .25s;
  }
  .btn-subscribe:hover { background: #fde047; }

  /* Coupon badge */
  .coupon {
    display: inline-block;
    margin-top: 2rem;
    padding: .55rem 1.2rem;
    background: var(--clr-surface-alt);
    border: 1px dashed var(--clr-primary);
    border-radius: .6rem;
    font-size: .9rem;
    letter-spacing: .03em;
    color: var(--clr-primary);
    font-weight: 600;
  }
</style>

<section class="signup" id="newsletter">
  <div class="signup-wrap">
    <h2>Get ₹20 Off Your First Order</h2>
    <p class="lead">Join our newsletter for exclusive deals, print tips, and early‑access coupons—straight to your inbox.</p>

    <form class="signup-form" onsubmit="event.preventDefault(); alert('Thanks! Check your inbox for the coupon.');">
      <input type="email" name="email" placeholder="Enter your email address" required />
      <button class="btn-subscribe" type="submit">Subscribe</button>
    </form>

    <span class="coupon">Use code <strong>WELCOME20</strong> at checkout.</span>
  </div>
</section>


<!-- =============== Footer (Dark Theme) =============== -->
<style>
  :root {
    /* — global palette (reuse) — */
    --clr-bg:          #0f1117;
    --clr-surface:     #1a1d24;
    --clr-surface-alt: #181b22;
    --clr-primary:     #facc15;
    --clr-text:        #f3f4f6;
    --clr-text-muted:  #9ca3af;
  }

  footer {
    background: var(--clr-surface);
    color: var(--clr-text);
    padding: 3.5rem 1.25rem 2rem;
    font-size: .95rem;
  }

  /* ===== Top grid ===== */
  .footer-grid {
    max-width: 1150px;
    margin: 0 auto 2.75rem;
    display: grid;
    gap: 2rem 2.5rem;
  }
  /* 4 columns on desktop, 2 on tablets, 1 on mobile */
  @media (min-width: 900px) { .footer-grid { grid-template-columns: repeat(4, 1fr); } }
  @media (min-width: 600px) and (max-width: 899px) { .footer-grid { grid-template-columns: repeat(2, 1fr); } }

  .footer-title {
    font-weight: 700;
    margin-bottom: 1rem;
    font-size: 1.05rem;
  }
  .footer-link {
    display: block;
    margin-bottom: .55rem;
    color: var(--clr-text-muted);
    transition: color .2s;
    text-decoration: none;
  }
  .footer-link:hover { color: var(--clr-primary); }

  /* Address block */
  .address span {
    display: block;
    margin-bottom: .55rem;
    color: var(--clr-text-muted);
    line-height: 1.45;
  }

  /* Social icons */
  .social-row {
    display: flex;
    gap: .8rem;
    margin-top: .8rem;
  }
  .social-row a {
    display: inline-flex;
    width: 34px;
    height: 34px;
    align-items: center;
    justify-content: center;
    border-radius: 50%;
    background: var(--clr-surface-alt);
    transition: background .25s;
  }
  .social-row a:hover { background: var(--clr-primary); }
  .social-row svg {
    width: 18px; height: 18px;
    fill: var(--clr-text);
    transition: fill .25s;
  }
  .social-row a:hover svg { fill: #000; }

  /* Divider */
  .footer-divider {
    height: 1px;
    background: #21242b;
    margin: 0 auto 1.75rem;
    max-width: 1150px;
  }

  /* Bottom bar */
  .footer-bottom {
    max-width: 1150px;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    gap: 1rem;
    font-size: .8rem;
    color: var(--clr-text-muted);
  }
  .payment-row img {
    height: 26px;
    margin-left: .6rem;
    filter: brightness(0) invert(1); /* white logos */
    opacity: .75;
    transition: opacity .25s;
  }
  .payment-row img:hover { opacity: 1; }
</style>

<footer id="footer">
  <div class="footer-grid">

    <!-- About -->
    <div>
      <h3 class="footer-title">CM Prints & Stationery</h3>
      <p style="color:var(--clr-text-muted); line-height:1.55; max-width:24rem;">
        Your trusted one‑stop hub for high‑quality printing, stationery supplies, and custom design solutions—serving Kolkata since 2010.
      </p>

      <!-- Social icons -->
      <div class="social-row">
        <a href="#" aria-label="Facebook">
          <svg viewBox="0 0 24 24"><path d="https://www.facebook.com/share/1CiynJr9P5/"/><img src="https://pro-assets.morningconsult.com/wp-uploads/2023/10/231009_Facebook-Brand-Spotlight_Feature-Image.jpg" alt=""></svg>
        </a>
        <a href="#" aria-label="Instagram">
          <svg viewBox="0 0 24 24"><path d="https://www.instagram.com/"/><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Instagram_logo_2022.svg/640px-Instagram_logo_2022.svg.png" alt=""></svg>
        </a>
        <a href="#" aria-label="WhatsApp">
          <svg viewBox="0 0 24 24"><path d="M12.04 2C6.5 2 2 6.53 2 12.08c0 1.97.52 3.85 1.47 5.5L2 22l4.64-1.42c1.62.89 3.46 1.35 5.4 1.35 5.55 0 10.06-4.52 10.06-10.06C22.1 6.53 17.59 2 12.04 2zm5.35 15.3c-.24.67-1.38 1.28-1.91 1.35-.48.07-1.07.11-1.73-.12-.4-.13-.92-.3-1.6-.59-2.77-1.2-4.58-4.05-4.73-4.24-.14-.2-1.13-1.51-1.13-2.9 0-1.39.72-2.08.98-2.33.23-.23.52-.3.7-.3.18 0 .35.01.51.01.15 0 .37-.05.58.43.21.5.75 1.79.82 1.93.07.14.12.3.03.49-.08.19-.13.31-.25.49-.12.18-.26.4-.37.54-.12.14-.25.28-.1.55.14.26.63 1.05.95 1.44 1.31 1.67 2.43 2.18 2.79 2.42.36.24.58.2.78-.12.2-.3.89-1.04 1.14-1.4.25-.35.5-.3.83-.18.34.11 2.15 1.03 2.52 1.21.37.18.62.26.71.41.09.15.09.75-.16 1.42z"/></svg>
        </a>
      </div>
    </div>

    <!-- Quick Links -->
    <div>
      <h3 class="footer-title">Quick Links</h3>
      <a class="footer-link" href="#services">Services</a>
      <a class="footer-link" href="#products">Products</a>
      <a class="footer-link" href="#why-us">Why Choose Us</a>
      <a class="footer-link" href="#offers">Offers</a>
      <a class="footer-link" href="#contact">Contact</a>
    </div>

    <!-- Customer Support -->
    <div>
      <h3 class="footer-title">Customer Support</h3>
      <a class="footer-link" href="tel:+91 9330713861">+91 93307 13861</a>
      <a class="footer-link" href="mailto:chattu1904@gmail.com">chattu1904@gmail.com</a>
      <a class="footer-link" href="#">FAQs</a>
      <a class="footer-link" href="#">Shipping & Returns</a>
      <a class="footer-link" href="#">Privacy Policy</a>
    </div>

    <!-- Visit Us -->
    <div class="address">
      <h3 class="footer-title">Visit Us</h3>
      <span>Bablatala Kalipark kali mandir</span>
      <span>Kolkata 700 136</span>
      <span>West Bengal, India</span>
      <span>Mon‑Sat 8 AM – 10 PM</span>
    </div>
  </div>

  <div class="footer-divider"></div>

  <!-- Bottom bar -->
  <div class="footer-bottom">
    <span>© 2025 CM Prints & Stationery — All rights reserved.</span>

    <!-- Payment icons (PNG/SVG placeholders) -->
    <div class="payment-row">
      <img src="https://upload.wikimedia.org/wikipedia/commons/0/04/Visa.svg" alt="Visa" />
      <img src="https://upload.wikimedia.org/wikipedia/commons/5/57/MasterCard_Logo.svg" alt="Mastercard" />
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/34/RuPay.svg/320px-RuPay.svg.png" alt="RuPay" />
      <img src="https://upload.wikimedia.org/wikipedia/commons/2/2a/Unified_Payments_Interface_logo.svg" alt="UPI" />
    </div>
  </div>
</footer>

</body>
</html>
