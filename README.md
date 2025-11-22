<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Water Guardian — SDG 6</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    *{margin:0;padding:0;box-sizing:border-box;font-family:Arial, Helvetica, sans-serif}

    body{
      background:#e9f7ff;
      color:#0a2a43;
    }

    /* HERO */
    .hero{
      background:linear-gradient(rgba(0,101,165,0.65), rgba(0,101,165,0.75)),
                 url('https://images.unsplash.com/photo-1504274066651-8d31a536b11a?q=80&w=1200&auto=format&fit=crop') center/cover;
      height:420px;
      display:flex;
      align-items:center;
      justify-content:center;
      text-align:center;
      color:white;
      padding:20px;
    }
    .hero h1{font-size:42px;margin-bottom:12px}
    .hero p{max-width:600px;font-size:18px;margin:auto}

    .btn{
      display:inline-block;
      background:#00aaff;
      padding:10px 18px;
      border-radius:8px;
      margin-top:18px;
      color:white;
      text-decoration:none;
      font-weight:bold;
    }

    /* SECTION */
    .section{
      padding:40px 22px;
      max-width:1100px;
      margin:auto;
    }
    .section h2{
      font-size:32px;
      margin-bottom:18px;
      text-align:center;
    }

    /* PROJECT CARDS */
    .grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:20px;
      margin-top:20px;
    }
    .card{
      background:white;
      padding:16px;
      border-radius:12px;
      box-shadow:0 4px 14px rgba(0,0,0,0.1);
    }
    .card img{
      width:100%;
      height:160px;
      object-fit:cover;
      border-radius:8px;
      margin-bottom:10px;
    }
    .card h3{margin-bottom:6px}
    .card p{color:#444;font-size:14px}

    /* TIMELINE */
    .timeline{
      margin-top:20px;
      border-left:4px solid #0099dd;
      padding-left:16px;
    }
    .timeline div{
      margin-bottom:20px;
      padding-left:10px;
    }
    .dot{
      width:14px;
      height:14px;
      background:#0099dd;
      border-radius:50%;
      position:relative;
      left:-23px;
      top:10px;
    }
    .timeline strong{font-size:15px}

    /* FOOTER */
    footer{
      background:#003d66;
      color:white;
      padding:20px;
      text-align:center;
      margin-top:40px;
    }
  </style>
</head>
<body>

  <!-- HERO -->
  <div class="hero">
    <div>
      <h1>Water Guardian</h1>
      <p>Empowering communities with clean water, sanitation, and sustainable water management — aligned with United Nations SDG 6.</p>
      <a href="#projects" class="btn">Explore Our Projects</a>
    </div>
  </div>

  <!-- PROJECTS -->
  <div class="section" id="projects">
    <h2>Featured Water Projects</h2>

    <div class="grid">

      <div class="card">
        <img src="https://images.unsplash.com/photo-1529618160092-2d6ec4a29a91?q=80&w=1200&auto=format&fit=crop" alt="">
        <h3>Village Water Pump</h3>
        <p>Installation of solar-powered water pumps for remote villages to ensure 24/7 water supply.</p>
      </div>

      <div class="card">
        <img src="https://images.unsplash.com/photo-1556760544-74068565f05c?q=80&w=1200&auto=format&fit=crop" alt="">
        <h3>School Sanitation Program</h3>
        <p>Providing clean toilets, hand-washing stations, and hygiene education for students.</p>
      </div>

      <div class="card">
        <img src="https://images.unsplash.com/photo-1580910051074-3eb694886505?q=80&w=1200&auto=format&fit=crop" alt="">
        <h3>Rainwater Harvesting Tanks</h3>
        <p>Large-capacity tanks installed in water-scarce areas to store clean rainwater.</p>
      </div>

    </div>
  </div>

  <!-- TIMELINE -->
  <div class="section">
    <h2>Our Progress</h2>

    <div class="timeline">

      <div>
        <div class="dot"></div>
        <strong>2023 — First Well Built</strong>
        <p>Our pilot project successfully delivered clean water to 68 families.</p>
      </div>

      <div>
        <div class="dot"></div>
        <strong>2024 — Expanded to Schools</strong>
        <p>Hygiene and sanitation programs launched in 12 rural schools.</p>
      </div>

      <div>
        <div class="dot"></div>
        <strong>2025 — Smart Water Sensors</strong>
        <p>Data-driven monitoring ensures water quality is safe and reliable.</p>
      </div>

    </div>
  </div>

  <!-- FOOTER -->
  <footer>
    Water Guardian • Supporting SDG 6: Clean Water & Sanitation
  </footer>

</body>
</html>

  



