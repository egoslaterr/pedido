<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Convite Especial</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            text-align: center;
            background-image: url('imagem.jpeg.jpeg'); /* Certifique-se de que o caminho está correto */
            background-size: cover; /* Faz a imagem cobrir todo o fundo */
            background-position: center; /* Centraliza a imagem de fundo */
            background-repeat: no-repeat; /* Impede que a imagem se repita */
        }

        h1 {
            color: #000000;
            font-size: 2rem; /* Ajuste o tamanho da fonte para dispositivos móveis */
            margin: 0.5rem;
        }![imagem jpeg](https://github.com/user-attachments/assets/c4ae419a-7823-4bd6-8f19-85690a2f0b33)


        p {
            font-size: 1.2rem; /* Ajuste o tamanho da fonte para dispositivos móveis */
            color: #000000;
            margin: 1rem 0;
        }

        .buttons {
            display: flex; /* Usa flexbox para centralizar os botões */
            flex-direction: column; /* Empilha os botões verticalmente */
            align-items: center; /* Centraliza os botões horizontalmente */
            gap: 10px; /* Espaçamento entre os botões */
            margin-top: 20px;
        }

        .button {
            display: inline-block;
            padding: 10px 20px;
            font-size: 16px;
            color: #fff;
            background-color: #28a745;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .button:hover {
            background-color: #218838;
        }

        #noButton {
            background-color: #dc3545;
            cursor: pointer;
        }

        #noButton:hover {
            background-color: #c82333;
        }

        @media (max-width: 600px) {
            h1 {
                font-size: 1.5rem; /* Reduz o tamanho do título em telas pequenas */
            }

            p {
                font-size: 1rem; /* Reduz o tamanho do texto em telas pequenas */
            }

            .button {
                font-size: 14px; /* Reduz o tamanho da fonte dos botões em telas pequenas */
                padding: 8px 16px; /* Ajusta o padding dos botões em telas pequenas */
            }
        }

        audio {
            display: none; /* Esconde o player de áudio */
        }
    </style>
</head>
<body>
    <h1>Date surpresa com o mômô</h1>
    <p>Gostaria de ir em um date surpresa no final da tarde de sábado?</p>
    <div class="buttons">
        <a href="#" class="button" onclick="mostrarMensagem()">Sim, claro!</a>
        <button id="noButton" class="button" onclick="fugir()">Não, obrigada</button>
    </div>

    <!-- Player de Áudio -->
    <audio autoplay loop>
        <source src="udio.mp3.mp3" type="audio/mpeg"> <!-- Certifique-se de que o caminho está correto -->
        Seu navegador não suporta o elemento de áudio.
    </audio>

    <script>
        function fugir() {
            var noButton = document.getElementById('noButton');
            var x = Math.random() * (window.innerWidth - noButton.clientWidth);
            var y = Math.random() * (window.innerHeight - noButton.clientHeight);
            noButton.style.position = 'absolute'; /* Necessário para mover o botão */
            noButton.style.left = x + 'px';
            noButton.style.top = y + 'px';
        }

        function mostrarMensagem() {
            alert('É algo simples mas espero que se divirta no dia!');
        }
    </script>
</body>
</html>
