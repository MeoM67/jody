# jody
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>بتصيري الفلنتاين حقي جودي?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: pink;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        h1 {
            color: red;
            font-size: 2em;
        }
        .buttons {
            position: relative;
            margin-top: 20px;
        }
        button {
            font-size: 1.5em;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            margin: 10px;
            transition: 0.3s;
        }
        #yes {
            background-color: rgb(119, 0, 255);
            color: white;
            border-radius: 10px;
        }
        #no {
            background-color: white;
            color: black;
            border: 2px solid black;
            position: absolute;
        }
        #heart {
            font-size: 100px;
            color: red;
            animation: heartbeat 1s infinite;
        }
        @keyframes heartbeat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }
    </style>
</head>
<body>

    <h1>Will You Be My Valentine, Jody? ❤️</h1>
    <div id="heart">❤️</div>
    
    <div class="buttons">
        <button id="yes" onclick="yesClicked()">Yes</button>
        <button id="no" onmouseover="moveNo()">No</button>
    </div>

    <script>
        function yesClicked() {
            document.body.innerHTML = "<h1>Yay! ❤️</h1><p>احبكككك اميرتييي!</p>";
        }

        function moveNo() {
            let button = document.getElementById("no");
            let x = Math.random() * window.innerWidth * 0.6;
            let y = Math.random() * window.innerHeight * 0.6;
            button.style.transform = `translate(${x}px, ${y}px)`;
        }
    </script>

</body>
</html>
