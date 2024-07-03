<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pedido de perdón a Natally</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 50px;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      margin: 10px;
    }
  </style>
</head>
<body>
  <h2>¿Me perdonas, Natally?</h2>
  <button id="siButton" onclick="agradecer()">Sí</button>
  <button id="noButton" onclick="denegar()">No</button>

  <p id="mensaje"></p>

  <script>
    function denegar() {
      document.getElementById('noButton').disabled = true;
      document.getElementById('siButton').disabled = false;
      document.getElementById('mensaje').innerText = "No pasa nada, te entiendo.";
    }

    function agradecer() {
      document.getElementById('siButton').disabled = true;
      document.getElementById('noButton').disabled = true;
      document.getElementById('mensaje').innerText = "¡Gracias! Te amo mucho 💖";
    }
  </script>
</body>
</html>
