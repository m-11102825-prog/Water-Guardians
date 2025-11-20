# Water-Guardians<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Water Guardians</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #e0f7fa;
    }
    header {
      background: #00acc1;
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      display: flex;
      justify-content: center;
      background: #00838f;
    }
    nav a {
      padding: 14px 20px;
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      background: #006064;
    }
    .content {
      padding: 20px;
      display: none;
    }
    .active {
      display: block;
    }
    .card {
      background: white;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
      margin-bottom: 20px;
    }
    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    button {
      padding: 10px 20px;
      background: #00acc1;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background: #00838f;
    }
  </style>
</head>
<body>
  <header>
    <h1>Water Guardians</h1>
  </header>

  <nav>
    <a onclick="showTab('tab1')">Why Clean Water Matters</a>
    <a onclick="showTab('tab2')">Water Challenges</a>
    <a onclick="showTab('tab3')">Solutions</a>
    <a onclick="showTab('tab4')">How You Can Help</a>
    <a onclick="showTab('feedback')">Feedback</a>
  </nav>

  <div id="tab1" class="content active card">
    <h2>Why Clean Water Matters</h2>
    <p>Clean water is essential for health, hygiene, and daily life. Many communities still struggle to access safe water sources.</p>
    <button onclick="alert('Fact: 1 in 3 people worldwide lack access to safe drinking water.')">Learn a Fact</button>
  </div>

  <div id="tab2" class="content card">
    <h2>Water Challenges</h2>
    <p>Pollution, climate change, and poor management affect water quality and availability.</p>
    <button onclick="alert('Challenge: Pollution from industries and households is a major threat to clean water.')">View Challenge</button>
  </div>

  <div id="tab3" class="content card">
    <h2>Solutions</h2>
    <p>Explore methods like water filtration, rainwater harvesting, and community clean-up efforts.</p>
    <button onclick="alert('Solution: Rainwater harvesting can provide clean water for daily use!')">View Solution</button>
  </div>

  <div id="tab4" class="content card">
    <h2>How You Can Help</h2>
    <p>Students can conserve water, raise awareness, or join school projects protecting water sources.</p>
    <button onclick="alert('Tip: Turn off taps tightly and reduce water waste in daily activities!')">Take Action</button>
  </div>

  <div id="feedback" class="content card">
    <h2>Feedback Form</h2>
    <form onsubmit="submitFeedback(event)">
      <label>Your Name:</label>
      <input type="text" required />

      <label>Your Feedback:</label>
      <textarea rows="5" required></textarea>

      <button type="submit">Submit</button>
    </form>
    <p id="response" style="color: green; font-weight: bold; margin-top: 10px;"></p>
  </div>

  <script>
    function showTab(tabId) {
      document.querySelectorAll('.content').forEach(section => section.classList.remove('active'));
      document.getElementById(tabId).classList.add('active');
    }

    function submitFeedback(event) {
      event.preventDefault();
      document.getElementById('response').innerText = "Thank you for your feedback!";
    }
  </script>
</body>
</html>



