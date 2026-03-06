<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>May I Court You Gel?</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;800&display=swap');

        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: #000000;
            font-family: 'Poppins', sans-serif;
            overflow: hidden;
            position: relative;
        }

        .container {
            text-align: center;
            background: rgba(30, 30, 30, 0.9);
            padding: 50px 30px;
            border-radius: 25px;
            box-shadow: 0 15px 35px rgba(255, 255, 255, 0.1);
            max-width: 90%;
            width: 450px;
            position: relative;
            z-index: 10;
            border: 2px solid #333;
        }

        h1 {
            color: #ff6b81;
            font-size: 2.8rem;
            margin-bottom: 15px;
            line-height: 1.2;
        }

        p {
            color: #ffffff;
            font-size: 1.2rem;
            margin-bottom: 40px;
        }

        .btn-group {
            display: flex;
            justify-content: center;
            gap: 30px;
            position: relative;
            height: 70px;
        }

        button {
            padding: 15px 40px;
            font-size: 1.3rem;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-family: 'Poppins', sans-serif;
            font-weight: 800;
            box-shadow: 0 5px 15px rgba(0,0,0,0.5);
        }

        .btn-yes {
            background-color: #ff6b81;
            color: white;
        }

        .btn-yes:hover {
            transform: scale(1.1);
            background-color: #ff4757;
        }

        .btn-no {
            background-color: #444;
            color: #ccc;
        }

        .btn-no:hover {
            transform: scale(1.1);
            background-color: #333;
        }

        /* Success Screen - No Animation */
        .success-screen {
            display: none;
            text-align: center;
        }

        .heart {
            font-size: 6rem;
            display: block;
            margin: 0 auto 20px;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- Question Section -->
        <div id="question-section">
            <h1>May I court you gel?</h1>
            <p>🙏🙏</p>
            
            <div class="btn-group">
                <button class="btn-yes" onclick="sayYes()">Yes</button>
                <button class="btn-no" onclick="sayNo()">No</button>
            </div>
        </div>

        <!-- Success Section (Yes) -->
        <div id="success-section" class="success-screen">
            <div class="heart"></div>
            <p>Sure nana, HAHAHAHAHA?</p>
        </div>

        <!-- No Section -->
        <div id="no-section" class="success-screen">
            <div class="heart"></div>
            <p>sge HAHAHAHAHA igna rako</p>
        </div>
    </div>

    <script>
        // Logic for "Yes" button
        function sayYes() {
            document.getElementById('question-section').style.display = 'none';
            document.getElementById('success-section').style.display = 'block';
        }

        // Logic for "No" button
        function sayNo() {
            document.getElementById('question-section').style.display = 'none';
            document.getElementById('no-section').style.display = 'block';
        }
    </script>
</body>
</html>
