<!DOCTYPE html>
<html lang="pl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" />
<title>Prosta Gra na Telefon</title>
<style>
  :root {
    --accent-color: #ff6f61;
    --background-color: #1e1e2f;
    --circle-color: #ffb86c;
    --text-color: #f8f8f2;
    --font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }
  html, body {
    margin: 0; padding: 0;
    height: 100%;
    background: var(--background-color);
    color: var(--text-color);
    font-family: var(--font-family);
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    user-select: none;
  }
  header {
    text-align: center;
    padding: 1rem;
  }
  header h1 {
    margin: 0;
    font-weight: 700;
    font-size: 1.8rem;
    color: var(--accent-color);
    text-shadow: 0 0 12px var(--accent-color);
  }
  main {
    flex: 1;
    width: 100%;
    max-width: 480px;
    position: relative;
    overflow: hidden;
    background: #2c2c44;
    border-radius: 1rem;
    margin: 1rem 0;
  }
  #gameArea {
    width: 100%;
    height: 400px;
    touch-action: manipulation;
    position: relative;
  }
  #circle {
    width: 80px;
    height: 80px;
    background: var(--circle-color);
    border-radius: 50%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    box-shadow: 0 0 12px var(--circle-color);
    transition: top 0.3s ease, left 0.3s ease;
    cursor: pointer;
  }
  footer {
    width: 100%;
    max-width: 480px;
    padding: 1rem;
    text-align: center;
    font-size: 1.2rem;
  }
  #score {
    font-weight: 700;
    color: var(--accent-color);
  }
  #timer {
    font-weight: 700;
    color: var(--accent-color);
  }
  button {
    cursor: pointer;
    background: var(--accent-color);
    border: none;
    padding: 0.6rem 1.2rem;
    border-radius: 0.5rem;
    font-size: 1rem;
    color: var(--text-color);
    box-shadow: 0 0 15px var(--accent-color);
    transition: background-color 0.3s ease;
  }
  button:hover, button:focus {
    background: #ff856f;
  }
</style>
</head>
<body>
<header>
  <h1>Dotknij Kółka!</h1>
  <p>Dotknij kółko tak szybko, jak potrafisz! Czas: <span id="timer">30</span>s | Wynik: <span id="score">0</span></p>
</header>
<main>
  <div id="gameArea" aria-label="Obszar gry" role="main">
    <div id="circle" tabindex="0" aria-label="Cel do dotknięcia"></div>
  </div>
</main>
<footer>
  <button id="startBtn" aria-label="Rozpocznij nową grę">Rozpocznij nową grę</button>
</footer>

<script>
  (function() {
    const circle = document.getElementById('circle');
    const gameArea = document.getElementById('gameArea');
    const timerElem = document.getElementById('timer');
    const scoreElem = document.getElementById('score');
    const startBtn = document.getElementById('startBtn');

    let score = 0;
    let timeLeft = 30;
    let timerId = null;
    let gameActive = false;

    function getRandomPosition() {
      const padding = 100; // to keep circle visible fully inside
      const maxX = gameArea.clientWidth - circle.clientWidth - padding;
      const maxY = gameArea.clientHeight - circle.clientHeight - padding;
      const x = Math.floor(Math.random() * maxX) + padding / 2;
      const y = Math.floor(Math.random() * maxY) + padding / 2;
      return {x, y};
    }

    function moveCircle() {
      const {x, y} = getRandomPosition();
      circle.style.left = x + 'px';
      circle.style.top = y + 'px';
    }

    function updateTimer() {
      timeLeft--;
      timerElem.textContent = timeLeft;
      if (timeLeft <= 0) {
        endGame();
      }
    }

    function endGame() {
      clearInterval(timerId);
      gameActive = false;
      circle.style.display = 'none';
      startBtn.disabled = false;
      alert('Koniec gry! Twój wynik to: ' + score);
    }

    function startGame() {
      score = 0;
      timeLeft = 30;
      scoreElem.textContent = score;
      timerElem.textContent = timeLeft;
      gameActive = true;
      circle.style.display = 'block';
      moveCircle();
      startBtn.disabled = true;
      timerId = setInterval(updateTimer, 1000);
    }

    circle.addEventListener('click', () => {
      if (!gameActive) return;
      score++;
      scoreElem.textContent = score;
      moveCircle();
    });

    // Keyboard accessibility: Allow Enter key to "click" circle
    circle.addEventListener('keydown', (e) => {
      if (e.key === 'Enter' || e.key === ' ') {
        e.preventDefault();
        circle.click();
      }
    });

    startBtn.addEventListener('click', startGame);

    // Initial state
    circle.style.display = 'none';
  })();
</script>
</body>
</html>

