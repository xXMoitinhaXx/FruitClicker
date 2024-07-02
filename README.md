# FruitClicker
Choose a fruit and click on it, each click accumulates points

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>
    <button id="clickButton">Click</button>
    <p>Clique no botão: <span id="clickCount">0</span> vezes</p>

    <script>
        // Obtém referências ao botão e ao elemento de contagem
        const button = document.getElementById('clickButton');
        const countDisplay = document.getElementById('clickCount');

        // Inicializa a contagem de cliques
        let clickCount = 0;

        // Adiciona um evento de clique ao botão
        button.addEventListener('click', () => {
            // Incrementa a contagem de cliques
            clickCount++;

            // Atualiza a exibição da contagem
            countDisplay.textContent = clickCount;
        });
    </script>
</body>
</html>
