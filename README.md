[Uploading ыы.html…]()<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Сайт со звуками</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
            overflow: hidden;
            background-color: black;
        }
        #image {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 100vw;
            height: 100vh;
            object-fit: cover;
            animation: shake 0.1s infinite; /* Анимация дергания */
        }

        @keyframes shake {
            0% { transform: translate(-50%, -50%) translateX(0); }
            25% { transform: translate(-50%, -50%) translateX(-10px); }
            50% { transform: translate(-50%, -50%) translateX(10px); }
            75% { transform: translate(-50%, -50%) translateX(-10px); }
            100% { transform: translate(-500%, -500%) translateX(0); }
        }
    </style>
</head>
<body>
    <img id="image" src="https://fotoslava.ru/wp-content/uploads/litso-putina-1.webp" alt="Изображение" />
    <audio id="audio" autoplay loop>
        <source src="URL_ВАШЕГО_АУДИО_ФАЙЛА" type="audio/mpeg">
        Ваш браузер не поддерживает аудио.
    </audio>
    <script>
        window.onload = function() {
            const audio = document.getElementById('audio');
            audio.volume = 1.0; // Установите громкость на максимум
        };
    </script>
</body>
</html>

