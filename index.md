<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>me desculpa?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding-top: 50px;
        }

        #question {
            font-size: 24px;
            margin-bottom: 20px;
        }

        #noButton {
            font-size: 18px;
            padding: 10px 20px;
            cursor: pointer;
            position: absolute;
        }
    </style>
</head>

<body>
    <h1>Me desculpa?</h1>
    <p id="question">Clique no botão abaixo para responder:</p>
    <button id="noButton" onclick="moveButton()">Não</button>

    <script>
        function moveButton() {
            const button = document.getElementById('noButton');
            const maxWidth = window.innerWidth - button.clientWidth;
            const maxHeight = window.innerHeight - button.clientHeight;

            const randomX = Math.floor(Math.random() * maxWidth);
            const randomY = Math.floor(Math.random() * maxHeight);

            button.style.left = randomX + 'px';
            button.style.top = randomY + 'px';
        }
    </script>
</body>

</html>
