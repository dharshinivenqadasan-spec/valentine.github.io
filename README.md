<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Be My Valentine? ❤️</title>
<style>
    body {
        text-align: center;
        font-family: Arial, sans-serif;
        background-color: #ffdde1;
        overflow: hidden;
    }

    h1 {
        margin-top: 100px;
        color: #d6336c;
        font-size: 40px;
    }

    .btn {
        padding: 15px 30px;
        font-size: 20px;
        border: none;
        border-radius: 10px;
        cursor: pointer;
        position: absolute;
    }

    #yesBtn {
        background-color: #ff4d6d;
        color: white;
        left: 45%;
        top: 55%;
    }

    #noBtn {
        background-color: #6c757d;
        color: white;
        left: 55%;
        top: 55%;
    }

    #message {
        font-size: 30px;
        margin-top: 50px;
        color: #c9184a;
    }
</style>
</head>
<body>

<h1>Will You Be My Valentine? 💖</h1>

<button id="yesBtn" class="btn" onclick="sayYes()">Yes 💘</button>
<button id="noBtn" class="btn">No 💔</button>

<div id="message"></div>

<script>
const noBtn = document.getElementById("noBtn");

noBtn.addEventListener("mouseover", function() {
    const x = Math.random() * (window.innerWidth - noBtn.offsetWidth);
    const y = Math.random() * (window.innerHeight - noBtn.offsetHeight);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
});

function sayYes() {
    document.getElementById("message").innerHTML = "YAYYYY!! ❤️ I knew you'd say YES 😘💞";
}
</script>

</body>
</html>
