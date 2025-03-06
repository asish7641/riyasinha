<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday My Love!</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
    <script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>
    <style>
        body {
            background-color: black;
            color: white;
            text-align: center;
            font-family: 'Arial', sans-serif;
            overflow: hidden;
        }
        .container {
            margin-top: 50px;
        }
        .message {
            font-size: 24px;
            margin-top: 20px;
        }
        .hidden-message {
            display: none;
            font-size: 22px;
            margin-top: 20px;
            position: relative;
        }
        button {
            background: red;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 18px;
            cursor: pointer;
            margin-top: 20px;
            border-radius: 5px;
        }
        @keyframes fall {
            from { transform: translateY(-10px); opacity: 1; }
            to { transform: translateY(100vh); opacity: 0; }
        }
        .heart {
            position: absolute;
            color: red;
            font-size: 20px;
            animation: fall linear infinite;
        }
        .rose {
            width: 100px;
            margin-top: 20px;
        }
        .flower {
            position: absolute;
            width: 20px;
            animation: fall linear infinite;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Hello Riya❤️</h1>
        <p class="message"> <span id="typed-text"></span></p>
        <button onclick="revealMessage()">Agot Tipa</button>
        <p class="hidden-message" id="hidden-message"> Happy Birthday...💖<br> 
Ajikar din ahn bht hoba r special din hn<br>
T na jorom oileis te tor dekita nw peiluis🤧<br>
Kaash tor lge tor kadat thaya, tor aath hn doriya, tore cheya tor b'day hn celebrate korluis, kintu kopal a nei, dureit ana lagil🤧...<br>
Tebou kittawnei dureittou dou homade prtou t hba bala oya harou oya thak mtiya...<br>
Aasha krwri abaka harou oya aaha2 khusi oya thawri, usade sara jibon hn ou harou khushi te thak mtiya...<br>
T morka bohot special, tor lge na totorle morta din hn pura nw or...<br>
T jesade oilou morta hba lagwri...jesade asot uhn ei morka perfect asot lgr😁...<br>
R kita ekortu, habita te matiya hodasu, tebou arak khani mating haee😉...<br>
Mor ahigit tor pohor hn thoitu, na mor aadar got tor mingal hn thoitu?..<br>
Tor lge mor jibon hn khalkortu, na torei mor jibon hn hongkortu?...<br>
Ahr kali kihn oitoi kungoi harpar, kintu mor mon hnt t ei thytei ahn hrpsu...<br>
Na tor aath hnt mor aath hn thoya tor ningsa hnt mor ningsa thoitu??<br>
T jehan mattei uhn😊<br>
<B> LOVE YOU😘 </B> <br>






</p>
	    </div>

    <script>
        // Typing Animation
        new Typed("#typed-text", {
            strings: ["A Special Message for You...", "My Love, My World!"],
            typeSpeed: 50,
            backSpeed: 25,
            loop: true
        });

        // Reveal Hidden Message with Infinite Love Effect
        function revealMessage() {
            let message = document.getElementById('hidden-message');
            message.style.display = 'block';
            setInterval(() => sprinkleHearts(), 300);
        }

        // Sprinkle Hearts Effect (Infinite Falling)
        function sprinkleHearts() {
            let heart = document.createElement('div');
            heart.innerHTML = '❤️';
            heart.classList.add('heart');
            heart.style.left = Math.random() * 100 + '%';
            heart.style.top = '-10px';
            heart.style.fontSize = Math.random() * 20 + 10 + 'px';
            heart.style.animationDuration = Math.random() * 3 + 2 + 's';
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 5000);
        }
    </script>
</body>
</html>
