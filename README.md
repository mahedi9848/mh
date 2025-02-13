<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gaming Website</title>
    <style>
        body { text-align: center; font-family: Arial, sans-serif; background: #222; color: white; }
        h1 { margin-top: 20px; }
        .game-container { margin: 20px auto; width: 80%; max-width: 600px; }
        iframe { width: 100%; height: 500px; border: none; }
        button { background: #28a745; color: white; padding: 10px 20px; border: none; cursor: pointer; margin-top: 10px; }
        button:hover { background: #218838; }
    </style>
    <script>
        function loadGame(url) {
            document.getElementById("gameFrame").src = url;
        }
    </script>
</head>
<body>
    <h1>Welcome to My Gaming Website</h1>
    <div class="game-container">
        <p>Choose a game:</p>
        <button onclick="loadGame('https://games.cdn.famobi.com/html5games/l/ludo-classic/v040/?fg_domain=play.famobi.com')">Play Ludo</button>
        <button onclick="loadGame('https://games.cdn.famobi.com/html5games/c/chess-classic/v120/?fg_domain=play.famobi.com')">Play Chess</button>
        <iframe id="gameFrame" src="https://games.cdn.famobi.com/html5games/l/ludo-classic/v040/?fg_domain=play.famobi.com" allowfullscreen></iframe>
    </div>
</body>
</html>
