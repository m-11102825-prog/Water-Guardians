<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Water Guardian</title>
<style>
  body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #eaf7ff;
  }

  /* SIDEBAR */
  .sidebar {
    position: fixed;
    top: 0;
    left: 0;
    width: 230px;
    height: 100%;
    background: #004b8d;
    padding-top: 20px;
    color: white;
  }

  .sidebar h2 {
    text-align: center;
    margin-bottom: 30px;
  }

  .sidebar a {
    display: block;
    color: white;
    padding: 12px 20px;
    text-decoration: none;
    font-size: 18px;
    transition: 0.3s;
  }

  .sidebar a:hover {
    background: #0066c2;
  }

  /* MAIN CONTENT */
  .content {
    margin-left: 260px;
    padding: 30px;
  }

  .section {
    background: white;
    margin-bottom: 30px;
    padding: 25px;
    border-radius: 12px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  }

  .section h1, .section h2 {
    color: #0077cc;
  }

  img {
    width: 100%;
    border-radius: 12px;
    margin-top: 15px;
  }

  textarea {
    width: 100%;
    height: 140px;
    border-radius: 10px;
    padding: 10px;
    font-size: 16px;
  }

  button {
    margin-top: 10px;
    padding: 10px 20px;
    font-size: 16px;
    background: #0077cc;
    border: none;
    border-radius: 10px;
    color: white;
    cursor: pointer;
  }

  button:hover {
    background: #005fa3;
  }
</style>
</head>
<body>

<div class="sidebar">
  <h2>Water Guardian</h2>
  <a href="#cleanwater">Why Clean Water Matters</a>
  <a href="#challenges">Water Challenges</a>
  <a href="#solutions">Solutions</a>
  <a href="#help">How You Can Help</a>
  <a href="#facts">Water Facts</a>
  <a href="#feedback">Feedback</a>
</div>

<div class="content">

  <div class="section" id="cleanwater">
    <h1>Why Clean Water Matters</h1>
    <p>Clean water is essential for every living organism on Earth. It keeps our bodies healthy, prevents diseases, and supports daily needs like cooking, drinking, bathing, and cleaning. Without clean water, communities struggle with illness, poor hygiene, and limited access to education because children often spend hours collecting water instead of attending school.</p>
    <p>Clean water also supports agriculture and food production. Farmers rely on water to grow crops, raise animals, and maintain healthy soil. Industries depend on water for manufacturing, cooling systems, and product development.</p>
    <p>Healthy ecosystems—like rivers, lakes, wetlands, and oceans—need clean water to support fish, plants, and wildlife. When water becomes polluted, entire ecosystems collapse, affecting humans and animals alike.</p>
    <img src="/mnt/data/c12ab307-0943-4cf5-adf7-a8901a85b374.png" alt="Water Image">
  </div>

  <div class="section" id="challenges">
    <h2>Water Challenges</h2>
    <p>The world faces many water-related challenges. Pollution from factories, sewage, chemicals, and plastics contaminates water sources, making them unsafe for drinking or farming. In some countries, people must walk for miles to collect water, and sometimes the water they find is still unsafe.</p>
    <p>Climate change is making water problems worse. Rising temperatures dry up rivers and lakes, causing droughts. Melting glaciers reduce long-term water supplies for millions of people. Heavy rainfall leads to floods that spread pollution and destroy homes.</p>
    <p>Lastly, poor water management—such as leaking pipes, lack of filtration systems, and outdated infrastructure—causes millions of liters of water to be wasted every day.</p>
  </div>

  <div class="section" id="solutions">
    <h2>Solutions</h2>
    <p>There are many effective solutions that can help protect and restore the world’s water resources. Improving water treatment systems ensures communities receive safe and clean drinking water. Modern filtration technology can remove harmful bacteria, chemicals, and waste from polluted water.</p>
    <p>Protecting rivers and forests prevents pollution and soil erosion. Reusing and recycling water in agriculture and industry reduces overall water consumption. Farmers can also use drip irrigation and water-efficient crops to save water.</p>
    <p>Governments, schools, and organizations play a big role by creating programs, policies, and awareness campaigns to educate people about water conservation. Innovation and teamwork are the keys to protecting water for future generations.</p>
  </div>

  <div class="section" id="help">
    <h2>How You Can Help</h2>
    <p>Even small actions can make a huge difference when everyone works together. Here’s how you can help protect water every day:</p>
    <ul>
      <li>Take shorter showers to reduce water usage.</li>
      <li>Fix leaking taps at home to prevent water wastage.</li>
      <li>Use reusable bottles and bags to reduce plastic pollution.</li>
      <li>Dispose of oil, paint, and chemicals properly—never pour them into sinks or drains.</li>
      <li>Plant trees and support green spaces that help filter water naturally.</li>
      <li>Educate friends and family about the importance of water conservation.</li>
    </ul>
    <p>When communities get involved, real change becomes possible.</p>
  </div>

  <div class="section" id="facts">
    <h2>Global Water Facts</h2>
    <p>Understanding the current water situation helps us see why SDG 6 is so important. Here are some powerful facts:</p>
    <ul>
      <li>2 billion people still live without clean and safe drinking water.</li>
      <li>Every minute, a child dies from water-related illnesses.</li>
      <li>Over 80% of wastewater in the world flows back into nature without being treated.</li>
      <li>By 2050, water demand may increase by 55% due to farming, industries, and population growth.</li>
      <li>Polluted water affects marine life, killing millions of fish, turtles, and birds each year.</li>
    </ul>
    <p>These facts show why protecting water is not only important but urgent. Our actions today decide the future of the planet.</p>
  </div>

  <div class="section" id="feedback">
    <h2>Feedback</h2>
    <p>Write your feedback here:</p>
    <textarea id="feedbackBox" placeholder="Your feedback..."></textarea>
    <button onclick="submitFeedback()">Submit</button>
    <p id="feedbackMessage" style="display:none; color:green; font-weight:bold;">Thank you for your feedback!</p>
  </div>

</div>

<script>
function submitFeedback() {
  let fb = document.getElementById('feedbackBox').value.trim();
  if (fb !== "") {
    document.getElementById('feedbackMessage').style.display = 'block';
    document.getElementById('feedbackBox').value = "";
  }
}
</script>

</body>
</html>
