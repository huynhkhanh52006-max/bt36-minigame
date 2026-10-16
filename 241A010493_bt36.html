<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bài tập 36 - Mini Game Hứng Táo</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: #f0f8e9;
            margin: 0;
            padding: 25px 10px;
        }

        h1 {
            color: #287442;
        }

        .stats {
            display: flex;
            justify-content: center;
            gap: 35px;
            margin: 20px;
            font-size: 20px;
            font-weight: bold;
        }

        #game-container {
            width: 500px;
            height: 400px;
            max-width: 100%;
            margin: auto;
            position: relative;
            overflow: hidden;
            border: 3px solid #65965b;
            border-radius: 15px;
            background: linear-gradient(#d9f2ff, #f8ffe9);
        }

        #basket {
            width: 85px;
            height: 30px;
            position: absolute;
            bottom: 12px;
            left: 207px;
            background: #a96832;
            border: 4px solid #75451f;
            border-top: 7px solid #d49a58;
            border-radius: 5px 5px 15px 15px;
        }

        #apple {
            position: absolute;
            top: 0;
            left: 100px;
            width: 32px;
            height: 32px;
            font-size: 30px;
            display: none;
        }

        button {
            margin-top: 18px;
            padding: 12px 30px;
            font-size: 18px;
            font-weight: bold;
            color: white;
            background: #258348;
            border: none;
            border-radius: 8px;
            cursor: pointer;
        }

        button:hover {
            background: #176333;
        }

        #message {
            font-size: 20px;
            font-weight: bold;
            color: #c0392b;
            margin-top: 15px;
        }
    </style>
</head>

<body>
    <h1>🍎 MINI GAME HỨNG TÁO 🍎</h1>
    <p>Dùng phím mũi tên trái và phải để hứng táo!</p>

    <div class="stats">
        <div>Điểm: <span id="score">0</span></div>
        <div>Mạng: <span id="lives">3</span> ❤️</div>
    </div>

    <div id="game-container">
        <div id="apple">🍎</div>
        <div id="basket"></div>
    </div>

    <button id="startButton" onclick="startGame()">Bắt đầu</button>
    <div id="message"></div>

    <script>
        const game = document.getElementById("game-container");
        const apple = document.getElementById("apple");
        const basket = document.getElementById("basket");
        const scoreText = document.getElementById("score");
        const livesText = document.getElementById("lives");
        const message = document.getElementById("message");
        const startButton = document.getElementById("startButton");

        let score = 0;
        let lives = 3;
        let basketX = 207;
        let appleX = 100;
        let appleY = 0;
        let speed = 2;
        let running = false;
        let animationId = null;

        // Di chuyển giỏ, không cho ra ngoài khung game.
        function moveBasket() {
            const maxX = game.clientWidth - basket.offsetWidth;

            basketX = Math.max(0, Math.min(basketX, maxX));
            basket.style.left = basketX + "px";
        }

        // Đưa táo về đầu khung tại vị trí ngẫu nhiên.
        function resetApple() {
            const maxX = game.clientWidth - apple.offsetWidth;

            appleX = Math.random() * maxX;
            appleY = 0;

            apple.style.left = appleX + "px";
            apple.style.top = appleY + "px";
        }

        // Bắt đầu hoặc chơi lại game.
        function startGame() {
            if (animationId !== null) {
                cancelAnimationFrame(animationId);
            }

            score = 0;
            lives = 3;
            speed = 2;
            basketX = (game.clientWidth - basket.offsetWidth) / 2;

            scoreText.textContent = score;
            livesText.textContent = lives;
            message.textContent = "";
            startButton.textContent = "Chơi lại";

            apple.style.display = "block";
            running = true;

            moveBasket();
            resetApple();
            gameLoop();
        }

        // Vòng lặp xử lý táo rơi và kiểm tra va chạm.
        function gameLoop() {
            if (!running) return;

            appleY += speed;
            apple.style.top = appleY + "px";

            const appleRight = appleX + apple.offsetWidth;
            const appleBottom = appleY + apple.offsetHeight;
            const basketRight = basketX + basket.offsetWidth;
            const basketTop =
                game.clientHeight - basket.offsetHeight - 12;

            // Kiểm tra táo có chạm vào giỏ hay không.
            const caught =
                appleRight > basketX &&
                appleX < basketRight &&
                appleBottom >= basketTop &&
                appleY < basketTop + basket.offsetHeight;

            if (caught) {
                score++;
                scoreText.textContent = score;

                // Tăng tốc độ rơi sau mỗi lần hứng được táo.
                speed += 0.2;
                resetApple();

            } else if (appleBottom >= game.clientHeight) {
                // Không hứng được táo thì mất một mạng.
                lives--;
                livesText.textContent = lives;

                if (lives <= 0) {
                    running = false;
                    apple.style.display = "none";
                    message.textContent =
                        "Game Over! Điểm của bạn: " + score;
                    startButton.textContent = "Chơi lại";
                    animationId = null;
                    return;
                }

                resetApple();
            }

            animationId = requestAnimationFrame(gameLoop);
        }

        // Điều khiển giỏ bằng phím mũi tên.
        document.addEventListener("keydown", function(event) {
            if (!running) return;

            if (event.key === "ArrowLeft") {
                event.preventDefault();
                basketX -= 25;
                moveBasket();
            }

            if (event.key === "ArrowRight") {
                event.preventDefault();
                basketX += 25;
                moveBasket();
            }
        });

        document.getElementById("startButton")
            .addEventListener("click", startGame);

        window.addEventListener("resize", moveBasket);
    </script>
</body>
</html>
