<!DOCTYPE html>
<html lang="ta">
<head>
  <meta charset="UTF-8">
  <title>🌸 ஆசிரியர் தின வாழ்த்துகள் 🌸</title>
  <style>
    body {
      margin: 0;
      font-family: "Poppins", sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: linear-gradient(270deg, #ff9a9e, #fad0c4, #fbc2eb, #a6c1ee);
      background-size: 800% 800%;
      animation: gradientBG 20s ease infinite;
      overflow: hidden;
      text-align: center;
    }
    @keyframes gradientBG {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    .card {
      background: rgba(255,255,255,0.9);
      padding: 40px;
      border-radius: 24px;
      box-shadow: 0 12px 40px rgba(0,0,0,0.2);
      max-width: 800px;
      position: relative;
      border: 4px solid gold;
    }
    h1 {
      font-size: 40px;
      color: #d97706;
      text-shadow: 0 0 10px #fcd34d, 0 0 20px #fbbf24;
      animation: glow 2s infinite alternate;
    }
    @keyframes glow {
      from { text-shadow: 0 0 10px #fcd34d, 0 0 20px #fbbf24; }
      to { text-shadow: 0 0 20px #f59e0b, 0 0 40px #fbbf24; }
    }
    p {
      font-size: 22px;
      color: #444;
      margin: 15px 0;
    }
    .music {
      margin-top: 20px;
    }
    iframe {
      border-radius: 12px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.3);
    }
    canvas {
      position: fixed;
      inset: 0;
      pointer-events: none;
    }
  </style>
</head>
<body>
  <canvas id="confetti"></canvas>
  <div class="card">
    <h1>🌟 ஆசிரியர் தின நல்வாழ்த்துக்கள் 🌟</h1>
    <p>எங்கள் வாழ்வில் ஒளி பாயச் செய்த ஆசிரியர்களுக்கு நன்றி 💐</p>
    <div class="music">
      <!-- Tamil song from YouTube (replace link with your favorite) -->
      <iframe width="560" height="315" 
        src="https://youtu.be/VWifDN4yWjo?si=9sYahGXxstoVe8XX" 
        title="Tamil Song" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen>
      </iframe>
    </div>
  </div>

  <script>
    // Confetti
    const canvas = document.getElementById('confetti');
    const ctx = canvas.getContext('2d');
    let confettiBits = [];
    function resize() { canvas.width = innerWidth; canvas.height = innerHeight; }
    window.addEventListener('resize', resize); resize();
    function launchConfetti() {
      confettiBits = Array.from({ length: 300 }, () => ({
        x: Math.random() * canvas.width,
        y: Math.random() * -50,
        r: 4 + Math.random() * 6,
        vy: 2 + Math.random() * 3,
        vx: -2 + Math.random() * 4,
        color: ['#ef4444','#f59e0b','#10b981','#3b82f6','#a855f7','#ec4899'][Math.floor(Math.random()*6)]
      }));
      animate();
      setTimeout(() => confettiBits = [], 7000);
    }
    function animate() {
      if (!confettiBits.length) return;
      ctx.clearRect(0,0,canvas.width,canvas.height);
      for (const p of confettiBits) {
        p.x += p.vx; p.y += p.vy;
        ctx.fillStyle = p.color;
        ctx.fillRect(p.x, p.y, p.r, p.r);
      }
      requestAnimationFrame(animate);
    }
    launchConfetti();
  </script>
</body>
</html>
