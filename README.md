<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Venda de Contas Blox Fruits</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: url('https://blogger.googleusercontent.com/img/a/AVvXsEi8bUdh_QuEV3gd_nomQ2Z7fYH8jeklX0cR8UYmRnZtsSrcfZHXwrE66ekzlrPlPOhjL2wbOWatNNi7XL0HW0HAtfalqQleST9thJSM6EpPecmXZpC1-FpuFqQubO73lZKhpRcyj2i7My6t6goQ6D6DZLW4OzhDBPzy2TNuvuMfk3G-mvpnCPVlBUxbM5GX=w1600') no-repeat center center fixed;
            background-size: cover;
            color: white;
        }
        .container {
            padding: 20px;
            text-align: center;
        }
        .produto {
            background: rgba(0, 0, 0, 0.7);
            padding: 20px;
            margin: 20px auto;
            border-radius: 10px;
            max-width: 400px;
            text-align: center;
        }
        .produto img {
            width: 100%;
            border-radius: 10px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            margin-top: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #45a049;
        }
        /* Modal styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
        }
        .modal-content {
            background: white;
            color: black;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            max-width: 400px;
        }
        .modal-content h3 {
            margin-top: 0;
        }
        .close {
            background-color: #d9534f;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            margin-top: 20px;
        }
        .close:hover {
            background-color: #c9302c;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Contas Blox Fruits</h1>
        <p>Escolha a conta ideal para você!</p>

        <!-- Produto 1 -->
        <div class="produto">
            <h3>Nível 1000 - R$ 15,00</h3>
            <p>Conta para o 1º mar</p>
            <img src="https://cdn.dfg.com.br/itemimages/993100068-contas-blox-fruits-godhuman-cdk-sg-melhor-preco-MXQ9.webp" alt="Conta Nível 1000">
            <button onclick="comprar(1000, 15)">Comprar</button>
        </div>

        <!-- Produto 2 -->
        <div class="produto">
            <h3>Nível 2000 - R$ 20,00</h3>
            <p>Conta para o 2º mar</p>
            <img src="https://cdn.dfg.com.br/itemimages/993100068-contas-blox-fruits-godhuman-cdk-sg-melhor-preco-MXQ9.webp" alt="Conta Nível 2000">
            <button onclick="comprar(2000, 20)">Comprar</button>
        </div>

        <!-- Produto 3 -->
        <div class="produto">
            <h3>Nível Máximo - R$ 30,00</h3>
            <p>Conta completa</p>
            <img src="https://cdn.dfg.com.br/itemimages/993100068-contas-blox-fruits-godhuman-cdk-sg-melhor-preco-MXQ9.webp" alt="Conta Nível Máximo">
            <button onclick="comprar('máximo', 30)">Comprar</button>
        </div>
    </div>

    <!-- Modal -->
    <div id="modal" class="modal">
        <div class="modal-content">
            <h3>Compra de Conta</h3>
            <p id="modal-text"></p>
            <a id="discord-link" href="https://discord.gg/xuAFazcm" target="_blank">
                <button class="close">Ir para o Discord</button>
            </a>
        </div>
    </div>

    <script>
        function comprar(nivel, preco) {
            const mensagem = `Você escolheu a conta de nível ${nivel} pelo preço de R$ ${preco},00.\n\n` +
                `1. Envie o pagamento via PIX para o email: kalel.ferreira.cruz712@gmail.com\n` +
                `2. Clique no botão abaixo para entrar no servidor do Discord.\n` +
                `3. Abra um ticket e envie o comprovante de pagamento!\n\n` +
                `Após a confirmação, a conta será liberada para você.`;
            document.getElementById("modal-text").innerText = mensagem;
            document.getElementById("modal").style.display = "flex";
        }

        function fecharModal() {
            document.getElementById("modal").style.display = "none";
        }
    </script>
</body>
</html>
