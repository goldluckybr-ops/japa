<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feliz Aniversário, Japinha!</title>
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #b71c1c 0%, #000000 100%);
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
            overflow-x: hidden;
        }
        .card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            padding: 30px;
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            max-width: 450px;
            width: 90%;
            box-shadow: 0 15px 35px rgba(0,0,0,0.5);
            animation: slideIn 1s ease-out;
        }
        .profile-img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 4px solid #ff5252;
            object-fit: cover;
            margin-bottom: 20px;
        }
        h1 { color: #ff5252; margin-bottom: 5px; }
        h2 { font-size: 1.2rem; font-weight: 300; margin-top: 0; }
        p { line-height: 1.6; font-size: 0.95rem; text-align: justify; }
        .btn-music {
            background: #ff5252;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 25px;
            cursor: pointer;
            margin-top: 15px;
            font-weight: bold;
        }
        .joke {
            margin-top: 20px;
            font-style: italic;
            color: #ff8a80;
            border-top: 1px solid rgba(255,255,255,0.1);
            padding-top: 15px;
        }
        @keyframes slideIn {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>

<div class="card">
    <img src="foto.jpg" alt="Yasmin e Você" class="profile-img">
    
    <h1>Parabéns, Japinha! 🎂</h1>
    <h2>20 Aninhos de pura luz!</h2>

    <p>
        Feliz aniversário Japinha, infelizmente não vou conseguir estar contigo no momento em que você estiver fazendo 20 aninhos mas quero que saiba que você é uma pessoa muito incrível, e a pessoa mais legal que conheço, continue sendo essa garota animada que sempre tira risada dos outros e continue com esse seu carisma, por mais que eu não vá estar aí sinta-se abraçada pelo angu, feliz aniversário Yasmin, ansioso pra ir ai.
    </p>

    <div class="joke">
        "Angu sentes saudades..." ❤️
    </div>

    <button class="btn-music" onclick="playMusic()">Clique para tocar Restless 🎵</button>
    
    <audio id="bdaySong" loop>
        <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
        </audio>
</div>

<script>
    function playMusic() {
        var audio = document.getElementById("bdaySong");
        if (audio.paused) {
            audio.play();
            document.querySelector('.btn-music').innerText = "Tocando Restless... 🎶";
        } else {
            audio.pause();
            document.querySelector('.btn-music').innerText = "Tocar Música 🎵";
        }
    }
</script>

</body>
</html>
