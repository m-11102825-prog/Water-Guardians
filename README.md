<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Water Guardians</title>
  <meta name="description" content="Water Guardians — student-focused interactive site about clean water (SDG 6)." />

  <style>
    /* -------------------- Reset & Base -------------------- */
    :root{
      --bg:#e8f7fb;
      --card:#ffffff;
      --accent:#00bcd4;
      --accent-2:#037b8c;
      --muted:#6b7c85;
      --glass: rgba(255,255,255,0.6);
      --radius:14px;
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;background:linear-gradient(180deg,var(--bg),#dff3f8);color:#053040}
    a{color:inherit}

    header{
      background:linear-gradient(90deg,var(--accent),var(--accent-2));
      color:white;padding:28px 18px;text-align:center;box-shadow:0 6px 18px rgba(1,43,53,0.12);
      border-bottom-left-radius:18px;border-bottom-right-radius:18px
    }
    header h1{margin:0;font-size:1.75rem;letter-spacing:0.6px}
    header p{margin:6px 0 0;opacity:0.95;font-size:0.95rem}

    /* -------------------- Layout -------------------- */
    .container{max-width:1100px;margin:20px auto;padding:18px}
    .top-row{display:flex;gap:18px;align-items:center;margin-bottom:18px}

    /* Nav tabs */
    .tabs{display:flex;gap:10px;background:transparent;padding:8px;border-radius:12px}
    .tab-btn{background:var(--card);padding:10px 14px;border-radius:10px;border:1px solid rgba(5,48,64,0.06);cursor:pointer;display:inline-flex;align-items:center;gap:8px}
    .tab-btn.active{box-shadow:0 8px 20px rgba(1,43,53,0.06);transform:translateY(-3px);border-color:var(--accent);}
    .tab-btn svg{width:18px;height:18px;opacity:0.95}

    /* Main grid */
    .grid{display:grid;grid-template-columns:1fr 360px;gap:18px}
    @media (max-width:980px){.grid{grid-template-columns:1fr} .top-row{flex-direction:column;align-items:stretch}}

    .card{background:var(--card);padding:18px;border-radius:var(--radius);box-shadow:0 6px 20px rgba(7,35,44,0.06);}

    h2{margin-top:0}
    p.lead{color:var(--muted);margin-top:6px}

    /* Accordion */
    .accordion{margin-top:8px}
    .acc-item{border-radius:10px;overflow:hidden;border:1px solid rgba(5,48,64,0.06);margin-bottom:10px}
    .acc-head{display:flex;justify-content:space-between;align-items:center;padding:12px 14px;background:linear-gradient(180deg,var(--glass),transparent);cursor:pointer}
    .acc-body{padding:12px 14px;border-top:1px solid rgba(5,48,64,0.04);display:none}

    /* Quiz */
    .quiz .q{margin-bottom:12px}
    .options button{display:block;width:100%;text-align:left;padding:10px;margin:6px 0;border-radius:8px;border:1px solid rgba(3,59,66,0.06);background:#f8feff;cursor:pointer}
    .options button.correct{border-color:green}
    .options button.wrong{border-color:#d9534f}

    /* Sidebar */
    .sidebar .small{font-size:0.95rem;color:var(--muted)}
    .stat-row{display:flex;gap:10px;margin-top:12px}
    .stat{flex:1;background:linear-gradient(180deg,#fff,#f3fcff);padding:10px;border-radius:10px;text-align:center}
    .stat h3{margin:6px 0 0}

    /* Feedback form */
    form label{display:block;margin-top:10px;font-weight:600}
    input[type=text],textarea{width:100%;padding:10px;border-radius:8px;border:1px solid rgba(5,48,64,0.08)}
    .btn{background:var(--accent);color:white;padding:10px 14px;border-radius:8px;border:none;cursor:pointer;margin-top:10px}

    footer{max-width:1100px;margin:22px auto;text-align:center;color:var(--muted);font-size:0.95rem}

    /* small helpers */
    .muted{color:var(--muted)}
    .hidden{display:none}

    /* subtle wave animation header underline */
    .wave{width:100%;height:8px;margin-top:12px;opacity:0.9}

  </style>
</head>
<body>

  <header>
    <h1>Water Guardians</h1>
    <p>Learn • Solve • Act — Clean Water for Everyone (SDG 6)</p>
    <svg class="wave" viewBox="0 0 1440 40" preserveAspectRatio="none"><path d="M0 20 C 360 0 720 40 1080 20 C 1260 10 1440 30 1440 30 L1440 40 L0 40 Z" fill="rgba(255,255,255,0.12)"></path></svg>
  </header>

  <main class="container">
    <div class="top-row">
      <div class="tabs card" role="tablist" aria-label="Main tabs">
        <button class="tab-btn active" data-tab="why" onclick="switchTab(event)">
          <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2v20" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/><path d="M5 12h14" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>
          Why Clean Water
        </button>
        <button class="tab-btn" data-tab="challenges" onclick="switchTab(event)">
          <svg viewBox="0 0 24 24"><path d="M12 3v18" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" stroke="currentColor"/></svg>
          Water Challenges
        </button>
        <button class="tab-btn" data-tab="solutions" onclick="switchTab(event)">
          <svg viewBox="0 0 24 24"><path d="M12 2l3 7h7l-5.6 4.2L20 21l-8-5-8 5 1.6-7.8L0 9h7l3-7z" fill="currentColor"/></svg>
          Solutions
        </button>
        <button class="tab-btn" data-tab="action" onclick="switchTab(event)">
          <svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="10" stroke="currentColor" stroke-width="1.2" fill="none"/></svg>
          How You Can Help
        </button>
        <button class="tab-btn" data-tab="feedback" onclick="switchTab(event)">
          <svg viewBox="0 0 24 24"><path d="M21 15a2 2 0 01-2 2H7l-4 4V5a2 2 0 012-2h14a2 2 0 012 2z" fill="currentColor"/></svg>
          Feedback
        </button>
      </div>

      <div style="flex:1"></div>

      <div style="min-width:220px" class="card sidebar">
        <div class="small">Quick stats</div>
        <div class="stat-row">
          <div class="stat"><strong>1 in 3</strong><div class="muted">lack safe water</div></div>
          <div class="stat"><strong>SDG 6</strong><div class="muted">Clean Water</div></div>
        </div>

        <div style="margin-top:12px" class="small">Student challenge</div>
        <div style="margin-top:8px">Design a DIY filter using household items — upload your idea in feedback!</div>
      </div>
    </div>

    <div class="grid">
      <!-- Main content column -->
      <section id="mainContent">

        <!-- WHY tab -->
        <article id="tab-why" class="card">
          <h2>Why Clean Water Matters</h2>
          <p class="lead">Clean water is the foundation for health, education and livelihoods. Unsafe water increases disease, reduces school attendance and impacts entire communities.</p>

          <div class="accordion" id="whyAcc">
            <div class="acc-item">
              <div class="acc-head" onclick="toggleAcc(this)">
                <div><strong>Health & Hygiene</strong><div class="muted">Water for drinking, cooking, and sanitation</div></div>
                <div>+</div>
              </div>
              <div class="acc-body">Access to clean water reduces diarrhoeal disease and lets people focus on school and work rather than fetching water.</div>
            </div>

            <div class="acc-item">
              <div class="acc-head" onclick="toggleAcc(this)">
                <div><strong>Education</strong><div class="muted">Attendance and performance improve</div></div>
                <div>+</div>
              </div>
              <div class="acc-body">When water and sanitation are available at schools, students — especially girls — are more likely to attend consistently.</div>
            </div>

            <div class="acc-item">
              <div class="acc-head" onclick="toggleAcc(this)">
                <div><strong>Economy & Community</strong><div class="muted">Time saved, jobs enabled</div></div>
                <div>+</div>
              </div>
              <div class="acc-body">Households with nearby water sources save hours per day, freeing time for study and income activities.</div>
            </div>
          </div>
        </article>

        <!-- CHALLENGES tab -->
        <article id="tab-challenges" class="card hidden">
          <h2>Water Challenges</h2>
          <p class="lead">Pollution, scarcity, and infrastructure gaps are some key problems. Choose a challenge below to learn more.</p>

          <div class="accordion">
            <div class="acc-item">
              <div class="acc-head" onclick="toggleAcc(this)"><div><strong>Pollution</strong><div class="muted">Waste & chemicals</div></div><div>+</div></div>
              <div class="acc-body">Household and industrial waste can contaminate freshwater sources making them unsafe without treatment.</div>
            </div>
            <div class="acc-item">
              <div class="acc-head" onclick="toggleAcc(this)"><div><strong>Climate impacts</strong><div class="muted">Droughts & floods</div></div><div>+</div></div>
              <div class="acc-body">Changing rainfall patterns make water availability unpredictable in many regions.</div>
            </div>
            <div class="acc-item">
              <div class="acc-head" onclick="toggleAcc(this)"><div><strong>Poor infrastructure</strong><div class="muted">Pipes & sanitation</div></div><div>+</div></div>
              <div class="acc-body">Many areas lack safe piped water and sanitation systems, increasing health risks.</div>
            </div>
          </div>

          <div style="margin-top:14px">
            <strong>Explore a case study</strong>
            <p class="muted">(Teacher idea) — research a local river or watershed: test water quality, note pollution sources, and propose fixes.</p>
          </div>
        </article>

        <!-- SOLUTIONS tab -->
        <article id="tab-solutions" class="card hidden">
          <h2>Solutions</h2>
          <p class="lead">Communities combine simple tech and good practices: filtration, rainwater harvesting, safe storage and policies.</p>

          <div class="acc-item" style="margin-bottom:10px">
            <div class="acc-head" onclick="toggleAcc(this)"><div><strong>Household filters</strong><div class="muted">DIY and low-cost</div></div><div>+</div></div>
            <div class="acc-body">Use sand, charcoal and gravel layers to build simple filters. Always boil or disinfect water after filtering if contamination is severe.</div>
          </div>

          <div class="acc-item" style="margin-bottom:10px">
            <div class="acc-head" onclick="toggleAcc(this)"><div><strong>Rainwater harvesting</strong><div class="muted">Collect & store</div></div><div>+</div></div>
            <div class="acc-body">Capturing roof runoff into tanks provides a local source for non-potable and, when treated, potable use.</div>
          </div>

          <div style="margin-top:12px">
            <strong>Student Project</strong>
            <p class="muted">Build a mini rain collector and measure how much water it collects in a week — compare with classmates.</p>
          </div>
        </article>

        <!-- ACTION tab -->
        <article id="tab-action" class="card hidden">
          <h2>How You Can Help</h2>
          <p class="lead">Small daily changes and projects at school can make big differences.</p>

          <ul>
            <li>Conserve water at home — shorter showers, fixed leaks.</li>
            <li>Organize school clean-ups near water bodies.</li>
            <li>Run awareness campaigns and share facts.</li>
            <li>Design a DIY water filter as a science project.</li>
          </ul>

          <div style="margin-top:12px">
            <strong>Interactive quiz — test yourself!</strong>
            <div class="quiz card" style="margin-top:10px;padding:12px">
              <div id="quiz"></div>
              <div id="quizResult" class="muted" style="margin-top:8px"></div>
            </div>
          </div>
        </article>

        <!-- FEEDBACK tab -->
        <article id="tab-feedback" class="card hidden">
          <h2>Feedback & Ideas</h2>
          <p class="muted">Share project ideas or upload descriptions of your DIY filters/projects.</p>

          <form id="feedbackForm">
            <label for="name">Name</label>
            <input id="name" type="text" placeholder="Your name or team" required />
            <label for="idea">Your idea / Feedback</label>
            <textarea id="idea" rows="5" placeholder="Describe your idea or feedback" required></textarea>
            <button class="btn" type="submit">Send Feedback</button>
            <div id="feedbackMsg" style="margin-top:10px;color:green;font-weight:600"></div>
          </form>

          <div style="margin-top:12px">
            <strong>Saved feedback (local)</strong>
            <div id="savedList" class="muted" style="margin-top:8px"></div>
          </div>
        </article>

      </section>

      <!-- Sidebar column -->
      <aside>
        <div class="card">
          <h3>Try this — Mini tasks</h3>
          <ol>
            <li>Measure how long you boil water at home and try to reduce time safely.</li>
            <li>Count how many taps at school drip — report to maintenance.</li>
            <li>Create a poster about 3 water-saving tips.</li>
          </ol>
        </div>

        <div class="card" style="margin-top:12px">
          <h3>Resources</h3>
          <ul class="muted">
            <li><a href="https://www.un.org/sustainabledevelopment/water-and-sanitation/" target="_blank">UN — Water & Sanitation</a></li>
            <li><a href="https://www.who.int/news-room/fact-sheets/detail/drinking-water" target="_blank">WHO — Drinking water facts</a></li>
          </ul>
        </div>
      </aside>
    </div>

  </main>

  <footer>Made for school — Water Guardians • Focus: SDG 6 • Save locally or publish to GitHub Pages</footer>

  <script>
    /* ---------- Tab handling ---------- */
    function switchTab(e){
      if(e) e.preventDefault();
      const btn = e.currentTarget || e.target.closest('.tab-btn');
      const tab = btn?.dataset?.tab;
      document.querySelectorAll('.tab-btn').forEach(b=>b.classList.remove('active'));
      btn.classList.add('active');

      // hide all content articles
      document.querySelectorAll('article[id^="tab-"]').forEach(a=>a.classList.add('hidden'));
      document.getElementById('tab-'+tab).classList.remove('hidden');
      window.scrollTo({top:0,behavior:'smooth'});
    }

    // initialize: attach to first tab if needed
    document.addEventListener('DOMContentLoaded',()=>{
      // quiz init
      initQuiz();
      loadFeedback();
    });

    /* ---------- Accordion ---------- */
    function toggleAcc(el){
      const body = el.nextElementSibling;
      const open = body.style.display === 'block';
      // close siblings
      el.parentElement.parentElement.querySelectorAll('.acc-body').forEach(b=>b.style.display='none');
      if(!open) body.style.display='block'; else body.style.display='none';
    }

    /* ---------- Simple quiz ---------- */
    const quizData = [
      {q:'Which practice saves the most household water?',opts:['Long showers','Fixing leaks','Leaving tap on'],a:1},
      {q:'Rainwater harvesting is useful for:',opts:['Potable water without treatment','Non-potable uses and, if treated, potable','Never useful'],a:1},
      {q:'A simple DIY filter often uses layers of:',opts:['Chocolate, sugar, salt','Sand, charcoal, gravel','Plastic and metal'],a:1}
    ];
    function initQuiz(){
      const container = document.getElementById('quiz');
      container.innerHTML='';
      quizData.forEach((item,i)=>{
        const div = document.createElement('div'); div.className='q';
        const q = document.createElement('div'); q.innerHTML=`<strong>Q${i+1}.</strong> ${item.q}`;
        div.appendChild(q);
        const opts = document.createElement('div'); opts.className='options';
        item.opts.forEach((o,oi)=>{
          const btn = document.createElement('button'); btn.type='button'; btn.innerText=o;
          btn.addEventListener('click',()=>{
            // visual feedback
            if(oi===item.a){ btn.classList.add('correct'); document.getElementById('quizResult').innerText='Correct!'; }
            else{ btn.classList.add('wrong'); document.getElementById('quizResult').innerText='Try again!'; }
            // disable siblings
            Array.from(opts.children).forEach(b=>b.disabled=true);
          });
          opts.appendChild(btn);
        });
        div.appendChild(opts); container.appendChild(div);
      });
    }

    /* ---------- Feedback (local saving) ---------- */
    const FB_KEY = 'water_guardians_feedback_v1';
    document.getElementById('feedbackForm').addEventListener('submit', function(e){
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const idea = document.getElementById('idea').value.trim();
      if(!name||!idea) return;
      const arr = JSON.parse(localStorage.getItem(FB_KEY) || '[]');
      arr.unshift({name,idea,date:new Date().toLocaleString()});
      localStorage.setItem(FB_KEY, JSON.stringify(arr));
      document.getElementById('feedbackMsg').innerText='Thanks — saved locally! (You can copy and upload to GitHub if needed)';
      this.reset(); loadFeedback();
    });
    function loadFeedback(){
      const arr = JSON.parse(localStorage.getItem(FB_KEY) || '[]');
      const el = document.getElementById('savedList');
      if(!el) return;
      if(arr.length===0){ el.innerText='No feedback yet.'; return; }
      el.innerHTML = arr.slice(0,6).map(f=>`• <strong>${escapeHtml(f.name)}</strong> (${f.date}): ${escapeHtml(f.idea)}`).join('<br>');
    }
    function escapeHtml(s){return s.replaceAll('&','&amp;').replaceAll('<','&lt;').replaceAll('>','&gt;')}

    /* small helper: ensure correct initial tab */
    (function setInitial(){
      // show 'why' by default (already visible)
    })();

  </script>
</body>
</html>

  



