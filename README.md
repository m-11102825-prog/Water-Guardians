<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Water Guardian</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #eaf7ff; }
    header { background: #0077cc; color: white; padding: 20px; text-align: center; font-size: 32px; font-weight: bold; }
    .section { background: white; margin: 20px auto; padding: 20px; width: 80%; border-radius: 12px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); }
    .section h2 { color: #0077cc; }
    img { width: 100%; border-radius: 10px; margin-top: 15px; }
    textarea { width: 100%; height: 120px; border-radius: 8px; padding: 10px; font-size: 16px; }
    button { margin-top: 10px; padding: 10px 20px; font-size: 16px; cursor: pointer; background: #0077cc; color: white; border: none; border-radius: 8px; }
  </style>
</head>
<body>

<header>Water Guardian</header>

<div class="section">
  <h2>Why Clean Water Matters</h2>
  <p>Clean water is essential for life. It keeps communities healthy, protects ecosystems, and supports food production.</p>
  <img src="/mnt/data/c12ab307-0943-4cf5-adf7-a8901a85b374.png" alt="Clean Water Image">
</div>

<div class="section">
  <h2>Water Challenges</h2>
  <p>Pollution, waste, rising temperatures, and poor management threaten global water supplies.</p>
</div>

<div class="section">
  <h2>Solutions</h2>
  <p>We can fix water problems through conservation, recycling, protecting rivers, and improving sanitation systems.</p>
</div>

<div class="section">
  <h2>Feedback</h2>
  <p>Write your feedback below:</p>
  <textarea id="feedbackBox" placeholder="Enter your feedback..."></textarea>
  <button onclick="submitFeedback()">Submit</button>
  <p id="feedbackMessage" style="color: green; font-weight: bold; display: none;">Thank you for your feedback!</p>
</div>

<script>
function submitFeedback() {
  const box = document.getElementById('feedbackBox');
  if (box.value.trim() !== "") {
    document.getElementById('feedbackMessage').style.display = 'block';
    box.value = "";
  }
}
</script>

  <div class="section"> 
    <h2>How You Can Help</h2>
    <p>You can help protect water by saving water at home, avoiding pollution, joining clean-up programs, and spreading awareness about SDG 6.</p>
  </div>

  <div class="section">
    <h2>Global Water Facts</h2>
    <ul>
      <li>Over 2 billion people lack access to safe drinking water.</li>
      <li>Every year, millions of tons of plastic waste enter rivers and oceans.</li>
      <li>70% of the Earth's surface is water, but only 1% is drinkable.</li>
      <li>Water scarcity affects over 700 million people worldwide.</li>
    </ul>
    <img src="/mnt/data/c12ab307-0943-4cf5-adf7-a8901a85b374.png" alt="Water Info Image">
  </div>

</body>
</html>
