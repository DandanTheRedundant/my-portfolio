[index.html](https://github.com/user-attachments/files/28274402/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Your Name</title>

  <!-- Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
    }

    html{
      scroll-behavior:smooth;
    }

    body{
      font-family:'Inter',sans-serif;
      background:#0d0d0d;
      color:white;
      overflow-x:hidden;
    }

    /* NAVBAR */

    nav{
      position:fixed;
      top:0;
      left:0;
      width:100%;
      padding:25px 8%;
      display:flex;
      justify-content:space-between;
      align-items:center;
      z-index:1000;
      backdrop-filter:blur(10px);
      background:rgba(0,0,0,0.2);
    }

    .logo{
      font-size:1.2rem;
      font-weight:600;
      letter-spacing:2px;
    }

    nav ul{
      display:flex;
      gap:40px;
      list-style:none;
    }

    nav a{
      color:white;
      text-decoration:none;
      font-size:0.95rem;
      transition:0.3s;
    }

    nav a:hover{
      opacity:0.6;
    }

    /* HERO */

    .hero{
      height:100vh;
      display:flex;
      align-items:center;
      justify-content:space-between;
      padding:0 8%;
      position:relative;
    }

    .hero-text{
      max-width:600px;
      z-index:2;
    }

    .hero-text h1{
      font-size:6rem;
      line-height:0.95;
      font-weight:700;
      margin-bottom:20px;
    }

    .hero-text p{
      color:#9f9f9f;
      font-size:1.1rem;
      line-height:1.8;
      max-width:500px;
    }

    .hero-btn{
      display:inline-block;
      margin-top:40px;
      padding:14px 32px;
      border:1px solid white;
      color:white;
      text-decoration:none;
      border-radius:50px;
      transition:0.3s;
    }

    .hero-btn:hover{
      background:white;
      color:black;
    }

    /* BIG BACKGROUND TEXT */

    .bg-text{
      position:absolute;
      right:-100px;
      top:50%;
      transform:translateY(-50%);
      font-size:18rem;
      font-weight:700;
      color:rgba(255,255,255,0.03);
      user-select:none;
      pointer-events:none;
      line-height:1;
    }

    /* SECTIONS */

    section{
      padding:120px 8%;
    }

    .section-title{
      font-size:3rem;
      margin-bottom:50px;
      font-weight:700;
    }

    /* ABOUT */

    .about{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:60px;
      align-items:center;
    }

    .about img{
      width:100%;
      border-radius:25px;
      object-fit:cover;
    }

    .about-text p{
      color:#9f9f9f;
      line-height:1.9;
      font-size:1rem;
    }

    /* PROJECTS */

    .projects-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
      gap:30px;
    }

    .project-card{
      background:#161616;
      border-radius:25px;
      overflow:hidden;
      transition:0.4s;
    }

    .project-card:hover{
      transform:translateY(-10px);
    }

    .project-card img{
      width:100%;
      height:250px;
      object-fit:cover;
    }

    .project-content{
      padding:30px;
    }

    .project-content h3{
      margin-bottom:15px;
      font-size:1.4rem;
    }

    .project-content p{
      color:#9f9f9f;
      line-height:1.7;
    }

    /* CONTACT */

    .contact{
      text-align:center;
    }

    .contact h2{
      font-size:4rem;
      margin-bottom:20px;
    }

    .contact p{
      color:#9f9f9f;
      margin-bottom:40px;
    }

    .contact a{
      display:inline-block;
      padding:16px 40px;
      background:white;
      color:black;
      text-decoration:none;
      border-radius:50px;
      font-weight:600;
      transition:0.3s;
    }

    .contact a:hover{
      transform:scale(1.05);
    }

    /* FOOTER */

    footer{
      padding:40px;
      text-align:center;
      color:#777;
      border-top:1px solid rgba(255,255,255,0.08);
    }

    /* MOBILE */

    @media(max-width:900px){

      .hero{
        flex-direction:column;
        justify-content:center;
        text-align:center;
      }

      .hero-text h1{
        font-size:4rem;
      }

      .bg-text{
        font-size:8rem;
        right:0;
      }

      .about{
        grid-template-columns:1fr;
      }

      nav ul{
        gap:20px;
      }

    }

  </style>
</head>

<body>

  <!-- NAV -->

  <nav>

    <div class="logo">
      YOURNAME
    </div>

    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#projects">Work</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>

  </nav>

  <!-- HERO -->

  <section class="hero">

    <div class="hero-text">

      <h1>
        Creative<br>
        Developer
      </h1>

      <p>
        I design and build modern digital experiences,
        personal brands, and visually stunning websites.
      </p>

      <a href="#projects" class="hero-btn">
        View Projects
      </a>

    </div>

    <div class="bg-text">
      CREATE
    </div>

  </section>

  <!-- ABOUT -->

  <section id="about">

    <h2 class="section-title">
      About Me
    </h2>

    <div class="about">

      <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?q=80&w=1200&auto=format&fit=crop" alt="Profile">

      <div class="about-text">

        <p>
          Hello, I’m Your Name — a designer and developer
          passionate about creating elegant and immersive
          digital experiences.
        </p>

        <br>

        <p>
          I specialize in modern UI design, branding,
          creative development, and building websites
          that feel premium and memorable.
        </p>

      </div>

    </div>

  </section>

  <!-- PROJECTS -->

  <section id="projects">

    <h2 class="section-title">
      Featured Work
    </h2>

    <div class="projects-grid">

      <div class="project-card">

        <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=1200&auto=format&fit=crop" alt="">

        <div class="project-content">

          <h3>Portfolio Website</h3>

          <p>
            A sleek and minimal portfolio website
            designed for creators and freelancers.
          </p>

        </div>

      </div>

      <div class="project-card">

        <img src="https://images.unsplash.com/photo-1558655146-9f40138edfeb?q=80&w=1200&auto=format&fit=crop" alt="">

        <div class="project-content">

          <h3>Brand Identity</h3>

          <p>
            Modern branding package with typography,
            visual identity, and social assets.
          </p>

        </div>

      </div>

      <div class="project-card">

        <img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?q=80&w=1200&auto=format&fit=crop" alt="">

        <div class="project-content">

          <h3>Creative Landing Page</h3>

          <p>
            Interactive landing page focused on
            storytelling and smooth animations.
          </p>

        </div>

      </div>

    </div>

  </section>

  <!-- CONTACT -->

  <section id="contact">

    <div class="contact">

      <h2>
        Let's Work Together
      </h2>

      <p>
        Available for freelance work, collaborations,
        and creative projects.
      </p>

      <a href="mailto:youremail@gmail.com">
        Contact Me
      </a>

    </div>

  </section>

  <!-- FOOTER -->

  <footer>

    © 2026 Your Name — All Rights Reserved

  </footer>

</body>
</html>
