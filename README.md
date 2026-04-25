<!DOCTYPE html>
<html lang="id">

<head>
  <!-- ================= META ================= -->
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Personal Website</title>

  <!-- ================= GOOGLE FONT ================= -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <!-- ================= ICON ================= -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <!-- ================= SCROLL ANIMATION ================= -->
  <link rel="stylesheet" href="https://unpkg.com/aos@2.3.4/dist/aos.css">

  <!-- ================= STYLE ================= -->
  <style>

    /* ================= GLOBAL ================= */

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
    }

    body{
      font-family:'Poppins',sans-serif;
      background:#0d1117;
      color:#e6edf3;
      overflow-x:hidden;
    }

    .container{
      width:90%;
      max-width:1200px;
      margin:auto;
    }

    section{
      padding:90px 0;
      position:relative;
      z-index:2;
    }

    /* ================= PARTICLE BACKGROUND ================= */

    #particles-js{
      position:fixed;
      width:100%;
      height:100%;
      top:0;
      left:0;
      z-index:0;
      background:#0d1117;
    }

    /* ================= NAVBAR ================= */

    nav{
      position:fixed;
      width:100%;
      top:0;
      background:#0d1117;
      border-bottom:1px solid rgba(77,163,255,0.3);
      z-index:999;
    }

    nav .container{
      display:flex;
      justify-content:space-between;
      align-items:center;
      padding:15px;
    }

    .logo{
      font-size:1.7rem;
      font-weight:700;
      color:#4da3ff;
      text-shadow:0 0 10px #4da3ff;
    }

    .nav-menu{
      display:flex;
      list-style:none;
      gap:25px;
    }

    .nav-menu a{
      text-decoration:none;
      color:white;
      transition:0.3s;
    }

    .nav-menu a:hover{
      color:#4da3ff;
      text-shadow:0 0 8px #4da3ff;
    }

    /* ================= HERO ================= */

    .hero{
      height:100vh;
      display:flex;
      align-items:center;
      padding-top:80px;
    }

    .hero-content{
      display:flex;
      align-items:center;
      justify-content:space-between;
      flex-wrap:wrap;
      gap:40px;
    }

    .hero-text h1{
      font-size:3rem;
      margin-bottom:10px;
    }

    .hero-text p{
      margin-bottom:20px;
      color:#c9d1d9;
    }

    /* ================= BUTTON ================= */

    .btn{
      display:inline-block;
      padding:12px 25px;
      border-radius:8px;
      background:#4da3ff;
      text-decoration:none;
      color:white;
      transition:0.3s;
      box-shadow:0 0 10px #4da3ff;
    }

    .btn:hover{
      transform:scale(1.05);
      box-shadow:0 0 25px #4da3ff;
    }

    /* ================= FOTO PROFIL ================= */

    .profile-img{
      width:260px;
      height:260px;
      border-radius:50%;
      overflow:hidden;
      border:4px solid #4da3ff;
      box-shadow:0 0 25px #4da3ff;
      animation:float 4s ease-in-out infinite;
    }

    .profile-img img{
      width:100%;
      height:100%;
      object-fit:cover;
    }

    @keyframes float{
      0%{transform:translateY(0);}
      50%{transform:translateY(-12px);}
      100%{transform:translateY(0);}
    }

    /* ================= SECTION HEADER ================= */

    .section-header{
      text-align:center;
      margin-bottom:40px;
    }

    .section-header h2{
      font-size:2.2rem;
      color:#4da3ff;
      text-shadow:0 0 10px #4da3ff;
    }

    /* ================= ABOUT ================= */

    .about-text{
      max-width:700px;
      margin:auto;
      text-align:center;
      line-height:1.7;
    }

    /* ================= SOCIAL ================= */

    .social{
      display:flex;
      justify-content:center;
      flex-wrap:wrap;
      gap:30px;
    }

    .social a{
      padding:20px 30px;
      border-radius:10px;
      background:#161b22;
      color:white;
      text-decoration:none;
      display:flex;
      align-items:center;
      gap:12px;
      font-size:1.2rem;
      transition:0.3s;
      border:1px solid rgba(77,163,255,0.4);
    }

    .social a:hover{
      transform:translateY(-8px);
      box-shadow:0 0 25px #4da3ff;
    }

    .social i{
      font-size:1.5rem;
    }

    /* ================= FOOTER ================= */

    footer{
      text-align:center;
      padding:40px;
      border-top:1px solid rgba(77,163,255,0.3);
      background:#020409;
    }

    /* ================= CURSOR GLOW ================= */

    .cursor{
      position:fixed;
      width:25px;
      height:25px;
      border-radius:50%;
      background:rgba(77,163,255,0.6);
      box-shadow:0 0 15px #4da3ff,0 0 30px #4da3ff;
      pointer-events:none;
      transform:translate(-50%,-50%);
      z-index:9999;
    }

  </style>
</head>

<body>

  <!-- ================= PARTICLE BACKGROUND ================= -->
  <div id="particles-js"></div>

  <!-- ================= CURSOR ================= -->
  <div class="cursor"></div>

  <!-- ================= NAVBAR ================= -->

  <nav>
    <div class="container">

      <div class="logo">Erlando Area</div>

      <ul class="nav-menu">
        <li><a href="#home">Beranda</a></li>
        <li><a href="#about">Tentang</a></li>
        <li><a href="#social">Sosial</a></li>
      </ul>

    </div>
  </nav>

  <!-- ================= HERO ================= -->

  <section id="home" class="hero">

    <div class="container hero-content">

      <div class="hero-text" data-aos="fade-right">
        <h1>Vin Aka Erlando</h1>
        <p>Content Creator | Gamer | Streamer</p>
        <a href="#about" class="btn">Tentang Saya</a>
      </div>

      <div class="profile-img" data-aos="zoom-in">
        <img src="erlando.jpeg" alt="Foto Profil">
      </div>

    </div>

  </section>

  <!-- ================= ABOUT ================= -->

  <section id="about">

    <div class="container">

      <div class="section-header" data-aos="fade-up">
        <h2>Tentang Saya</h2>
      </div>

      <div class="about-text" data-aos="fade-up">
        <p>
         Yo! 👋
         Selamat datang di website gue. Gue orang yang suka banget sama dunia game dan
         teknologi. Di sini gue share beberapa hal tentang project, eksperimen IT, dan hal-hal
         random yang berhubungan sama dunia digital. Gue juga suka banget main game, jadi jangan kaget kalau ada beberapa konten tentang gaming.
         Gue juga aktif di Tiktok, jadi jangan lupa follow ya!!

        </p>
      </div>

    </div>

  </section>

  <!-- ================= SOCIAL ================= -->

  <section id="social">

    <div class="container">

      <div class="section-header" data-aos="fade-up">
        <h2>Sosial Media</h2>
      </div>

      <div class="social" data-aos="zoom-in">

        <a href="https://discord.gg/WQeqNawxH" target="_blank">
          <i class="fab fa-discord"></i>
            Discord
        </a>       

        <a href="https://www.tiktok.com/@ini.vincen?_r=1&_t=ZS-94eMtNpJa0A" target="_blank">
          <i class="fab fa-tiktok"></i>
          TikTok
        </a>

        <a href="https://www.instagram.com/vinmora__?igsh=MjN6NGJhaWx5NHps" target="_blank">
          <i class="fab fa-instagram"></i>
          Instagram
        </a>

        <a href="https://sociabuzz.com/vinakaerlando/tribe" target="_blank">
          <i class="fas fa-hand-holding-heart"></i>
          Socialbuzz
        </a>

      </div>

    </div>

  </section>

  <!-- ================= FOOTER ================= -->

  <footer>
    <p>© 2026 Personal Website</p>
  </footer>

  <!-- ================= SCRIPT ================= -->

  <!-- PARTICLES -->
  <script src="https://cdn.jsdelivr.net/npm/particles.js"></script>

  <script>
  particlesJS("particles-js",{
    particles:{
      number:{value:80},
      color:{value:"#4da3ff"},
      shape:{type:"circle"},
      opacity:{value:0.5},
      size:{value:3},
      line_linked:{
        enable:true,
        distance:150,
        color:"#4da3ff",
        opacity:0.4
      },
      move:{
        enable:true,
        speed:2
      }
    }
  });
  </script>

  <!-- SCROLL ANIMATION -->
  <script src="https://unpkg.com/aos@2.3.4/dist/aos.js"></script>

  <script>
    AOS.init({
      duration:1000,
      once:true
    });
  </script>

  <!-- CURSOR GLOW -->
  <script>

  const cursor=document.querySelector(".cursor");

  document.addEventListener("mousemove",e=>{
    cursor.style.left=e.clientX+"px";
    cursor.style.top=e.clientY+"px";
  });

  </script>

</body>
</html>
```
