<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online Gameplay</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #1a1a2e;
            color: white;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        header {
            background: #16213e;
            padding: 20px;
            font-size: 24px;
        }
        nav {
            margin: 20px;
        }
        nav a {
            text-decoration: none;
            color: #e94560;
            margin: 0 15px;
            font-size: 20px;
        }
        .game-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            padding: 20px;
        }
        .game-card {
            background: #0f3460;
            margin: 15px;
            padding: 15px;
            border-radius: 10px;
            width: 250px;
            text-align: center;
        }
        .game-card img {
            width: 100%;
            border-radius: 5px;
        }
        .play-btn {
            display: inline-block;
            margin-top: 10px;
            padding: 10px 20px;
            background: #e94560;
            color: white;
            text-decoration: none;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <header>Online Gameplay</header>
    <nav>
        <a href="#">Home</a>
        <a href="#">Games</a>
        <a href="#">Leaderboard</a>
        <a href="#">Contact</a>
    </nav>
    <div class="game-container">
        <div class="game-card">
            <img src="game1.jpg" alt="Game 1">
            <h3>Game Title 1</h3>
            <a href="#" class="play-btn">Play Now</a>
        </div>
        <div class="game-card">
            <img src="game2.jpg" alt="Game 2">
            <h3>Game Title 2</h3>
            <a href="#" class="play-btn">Play Now</a>
        </div>
        <div class="game-card">
            <img src="game3.jpg" alt="Game 3">
            <h3>Game Title 3</h3>
            <a href="#" class="play-btn">Play Now</a>
        </div>
    </div>
</body>
</html>



