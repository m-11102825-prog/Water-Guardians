<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Water Guardian — School Project</title>
  <style>
    :root{--accent:#0077cc;--dark:#003049;--muted:#6b7280}
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, Arial;background:linear-gradient(180deg,#eaf7ff 0%,#ffffff 60%);color:var(--dark)}

    /* layout */
    .sidebar{position:fixed;left:0;top:0;height:100%;width:240px;background:var(--accent);color:white;padding:28px 18px;display:flex;flex-direction:column;gap:10px}
    .brand{font-weight:800;font-size:20px;margin-bottom:8px}
    .nav-btn{background:transparent;border:0;color:inherit;text-align:left;padding:10px;border-radius:8px;cursor:pointer;font-weight:700}
    .nav-btn:hover{background:rgba(255,255,255,0.08)}
    .content{margin-left:260px;padding:28px;max-width:1000px}

    /* top card */
    .hero{background:linear-gradient(90deg,rgba(0,119,182,0.95),rgba(0,150,199,0.95));color:white;padding:28px;border-radius:12px;box-shadow:0 8px 30px rgba(2,6,23,0.08);display:flex;gap:20px;align-items:center}
    .hero h1{margin:0;font-size:26px}
    .hero p{margin:0;color:rgba(255,255,255,0.93)}

    /* page card */
    .page{display:none;background:white;border-radius:12px;padding:22px;margin-top:20px;box-shadow:0 8px 30px rgba(2,6,23,0.06);animation:fade .36s ease}
    .page.active{display:block}
    @keyframes fade{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:none}}

    h2{color:var(--accent);margin-top:0}
    p.lead{color:var(--muted);font-size:15px;line-height:1.6}

    .page-img{width:100%;height:320px;object-fit:cover;border-radius:10px;margin:14px 0}

    /* feedback */
    .form-row{display:grid;grid-template-columns:1fr 1fr;gap:12px}
    input,textarea{width:100%;padding:10px;border-radius:8px;border:1px solid #e6eef6;font-size:15px}
    textarea{min-height:120px;resize:vertical}
    .btn{background:var(--accent);color:white;border:0;padding:10px 14px;border-radius:8px;font-weight:700;cursor:pointer}

    /* feedback list */
    .fb-list{margin-top:14px;display:grid;gap:10px}
    .fb-item{background:#f5fdff;border-left:4px solid var(--accent);padding:10px;border-radius:8px}
    .meta{font-size:13px;color:var(--muted)}

    /* responsive */
    @media (max-width:880px){.sidebar{position:relative;width:100%;height:auto;flex-direction:row;overflow:auto;padding:12px}.content{margin-left:0;padding:16px}.hero{flex-direction:column;align-items:flex-start}.page-img{height:220px}}

    /* small helper */
    .muted{color:var(--muted)}
  </style>
</head>
<body>

  <aside class="sidebar" aria-label="Main navigation">
    <div class="brand">Water Guardian</div>
    <div class="muted" style="font-size:13px;margin-bottom:6px">School Project — SDG 6</div>
    <button class="nav-btn" onclick="show('cleanwater')">Why Clean Water Matters</button>
    <button class="nav-btn" onclick="show('challenges')">Water Challenges</button>
    <button class="nav-btn" onclick="show('solutions')">Solutions</button>
    <button class="nav-btn" onclick="show('help')">How You Can Help</button>
    <button class="nav-btn" onclick="show('facts')">Global Water Facts</button>
    <button class="nav-btn" onclick="show('feedback')">Feedback</button>
    <div style="flex:1"></div>
    <div style="font-size:13px" class="muted">Built with HTML, CSS & JS</div>
  </aside>

  <main class="content">
    <section class="hero">
      <div>
        <h1>Water Guardian — Protecting Water, Protecting Life</h1>
        <p class="muted">A school project exploring SDG 6: Clean Water & Sanitation. Use the menu to navigate each topic.</p>
      </div>
      <div style="margin-left:auto;font-size:13px;opacity:0.95" class="muted">Author: You</div>
    </section>

    <!-- Pages: each page is a full topic with its own image and longer description -->

    <article id="cleanwater" class="page active" aria-labelledby="clean-title">
      <h2 id="clean-title">Why Clean Water Matters</h2>
      <p class="lead">Clean water supports human health, economic development, education, and ecosystems. Children who have access to safe water attend school more regularly. Communities that secure their water supply experience fewer illnesses, improved livelihoods, and stronger resilience to environmental shocks.</p>
      <img class="page-img" src="https://raw.githubusercontent.com/m-11102825-prog/Water%20Guardian/main/images/water_image.png" alt="Clean water example">
      <h3>Health and Hygiene</h3>
      <p class="lead">Unsafe water causes waterborne diseases such as cholera and diarrhea. By providing clean drinking water and improved sanitation, we reduce disease spread and protect vulnerable groups like young children and the elderly.</p>
      <h3>Education & Economy</h3>
      <p class="lead">When students don't need to fetch water, they spend more time in school. Healthy communities are more productive: fewer sick days and stronger local economies.</p>
    </article>

    <article id="challenges" class="page" aria-labelledby="challenges-title">
      <h2 id="challenges-title">Water Challenges</h2>
      <p class="lead">The world faces complex water challenges: pollution from industry and agriculture, plastic and chemical contamination, aging infrastructure that leaks millions of liters daily, and shifting rainfall patterns due to climate change.</p>
      <img class="page-img" src="https://raw.githubusercontent.com/m-11102825-prog/Water%20Guardian/main/images/water_image.png" alt="Water pollution example">
      <h3>Pollution & Waste</h3>
      <p class="lead">Untreated wastewater and agricultural runoff introduce nitrates, phosphates, and pathogens into rivers and groundwater. Plastics and oil spills further harm aquatic life.</p>
      <h3>Scarcity & Climate</h3>
      <p class="lead">Droughts and melting glaciers reduce freshwater availability. In many regions, demand outpaces supply, leading to conflict and hardship.</p>
    </article>

    <article id="solutions" class="page" aria-labelledby="solutions-title">
      <h2 id="solutions-title">Solutions</h2>
      <p class="lead">Several practical and technological solutions help restore and protect water resources. These include building proper wastewater treatment plants, installing household water filters, promoting rainwater harvesting, and protecting watersheds.</p>
      <img class="page-img" src="https://raw.githubusercontent.com/m-11102825-prog/Water%20Guardian/main/images/water_image.png" alt="Water treatment example">
      <h3>Community-Led Projects</h3>
      <p class="lead">Local involvement is key: training community members to maintain wells, teaching hygiene in schools, and using inexpensive filter technology can create durable change.</p>
      <h3>Policy & Innovation</h3>
      <p class="lead">Government policies that protect rivers and funds for infrastructure, combined with innovation (smart sensors, efficient irrigation), scale solutions faster.</p>
    </article>

    <article id="help" class="page" aria-labelledby="help-title">
      <h2 id="help-title">How You Can Help</h2>
      <p class="lead">Everyone can take action. Simple daily habits and community projects add up to real impact.</p>
      <img class="page-img" src="https://raw.githubusercontent.com/m-11102825-prog/Water%20Guardian/main/images/water_image.png" alt="Community helping">
      <ul>
        <li>Conserve water: shorter showers, full loads of laundry, and fixing leaks.</li>
        <li>Reduce pollution: dispose of chemicals properly and reduce single-use plastics.</li>
        <li>Support local projects or volunteer with NGOs working on water access.</li>
        <li>Share knowledge: teach others about hygiene and safe water practices.</li>
      </ul>
    </article>

    <article id="facts" class="page" aria-labelledby="facts-title">
      <h2 id="facts-title">Global Water Facts</h2>
      <p class="lead">Facts help us understand the scale and urgency of problems.</p>
      <img class="page-img" src="https://raw.githubusercontent.com/m-11102825-prog/Water%20Guardian/main/images/water_image.png" alt="Water facts">
      <ol>
        <li>More than 2 billion people lack access to safe drinking water.</li>
        <li>Over 80% of the world's wastewater returns to the environment untreated.</li>
        <li>Water demand is projected to rise by up to 55% by 2050 in some regions.</li>
      </ol>
    </article>

    <article id="feedback" class="page" aria-labelledby="feedback-title">
      <h2 id="feedback-title">Feedback</h2>
      <p class="lead">Please share your feedback or ideas. Your responses help improve this project.</p>

      <div style="max-width:760px">
        <div class="form-row">
          <input id="fbName" placeholder="Your name (optional)" />
          <input id="fbEmail" placeholder="Email (optional)" />
        </div>
        <textarea id="fbMessage" placeholder="Write your feedback here..."></textarea>
        <div style="display:flex;gap:8px;align-items:center;margin-top:8px">
          <button class="btn" onclick="saveFeedback()">Submit Feedback</button>
          <div id="fbSaved" class="muted" style="display:none">Saved locally ✅</div>
        </div>

        <div id="fbList" class="fb-list" aria-live="polite"></div>
      </div>
    </article>

  </main>

  <script>
    // Navigation: show a single page
    function show(id){
      document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
      const el = document.getElementById(id);
      if(el) el.classList.add('active');
      // scroll to top of content for better UX
      window.scrollTo({top:0,behavior:'smooth'});
    }

    // Feedback: use localStorage to persist feedback on user's browser
    const FB_KEY = 'wg_feedback_v1';
    function loadFeedback(){
      const raw = localStorage.getItem(FB_KEY);
      if(!raw) return [];
      try{ return JSON.parse(raw) }catch(e){return []}
    }
    function renderFeedback(){
      const list = document.getElementById('fbList');
      list.innerHTML = '';
      const items = loadFeedback();
      if(items.length===0){ list.innerHTML = '<div class="muted">No feedback yet — be the first to add!</div>'; return; }
      items.slice().reverse().forEach(it =>{
        const d = document.createElement('div'); d.className='fb-item';
        d.innerHTML = `<div style="font-weight:700">${escapeHtml(it.name||'Anonymous')}</div><div class="meta">${escapeHtml(it.email||'')}</div><div style="margin-top:6px">${escapeHtml(it.message)}</div>`;
        list.appendChild(d);
      })
    }
    function saveFeedback(){
      const name = document.getElementById('fbName').value.trim();
      const email = document.getElementById('fbEmail').value.trim();
      const msg = document.getElementById('fbMessage').value.trim();
      if(!msg){ alert('Please write a feedback message.'); return; }
      const items = loadFeedback();
      items.push({name,email,message:msg,ts:Date.now()});
      localStorage.setItem(FB_KEY, JSON.stringify(items));
      document.getElementById('fbSaved').style.display='inline-block';
      document.getElementById('fbMessage').value='';
      setTimeout(()=>document.getElementById('fbSaved').style.display='none',1500);
      renderFeedback();
    }
    function escapeHtml(s){ return String(s).replace(/[&<>\"']/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c])) }

    // initial render
    renderFeedback();
  </script>

</body>
</html>
