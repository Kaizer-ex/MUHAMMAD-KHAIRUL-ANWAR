MUHAMMAD KHAIRUL ANWAR
<html lang="ms">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kejutan Gila Meriah 🎉</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            text-align: center;
            background: linear-gradient(45deg, #ff00ff, #ffcc00, #00ffcc, #ff3300);
            background-size: 400% 400%;
            animation: gradientBG 5s infinite alternate;
            color: white;
            overflow: hidden;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            100% { background-position: 100% 50%; }
        }

        .container {
            margin-top: 100px;
        }

        .btn {
            background: rgb(255, 223, 0);
            color: black;
            padding: 15px 30px;
            font-size: 22px;
            border: none;
            cursor: pointer;
            margin-top: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(255, 255, 0, 0.9);
            transition: transform 0.2s, box-shadow 0.2s;
        }

        .btn:hover {
            transform: scale(1.1);
            box-shadow: 0px 0px 20px rgba(255, 255, 0, 1);
        }

        .certificate {
            display: none;
            width: 80%;
            max-width: 600px;
            margin: auto;
            margin-top: 20px;
            border: 10px solid gold;
            padding: 20px;
            background: white;
            color: black;
            box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.3);
            border-radius: 10px;
            opacity: 0;
            transition: opacity 2s ease-in-out;
        }

        .certificate img {
            width: 100%;
            border-radius: 5px;
        }

    </style>
</head>
<body>

    <div class="container">
        <h1>🎊 Tahniah & Surprise Gila Meriah! 🎊</h1>
        <p>Tekan butang ni untuk mainkan lagu & lihat kejutan!</p>
        <button class="btn" onclick="startCelebration()">🎶 Play Lagu & Surprise! 🎶</button>
    </div>

    <div id="certificate" class="certificate">
        <img src="Sijil LI.jpg" alt="Sijil Penghargaan">
    </div>

    <!-- Lagu Latar -->
    <audio id="background-music">
        <source src="NEXT!-Slowed By NCTS.mp3" type="audio/mpeg">
        Browser anda tidak menyokong elemen audio.
    </audio>

    <script>
        function startCelebration() {
            let music = document.getElementById("background-music");
            let certificate = document.getElementById("certificate");
            
            music.play().then(() => {
                certificate.style.display = "block";
                setTimeout(() => {
                    certificate.style.opacity = "1";
                }, 100);
            }).catch(error => {
                alert("Sila tekan play secara manual pada pemain muzik.");
            });
        }
    </script>

</body>
</html>
