<!-- templates/trade.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mytra-FX | Trade</title>
    <link rel="stylesheet" href="/static/style.css">
</head>
<body>
    <div class="container">
        <h2 id="symbol-name"></h2>

        <div class="trade-panel">
            <input type="number" id="quantity" placeholder="Miktar" min="0" step="0.01">
            <button onclick="placeOrder('BUY')" class="btn buy">Buy</button>
            <button onclick="placeOrder('SELL')" class="btn sell">Sell</button>
        </div>

        <div id="result"></div>
    </div>

    <script>
        const pathParts = window.location.pathname.split("/");
        const symbol = decodeURIComponent(pathParts[pathParts.length - 1]);
        const userId = localStorage.getItem("user_id"); // giriş sonrası localStorage'da tutulmalı

        document.getElementById("symbol-name").innerText = `Parite: ${symbol}`;

        function placeOrder(side) {
            const quantity = parseFloat(document.getElementById("quantity").value);
            if (!quantity || quantity <= 0) {
                alert("Geçerli bir miktar girin.");
                return;
            }

            fetch("/api/trade/place_order", {
                method: "POST",
                headers: { "Content-Type": "application/json" },
                body: JSON.stringify({
                    user_id: userId,
                    symbol: symbol,
                    quantity: quantity,
                    side: side,
                    order_type: "MARKET"
                })
            })
            .then(res => res.json())
            .then(data => {
                document.getElementById("result").innerText = data.message;
            })
            .catch(err => {
                console.error(err);
                document.getElementById("result").innerText = "İşlem başarısız.";
            });
        }
    </script>
</body>
</html>
