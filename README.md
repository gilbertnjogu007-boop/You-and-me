<!DOCTYPE html>
<html>
<head>
    <title>For You ❤️</title>
    <style>
        body {
            text-align: center;
            font-family: Arial;
            margin-top: 100px;
            background-color: #ffe6e6;
        }
        h1 {
            color: #ff4d4d;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 10px;
        }
        #yes {
            background-color: #4CAF50;
            color: white;
        }
        #no {
            background-color: #f44336;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>

<h1>Will you be my lover? ❤️</h1>

<button id="yes" onclick="yesClicked()">Yes ❤️</button>
<button id="no" onmouseover="moveNo()">No 😢</button>

<script>
function yesClicked() {
    document.body.innerHTML = "<h1>Yay! I knew it 😍❤️</h1>";
}

function moveNo() {
    let x = Math.random() * window.innerWidth;
    let y = Math.random() * window.innerHeight;
    document.getElementById("no").style.left = x + "px";
    document.getElementById("no").style.top = y + "px";
}
</script>

</body>
</html>
