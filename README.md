<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Water Guardian</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #e8f7ff;
            color: #003049;
        }
        header {
            background: linear-gradient(#0077b6, #0096c7);
            padding: 30px;
            text-align: center;
            color: white;
            font-size: 40px;
            font-weight: bold;
        }
        .section {
            padding: 40px;
            background: white;
            margin: 20px auto;
            width: 80%;
            border-radius: 20px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        }
        h2 {
            font-size: 32px;
            margin-bottom: 10px;
        }
        img.sec-img {
            width: 100%;
            border-radius: 15px;
            margin-top: 15px;
        }
        textarea {
            width: 100%;
            height: 130px;
            padding: 10px;
            border-radius: 10px;
            border: 2px solid #0077b6;
            resize: none;
            font-size: 16px;
        }
        button {
            margin-top: 15px;
            padding: 12px 20px;
            background: #0096c7;
            color: white;
            font-size: 18px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
        }
        button:hover {
            background: #0077b6;
        }
        #feedback-list {
            margin-top: 20px;
            background: #f0fbff;
            padding: 15px;
            border-radius: 10px;
        }
        .fb-item {
            background: #ffffff;
            padding: 10px;
            border-radius: 8px;
            margin-bottom: 10px;
            border-left: 5px solid #0096c7;
        }
    </style>
</head>
<body>
    <header>Water Guardian 🌊</header>

    <div class="section">
        <h2>Why Clean Water Matters</h2>
        <p>Clean water is essential for health, hygiene, agriculture, and the environment. Millions of people still lack access to safe drinking water, causing diseases and poverty.</p>
        <img class="sec-img" src="https://i.imgur.com/ZqU4EoT.jpeg" alt="Clean Water" />
    </div>

    <div class="section">
        <h2>Water Challenges</h2>
        <p>Challenges include pollution, waste, droughts, climate change, and lack of proper water treatment systems. These problems affect rivers, lakes, oceans, and the people who depend on them.</p>
        <img class="sec-img" src="https://i.imgur.com/xsJfFUt.jpeg" alt="Water Issues" />
    </div>

    <div class="section">
        <h2>Solutions</h2>
        <p>Solutions include better water management, reducing pollution, building water treatment plants, conserving water, and educating communities about protection efforts.</p>
        <img class="sec-img" src="https://i.imgur.com/WGzxe2E.jpeg" alt="Solutions" />
    </div>

    <div class="section">
        <h2>How You Can Help</h2>
        <ul>
            <li>Save water at home</li>
            <li>Avoid littering and reduce plastic waste</li>
            <li>Report water pollution</li>
            <li>Support clean water projects</li>
        </ul>
        <img class="sec-img" src="https://i.imgur.com/8pPrRHL.jpeg" alt="Help Water" />
    </div>

    <div class="section">
        <h2>Feedback</h2>
        <p>Share your thoughts or ideas to protect water resources:</p>
        <textarea id="feedback-input" placeholder="Write your feedback here..."></textarea>
        <button onclick="submitFeedback()">Submit Feedback</button>

        <div id="feedback-list"></div>
    </div>

    <script>
        function submitFeedback() {
            const input = document.getElementById('feedback-input');
            const text = input.value.trim();

            if (text === '') {
                alert('Please write something.');
                return;
            }

            const list = document.getElementById('feedback-list');
            const item = document.createElement('div');
            item.className = 'fb-item';
            item.textContent = text;

            list.appendChild(item);
            input.value = '';
        }
    </script>
</body>
</html>

