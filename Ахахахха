<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NFS Loading...</title>
  <style>
    body {
      margin: 0;
      overflow: hidden;
      background: black;
      color: white;
      font-family: 'Arial Black', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      position: relative;
    }
    .fake-loading {
      font-size: 2rem;
      animation: pulse 1s infinite;
    }
    @keyframes pulse {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.5; }
    }
    .screamer {
      position: absolute;
      top: 50%;
      left: -100%;
      transform: translateY(-50%);
      transition: left 0.5s ease-in-out;
      z-index: 10;
    }
    .screamer.show {
      left: 50%;
      transform: translate(-50%, -50%) scale(1.5);
    }
  </style>
</head>
<body>
  <div class="fake-loading">Loading Need for Speed...</div>
  <img src="https://i.imgur.com/rxD9GmY.png" alt="Car Screamer" class="screamer" id="car" />
  <audio id="sfx">
    <source src="https://www.soundjay.com/transportation/car-skid-crash-1.mp3" type="audio/mpeg">
  </audio>
  <script>
    setTimeout(() => {
      document.getElementById('car').classList.add('show');
      document.getElementById('sfx').play();
      if (navigator.vibrate) {
        navigator.vibrate([200, 100, 200, 100, 300]);
      }
    }, 3000);
  </script>
</body>
</html>
