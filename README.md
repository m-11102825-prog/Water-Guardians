<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Water Guardians</title>
  <style>
    /* --- Modern Blue Card Style --- */
    :root{--bg:#e9f9ff;--accent1:#00aaff;--accent2:#0077cc;--card:#ffffff}
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter, "Segoe UI", Arial, sans-serif;background:var(--bg);color:#04323f}
    header{
      background:linear-gradient(135deg,var(--accent1),var(--accent2));
      color:white;padding:48px 20px;text-align:center;border-bottom-left-radius:18px;border-bottom-right-radius:18px;
      box-shadow:0 6px 20px rgba(2,40,60,0.08)
    }
    header h1{margin:0;font-size:2.2rem;letter-spacing:0.3px}
    header p{margin:8px 0 0;opacity:0.95}

    nav{display:flex;gap:12px;justify-content:center;padding:18px;background:transparent;flex-wrap:wrap;margin-top:18px}
    .nav-btn{background:var(--card);border:1px solid rgba(0,0,0,0.06);padding:10px 18px;border-radius:12px;cursor:pointer;font-weight:600}
    .nav-btn.active{box-shadow:0 8px 22px rgba(3,63,96,0.06);transform:translateY(-3px);border-color:var(--accent1)}
    .container{max-width:1000px;margin:22px auto;padding:0 18px}
    .tab{display:none}
    .tab.active{display:block}
    .card{background:var(--card);padding:20px;border-radius:14px;box-shadow:0 10px 30px rgba(3,40,50,0.04);margin-bottom:18px}
    h2{color:var(--accent2);margin-top:0}
    label{display:block;margin-top:10px;font-weight:600}
    input,textarea{width:100%;padding:10px;border-radius:10px;border:1px solid rgba(3,63,96,0.08);margin-top:8px;font-size:14px}
    .btn{background:var(--accent2);color:white;padding:10px 16px;border-radius:10px;border:none;cursor:pointer;margin-top:12px}
    footer{text-align:center;color:#5b6d73;margin:26px 0 50px;font-size:14px}

    /* small responsive */
    @media (max-width:720px){
      header h1{font-size:1.6rem}
      .nav-btn{padding:8px 12px;font-size:14px}
    }
  </style>
</head>
<body>
  <!-- Defensive script: remove any visible literal "<!DOCTYPE html>" nodes if present in the body -->
  <script>
    (function removeVisibleDoctype(){
      try {
        // Walk text nodes inside body and remove nodes containing '<!DOCTYPE html>'
        const walker = document.createTreeWalker(document.body, NodeFilter.SHOW_TEXT, null, false);
        const toRemove = [];
        while(walker.nextNode()){
          const txt = walker.currentNode.nodeValue;
          if(txt && txt.includes('<!DOCTYPE html>')){
            // remove the substring or the whole text node if it's only doctype
            if(txt.trim() === '<!DOCTYPE html>'){
              toRemove.push(walker.currentNode);
            } else {
              walker.currentNode.nodeValue = txt.replace(/<!DOCTYPE html>/g, '');
            }
          }
        }
        toRemove.forEach(n => n.parentNode && n.parentNode.removeChild(n));
      } catch (e) { /* fail silently */ }
    })();
  </script>

  <header>
    <h1>Water Guardians</h1>
    <p>Learn • Solve • Act — Clean Water for Everyone (SDG 6)</p>
  </header>

  <nav aria-label="Main navigation" id="mainNav" style="padding:12px 18px;display:flex;justify-content:center;flex-wrap:wrap;gap:8px">
    <button class="nav-btn active" data-tab="why">Why Clean Water?</button>
    <button class="nav-btn" data-tab="challenges">Challenges</button>
    <button class="nav-btn" data-tab="solutions">Solutions</button>
    <button class="nav-btn" data-tab="help">How You Can Help</button>
    <button class="nav-btn" data-tab="feedback">Feedback</button>
  </nav>

  <main class="container" role="main">
    <section id="why" class="tab active">
      <div class="card">
        <h2>Why Clean Water Matters</h2>
        <p>Access to safe water supports health, education and livelihoods. Clean water prevents disease and helps communities thrive.</p>
      </div>
    </section>

    <section id="challenges" class="tab">
      <div class="card">
        <h2>Water Challenges</h2>
        <ul>
          <li>Pollution from households and industry</li>
          <li>Insufficient infrastructure for safe supply</li>
          <li>Climate variability causing droughts and floods</li>
        </ul>
      </div>
    </section>

    <section id="solutions" class="tab">
      <div class="card">
        <h2>Solutions</h2>
        <p>Filtration, rainwater harvesting, protection of watersheds and behaviour change (less waste, fixing leaks) are practical solutions.</p>
      </div>
    </section>

    <section id="help" class="tab">
      <div class="card">
        <h2>How You Can Help</h2>
        <ol>
          <li>Fix leaking taps and save water</li>
          <li>Organize a local river/lake clean-up</li>
          <li>Build a DIY filter demo for school</li>
        </ol>
      </div>
    </section>

    <section id="feedback" class="tab">
      <div class="card">
        <h2>Feedback & Ideas</h2>
        <form id="feedbackForm">
          <label for="name">Name</label>
          <input id="name" type="text" placeholder="Your name (or team)">

          <label for="idea">Idea or Feedback</label>
          <textarea id="idea" rows="5" placeholder="Describe your idea"></textarea>

          <button class="btn" type="submit">Save Feedback</button>
          <div id="msg" style="margin-top:10px;color:green;font-weight:600"></div>
        </form>

        <div style="margin-top:12px">
          <strong>Saved (local)</strong>
          <div id="saved" style="margin-top:8px;color:#4b6168"></div>
        </div>
      </div>
    </section>
  </main>

  <footer>Made for school — Water Guardians • Focus: SDG 6</footer>

  <script>
    // Tab switching
    document.querySelectorAll('.nav-btn').forEach(btn=>{
      btn.addEventListener('click', ()=> {
        document.querySelectorAll('.nav-btn').forEach(b=>b.classList.remove('active'));
        btn.classList.add('active');
        const tab = btn.dataset.tab;
        document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
        const sel = document.getElementById(tab);
        if(sel) sel.classList.add('active');
        window.scrollTo({top:0, behavior:'smooth'});
      });
    });

    // Feedback saved to localStorage
    const FB_KEY = 'water_guardians_fb_v2';
    const form = document.getElementById('feedbackForm');
    const msg = document.getElementById('msg');
    const saved = document.getElementById('saved');

    function loadSaved(){
      const arr = JSON.parse(localStorage.getItem(FB_KEY) || '[]');
      if(arr.length === 0) saved.innerText = 'No saved feedback.';
      else saved.innerHTML = arr.slice(0,6).map(x=>`• <strong>${escapeHtml(x.name)}</strong> (${x.date}): ${escapeHtml(x.idea)}`).join('<br>');
    }

    form.addEventListener('submit', e=>{
      e.preventDefault();
      const name = document.getElementById('name').value.trim();
      const idea = document.getElementById('idea').value.trim();
      if(!name || !idea){ msg.style.color = 'crimson'; msg.innerText = 'Please fill in both fields.'; return; }
      const arr = JSON.parse(localStorage.getItem(FB_KEY) || '[]');
      arr.unshift({name, idea, date: new Date().toLocaleString()});
      localStorage.setItem(FB_KEY, JSON.stringify(arr));
      form.reset(); msg.style.color = 'green'; msg.innerText = 'Saved locally — copy to submit to teacher if needed.';
      loadSaved();
    });

    // small helper
    function escapeHtml(s){ return s.replaceAll('&','&amp;').replaceAll('<','&lt;').replaceAll('>','&gt;'); }

    // On load
    window.addEventListener('DOMContentLoaded', () => {
      loadSaved();
      // Defensive: in rare server cases the doctype may appear as text inserted at top of body.
      // This removes any visible element nodes that match exactly "<!DOCTYPE html>".
      try {
        const nodes = Array.from(document.body.childNodes);
        for(const n of nodes){
          if(n.nodeType === Node.TEXT_NODE && n.nodeValue && n.nodeValue.trim() === '<!DOCTYPE html>'){
            n.parentNode.removeChild(n);
          }
          if(n.nodeType === Node.ELEMENT_NODE && n.textContent && n.textContent.trim() === '<!DOCTYPE html>'){
            n.parentNode.removeChild(n);
          }
        }
      } catch(e){}
    });
  </script>
</body>
</html>



  



