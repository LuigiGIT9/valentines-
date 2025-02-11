<!DOCTYPE html>
<html>
<head>
    <title>Will You Be My First Valentine, LOVELOVE? ❤️</title>
    <style>
        body {
            text-align: center;
            font-family: 'Comic Sans MS', cursive, sans-serif;
            background: linear-gradient(to right, #ff758c, #ff7eb3);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            overflow: hidden;
            position: relative;
        }
        h1 {
            font-size: 36px;
            color: white;
            text-shadow: 2px 2px 5px #ff3366;
        }
        .btn-container {
            margin-top: 20px;
            position: relative;
        }
        button {
            font-size: 18px;
            padding: 12px 25px;
            margin: 10px;
            border: none;
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s ease-in-out;
        }
        #yes {
            background-color: #ff3366;
            color: white;
            font-size: 18px;
        }
        #no {
            background-color: #666;
            color: white;
            position: absolute;
        }
        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: red;
            clip-path: polygon(50% 15%, 90% 0, 100% 50%, 50% 100%, 0 50%, 10% 0);
            opacity: 0.8;
            animation: float 3s infinite linear;
        }
        @keyframes float {
            0% { transform: translateY(0); opacity: 0.8; }
            50% { transform: translateY(-30px); opacity: 0.5; }
            100% { transform: translateY(-60px); opacity: 0; }
        }
    </style>
    <script>
        let yesSize = 18;

        function sayYes() {
            alert("Buti naman Love yesss!! -Love Luigi Your Future");
        }

        function moveNoButton() {
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            document.getElementById("no").style.left = x + "px";
            document.getElementById("no").style.top = y + "px";
        }

        function growYesButton() {
            yesSize += 5;
            document.getElementById("yes").style.fontSize = yesSize + "px";
        }

        function createHeart() {
            let heart = document.createElement("div");
            heart.classList.add("heart");
            heart.style.left = Math.random() * 100 + "vw";
            heart.style.animationDuration = Math.random() * 3 + 2 + "s";
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 3000);
        }

        setInterval(createHeart, 300);
    </script>
</head>
<body>
    <h1>Will You Be My First Valentine Daniella Bianca Alcayde in short LOVELOVE? ❤️</h1>
    <div class="btn-container">
        <button id="yes" onclick="sayYes()" onmouseover="growYesButton()">Yes</button>
        <button id="no" onmouseover="moveNoButton()">No</button>
    </div>
</body>
</html>
