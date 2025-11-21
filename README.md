<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Water Guardians</title>

    <style>
        body {
            margin: 0;
            font-family: "Segoe UI", Arial, sans-serif;
            background: #e7f7ff;
        }

        /* HEADER */
        header {
            background: linear-gradient(135deg, #00aaff, #0077cc);
            padding: 60px 20px;
            text-align: center;
            color: white;
            border-radius: 0 0 30px 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        header h1 {
            font-size: 45px;
            margin: 0;
        }
        header p {
            font-size: 18px;
            opacity: 0.9;
        }

        /* NAVIGATION */
        nav {
            display: flex;
            justify-content: center;
            gap: 20px;
            padding: 20px;
            background: white;
            position: sticky;
            top: 0;
            z-index: 10;
            border-bottom: 2px solid #bbe7ff;
        }

        nav button {
            padding: 12px 25px;
            font-size: 16px;
            border: 2px solid #0099dd;
            background: #ffffff;
            border-radius: 12px;
            cursor: pointer;
            transition: 0.3s;
        }

        nav button:hover {
            background: #0099dd;
            color: white;
        }

        /* TABS */
        .tab {
            display: none;
            max-width: 900px;
            margin: auto;
            padding: 20px;
            animation: fadeIn 0.4s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* CARDS */
        .card {
            background: white;
            padding: 25px;
            margin-bottom: 20px;
            border-radius: 20px;
            box-shadow: 0 6px 18px rgba(0,0,0,0.08);
        }

        .card h2 {
            margin-top: 0;
            color: #0077bb;
        }

        /* FEEDBACK FORM */
        input, textarea {
            width: 100%;
            padding: 12px;
            border-radius: 12px;
            border: 1.5px solid #0099dd;
            margin-top: 10px;
            font-size: 15px;
        }

        .submit-btn {
            background: #0077cc;
            color: white;
            padding: 12px 25px;
            border: none;
            border-radius: 12px;
            cursor: pointer;
            margin-top: 10px;
            transition: 0.3s;
        }
        .submit-btn:hover {
            background: #005fa3;
        }
    </style>
</head>

<body>

    <header>
        <h1>Water Guardians</h1>
        <p>Ensuring Clean Water for All — SDG 6</p>
    </header>

    <nav>
        <button onclick="openTab('why')">Why Clean Water?</button>
        <button onclick="openTab('challenges')">Challenges</button>
        <button onclick="openTab('solutions')">Solutions</button>
        <button onclick="openTab('help')">How You Can Help</button>
        <button onclick="openTab('feedback')">Feedback</button>
    </nav>

    <!-- WHY TAB -->
    <div id="why" class="tab" style="display:block;">
        <div class="card">
            <h2>Why Clean Water Matters</h2>
            <p>Clean water is essential for drinking, cooking, health, sanitation, and the environment.</p>
        </div>
    </div>

    <!-- CHALLENGES TAB -->
    <div id="challenges" class="tab">
        <div class="card">
            <h2>Water Challenges</h2>
            <p>Pollution, waste, and lack of access to clean water affect billions of people globally.</p>
        </div>
    </div>

    <!-- SOLUTIONS TAB -->
    <div id="solutions" class="tab">
        <div class="card">
            <h2>Solutions</h2>
            <p>Saving water, preventing pollution, improving systems, and educating communities.</p>
        </div>
    </div>

    <!-- HELP TAB -->
    <div id="help" class="tab">
        <div class="card">
            <h2>How You Can Help</h2>
            <p>Turn off taps, report leaks, reduce plastic waste, and support clean water projects.</p>
        </div>
    </div>

    <!-- FEEDBACK TAB -->
    <div id="feedback" class="tab">
        <div class="card">
            <h2>Feedback Form</h2>

            <label>Your Name:</label>
            <input type="text">

            <label>Your Message:</label>
            <textarea rows="5"></textarea>

            <button class="submit-btn">Submit</button>
        </div>
    </div>

    <script>
        function openTab(tabName) {
            document.querySelectorAll('.tab').forEach(t => t.style.display = "none");
            document.getElementById(tabName).style.display = "block";
        }
    </script>

</body>
</html>



  



