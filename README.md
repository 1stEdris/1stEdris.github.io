<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Cook Edris — Portfolio</title>

  <!-- Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Montserrat:wght@300;500;700&display=swap" rel="stylesheet">

  <style>
    *{box-sizing:border-box;margin:0;padding:0}
    html,body,#app{height:100%}
    body{font-family: 'Montserrat', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; color:#fff; background:#000}

    /* slideshow */
    .slideshow{position:relative;height:100vh;overflow:hidden}
    .slide{position:absolute;inset:0;background-size:cover;background-position:center;display:flex;align-items:center;justify-content:center;transition:opacity 1s ease;opacity:0}
    .slide.visible{opacity:1}

    .overlay{position:absolute;inset:0;background:linear-gradient(180deg, rgba(0,0,0,.25) 0%, rgba(0,0,0,.6) 100%);pointer-events:none}

    .headline{
      font-family: 'Great Vibes', cursive;
      font-size: clamp(36px, 8vw, 120px);
      transform: scaleX(1.18);
      letter-spacing: 1px;
      text-align:center;
      text-shadow: 0 6px 30px rgba(0,0,0,.6);
      pointer-events:auto;
      z-index:2;
    }

    /* intro card */
    .intro-card{
      position: absolute; bottom:6vh; left:50%; transform:translateX(-50%);
      background:rgba(0,0,0,0.35);backdrop-filter:blur(4px);
      padding:20px 28px;border-radius:14px;display:flex;gap:18px;align-items:center;
      box-shadow:0 10px 30px rgba(0,0,0,.6); z-index:3;
    }
    .intro-card img{width:84px;height:84px;object-fit:cover;border-radius:10px;border:3px solid rgba(255,255,255,.06)}
    .intro-text{display:flex;flex-direction:column}
    .intro-text strong{font-size:18px}
    .intro-text small{opacity:.8;font-size:13px}

    .thumbs{display:flex;gap:10px;margin-top:8px}
    .thumbs img{width:64px;height:44px;object-fit:cover;border-radius:6px;filter:grayscale(.02);border:2px solid rgba(255,255,255,.06)}

    /* section buttons style (consistent look) */
    .section {
      max-width:1000px;
      margin:40px auto;
      text-align:left;
    }
    .section h2{font-family:'Great Vibes',cursive;font-size:36px;margin-bottom:8px}
    .section p{color:rgba(255,255,255,0.92)}
    .btn {
      display:inline-block;
      margin-top:12px;padding:8px 20px;color:#fff;
      background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.3);
      border-radius:8px;text-decoration:none;font-weight:600;
    }

    .cv-text{font-size:13px;opacity:.9;margin-top:6px}

    @media (max-width:720px){
      .intro-card{left:50%;transform:translateX(-50%);padding:14px;flex-direction:column;align-items:center}
      .intro-card img{width:96px;height:96px}
      .headline{font-size:clamp(28px,9vw,64px)}
      .section{padding:0 18px}
    }
  </style>
</head>
<body>
  <div id="app">

    <!-- SLIDESHOW -->
    <section class="slideshow" id="slideshow" aria-label="Hero slideshow">

      <article class="slide visible" style="background-image: Roast-Beff-Sandwich.png" data-title="Spiced Lamb Platter">
        <div class="overlay"></div>
        <h1 class="headline">Spiced Lamb Platter</h1>
      </article>

      <article class="slide" style="background-image:url('https://images.unsplash.com/photo-1543353071-087092ec393a?auto=format&fit=crop&w=1600&q=80');" data-title="Seafood Medley">
        <div class="overlay"></div>
        <h1 class="headline">Seafood Medley</h1>
      </article>

      <article class="slide" style="background-image:url('https://images.unsplash.com/photo-1541544741938-0af808871cc0?auto=format&fit=crop&w=1600&q=80');" data-title="Colorful Vegan Bowl">
        <div class="overlay"></div>
        <h1 class="headline">Colorful Vegan Bowl</h1>
      </article>

      <article class="slide" style="background-image:url('https://images.unsplash.com/photo-1473093295043-cdd812d0e601?auto=format&fit=crop&w=1600&q=80');" data-title="Crispy Street Burger">
        <div class="overlay"></div>
        <h1 class="headline">Crispy Street Burger</h1>
      </article>

      <!-- intro card -->
      <div class="intro-card" role="region" aria-label="Introduction">
        <img src="My-photo.png" alt="Cook Edris portrait">
        <div class="intro-text">
          <strong>Hello, I'm Cook Edris</strong>
          <small>Chef's assistant • cook</small>

          <div class="thumbs" aria-hidden="false">
            <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=400&q=60" alt="food thumb 1">
            <img src="https://images.unsplash.com/photo-1543353071-087092ec393a?auto=format&fit=crop&w=400&q=60" alt="food thumb 2">
            <img src="https://images.unsplash.com/photo-1541544741938-0af808871cc0?auto=format&fit=crop&w=400&q=60" alt="food thumb 3">
          </div>

          <div class="cv-text"><a href="cv.html" style="color:inherit;text-decoration:underline;">My CV</a></div>
        </div>
      </div>

    </section>

    <!-- MAIN SECTIONS -->
    <main style="padding:40px;background:#0b0b0b;color:#fff;">

      <section id="international" class="section">
        <h2>International Dishes</h2>
        <p>Gallery and recipes for refined international cuisine — explore dishes from around the world.</p>
        <a href="international.html" class="btn">See More →</a>
      </section>

      <section id="fastfood" class="section">
        <h2>Fast Food Samples</h2>
        <p>Samples from the fast-food and street-food repertoire — explore my fast food creations below.</p>
        <a href="fastfood.html" class="btn">See More →</a>
      </section>

      <!-- بخش جدید Salad که بعد از Fast Food اضافه شده -->
      <section id="salad" class="section">
        <h2>Salads</h2>
        <p>Experience the freshness of our carefully crafted salads, made with the finest seasonal ingredients and house-made dressings.</p>
        <a href="salad.html" class="btn">See More →</a>
      </section>

      <section id="breakfast" class="section">
        <h2>Breakfast</h2>
        <p>Discover delicious and energizing breakfast dishes from around the world.</p>
        <a href="breakfast.html" class="btn">See More →</a>
      </section>

      <section id="seafood" class="section">
        <h2>Seafood</h2>
        <p>Fresh seafood selections — from calamari to lobster and more.</p>
        <a href="seafood.html" class="btn">See More →</a>
      </section>

      <section id="dessert" class="section">
        <h2>Desserts</h2>
        <p>Sweet and delightful desserts — enjoy a curated selection of world favorites.</p>
        <a href="desserts.html" class="btn">See More →</a>
      </section>

      <section id="cv" class="section">
        <h2>My CV</h2>
        <p>View my professional chef résumé — experience, skills, and background.</p>
        <a href="cv.html" class="btn">See My Full CV →</a>
      </section>

    </main>

  </div>

  <!-- SLIDESHOW SCRIPT -->
  <script>
    (function(){
      const slides = Array.from(document.querySelectorAll('.slide'));
      let idx = 0;
      const show = i => slides.forEach((s,si)=> s.classList.toggle('visible', si===i));
      show(idx);
      let interval = setInterval(()=>{ idx = (idx+1) % slides.length; show(idx); }, 5000);

      const slideshow = document.getElementById('slideshow');
      let paused = false;
      slideshow.addEventListener('mouseenter', ()=>{ if(!paused){ clearInterval(interval); paused=true }});
      slideshow.addEventListener('mouseleave', ()=>{ if(paused){ interval = setInterval(()=>{ idx = (idx+1) % slides.length; show(idx); }, 5000); paused=false }});

    })();
  </script>

</body>
</html>
