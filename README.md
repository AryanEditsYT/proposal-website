<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be Mine? 💖</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe6e6;
            padding: 50px;
        }
        .card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            display: inline-block;
        }
        .btn {
            margin: 10px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 18px;
        }
        .yes { background: #ff4d4d; color: white; }
        .no { background: #ccc; color: black; }
        .retry-card {
            display: none;
            margin-top: 20px;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        }
    </style>
    <script>
        function noClicked() {
            document.getElementById("retry-card").style.display = "block";
            document.getElementById("retry-text").innerText = "Are you really sure? 🥺";
        }
        function yesClicked() {
            document.getElementById("retry-card").style.display = "block";
            document.getElementById("retry-text").innerText = "Now can i flex i have u? 😏";
        }
        function finalDecision(answer) {
            if (answer === 'yes') {
                alert("Yay! ik you will love me <3 ❤️");
            } else {
                alert("Pls think agian! 😊");
            }
        }
    </script>
</head>
<body>
    <div class="card">
        <h1>Hey [Sanyuuuu],</h1>
        <p>I have something special to ask you... 💕</p>
        <h2>Will you be my Girlfreind? 🥰</h2>
        <button class="btn yes" onclick="yesClicked()">Yes</button>
        <button class="btn no" onclick="noClicked()">No</button>
    </div>
    
    <div id="retry-card" class="retry-card">
        <h2 id="retry-text">Are you really sure? 🥺</h2>
        <button class="btn yes" onclick="finalDecision('yes')">Yes</button>
        <button class="btn no" onclick="finalDecision('pls think agian')">No</button>
    </div>
</body>
</html>
