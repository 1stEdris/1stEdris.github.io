
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Cook Edris — Portfolio</title>  <!-- Google Fonts: a calligraphic 'stretched' headline + clean body -->  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Montserrat:wght@300;500;700&display=swap" rel="stylesheet">  <style>
    *{box-sizing:border-box;margin:0;padding:0}
    html,body,#app{height:100%}
    body{font-family: 'Montserrat', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; color:#fff; background:#000}

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
    }

    .intro-card{
      position: absolute; bottom:6vh; left:50%; transform:translateX(-50%);
      background:rgba(0,0,0,0.35);backdrop-filter:blur(4px);
      padding:20px 28px;border-radius:14px;display:flex;gap:18px;align-items:center;
      box-shadow:0 10px 30px rgba(0,0,0,.6);
    }
    .intro-card img{width:84px;height:84px;object-fit:cover;border-radius:10px;border:3px solid rgba(255,255,255,.06)}
    .intro-text{display:flex;flex-direction:column}
    .intro-text strong{font-size:18px}
    .intro-text small{opacity:.8;font-size:13px}

    .thumbs{display:flex;gap:10px;margin-top:8px}
    .thumbs img{width:64px;height:44px;object-fit:cover;border-radius:6px;filter:grayscale(.02);border:2px solid rgba(255,255,255,.06)}

    .menu-btn{position:absolute;top:18px;left:18px;z-index:40;background:rgba(255,255,255,0.06);border-radius:8px;padding:8px 10px;cursor:pointer}
    .menu-btn .dots{font-weight:700;letter-spacing:6px}

    .side-menu{position:fixed;top:0;left:0;transform:translateX(-110%);height:100%;width:320px;max-width:82vw;background:rgba(10,10,10,0.95);backdrop-filter: blur(6px);padding:28px;z-index:50;transition:transform .35s ease}
    .side-menu.open{transform:translateX(0)}
    .side-menu h3{font-family:'Great Vibes',cursive;font-size:34px;margin-bottom:12px}
    .side-menu nav{display:flex;flex-direction:column;gap:12px;margin-top:12px}
    .side-menu a{color:#fff;text-decoration:none;padding:10px 12px;border-radius:8px;font-weight:600}
    .side-menu a:hover{background:rgba(255,255,255,0.03)}

    .cv-text{font-size:13px;opacity:.9;margin-top:6px}

    @media (max-width:720px){
      .intro-card{left:50%;transform:translateX(-50%);padding:14px}
      .headline{font-size:clamp(28px,9vw,64px)}
    }

  </style></head>
<body>  <div id="app"><button class="menu-btn" id="menuBtn" aria-label="Open menu"><span class="dots">⋯</span></button>

<aside class="side-menu" id="sideMenu" aria-hidden="true">
  <h3>Cook Edris</h3>
  <nav>
    <a href="international.html">International Dishes</a>
    <a href="fastfood.html">Fast Food Samples</a>
<a href="breakfast.html">Breakfast</a>
<a href="seafood.html">Seafood</a>
<a href="desserts.html">Desserts</a>
    <a href="cv.html">My CV</a>
  </nav>
</aside>

<section class="slideshow" id="slideshow">

  <article class="slide visible" style="background-image:url('https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=1600&q=80');" data-title="Spiced Lamb Platter">
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

  <div class="intro-card" role="region" aria-label="Introduction">
    <img src="My-photo.png" alt="Chef Edris portrait">
    <div class="intro-text">
      <strong>Hello, I'm Cook Edris</strong>
      <small>Chef's assistant • cook </small>
      <div class="thumbs" aria-hidden="false">
        <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=400&q=60" alt="food thumb 1">
        <img src="https://images.unsplash.com/photo-1543353071-087092ec393a?auto=format&fit=crop&w=400&q=60" alt="food thumb 2">
        <img src="https://images.unsplash.com/photo-1541544741938-0af808871cc0?auto=format&fit=crop&w=400&q=60" alt="food thumb 3">
      </div>
      <div class="cv-text"><a href="#cv" style="color:inherit;text-decoration:underline;">My CV</a></div>
    </div>
  </div>

</section>

<main style="padding:40px;background:#0b0b0b;color:#fff;">
  <section id="international" style="max-width:1000px;margin:40px auto;">
    <h2 style="font-family:'Great Vibes',cursive;font-size:36px;margin-bottom:8px">International Dishes</h2>
    <p>Gallery and recipes for refined international cuisine — explore dishes from around the world.</p>
    <a href="international.html" style="display:inline-block;margin-top:12px;padding:8px 20px;color:#fff;background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.3);border-radius:8px;text-decoration:none;">See More →</a>
</section>

<section id="fastfood" style="max-width:1000px;margin:40px auto;">
    <h2 style="font-family:'Great Vibes',cursive;font-size:36px;margin-bottom:8px">Fast Food Samples</h2>
    <p>Samples from the fast-food and street-food repertoire — explore my fast food creations below.</p>
    <a href="fastfood.html" style="display:inline-block;margin-top:12px;padding:8px 20px;color:#fff;background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.3);border-radius:8px;text-decoration:none;">See More →</a>
</section>

<section id="breakfast" style="max-width:1000px;margin:40px auto;">
    <h2 style="font-family:'Great Vibes',cursive;font-size:36px;margin-bottom:8px">Breakfast</h2>
    <p>Discover delicious and energizing breakfast dishes from around the world.</p>
    <a href="breakfast.html" style="display:inline-block;margin-top:12px;padding:8px 20px;color:#fff;background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.3);border-radius:8px;text-decoration:none;">See More →</a>
</section>

<section id="seafood" style="max-width:1000px;margin:40px auto;">
    <h2 style="font-family:'Great Vibes',cursive;font-size:36px;margin-bottom:8px">Seafood</h2>
    <p>Fresh seafood selections — from calamari to lobster and more.</p>
    <a href="seafood.html" style="display:inline-block;margin-top:12px;padding:8px 20px;color:#fff;background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.3);border-radius:8px;text-decoration:none;">See More →</a>
</section>

<section id="desserts" style="max-width:1000px;margin:40px auto;">
    <h2 style="font-family:'Great Vibes',cursive;font-size:36px;margin-bottom:8px">Desserts</h2>
    <p>Sweet and delightful desserts — enjoy a curated selection of world favorites.</p>
    <a href="desserts.html" style="display:inline-block;margin-top:12px;padding:8px 20px;color:#fff;background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.3);border-radius:8px;text-decoration:none;">See More →</a>
</section>

<section id="cv" style="max-width:1000px;margin:40px auto;">
    <h2 style="font-family:'Great Vibes',cursive;font-size:36px;margin-bottom:8px">My CV</h2>
    <p>View my professional chef résumé — experience, skills, and background.</p>
    <a href="cv.html" style="display:inline-block;margin-top:12px;padding:8px 20px;color:#fff;background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.3);border-radius:8px;text-decoration:none;">See My Full CV →</a>
</section>
</main>

  </div>  <script>
    (function(){
      const slides = Array.from(document.querySelectorAll('.slide'));
      let idx = 0;
      const show = i => {
        slides.forEach((s,si)=> s.classList.toggle('visible', si===i));
      };
      show(idx);
      const interval = setInterval(()=>{ idx = (idx+1) % slides.length; show(idx); }, 5000);

      const menuBtn = document.getElementById('menuBtn');
      const sideMenu = document.getElementById('sideMenu');
      menuBtn.addEventListener('click', ()=>{
        const open = sideMenu.classList.toggle('open');
        sideMenu.setAttribute('aria-hidden', !open);
      });

      const slideshow = document.getElementById('slideshow');
      let paused = false;
      slideshow.addEventListener('mouseenter', ()=>{ if(!paused) clearInterval(interval); paused=true });
      slideshow.addEventListener('mouseleave', ()=>{ if(paused){ setInterval(()=>{ idx = (idx+1) % slides.length; show(idx); }, 5000); paused=false }});

      document.addEventListener('keydown', (e)=>{
        if(e.key==='Escape' && sideMenu.classList.contains('open')){
          sideMenu.classList.remove('open'); sideMenu.setAttribute('aria-hidden','true');
        }
      });

    })();
  </script></body>
</html>
