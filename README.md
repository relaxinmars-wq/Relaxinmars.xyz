To create website 
What should I do next on GitHub 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Relax in Mars (RLXMR)</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500&family=Roboto&display=swap" rel="stylesheet">
  <style>
    /* Reset and base styles */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Roboto', sans-serif; }
    body { background: #0D0D0D; color: #fff; overflow-x: hidden; }
    a { color: inherit; text-decoration: none; }

    /* Header / Hero */
    header {
      height: 100vh;
      background: radial-gradient(circle at top, #1a0000, #0D0D0D);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      position: relative;
      overflow: hidden;
    }
    header h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: 4rem;
      color: #FF4500;
      text-shadow: 0 0 20px #FF4500, 0 0 40px #FF7F50;
    }
    header p {
      margin-top: 20px;
      font-size: 1.5rem;
      color: #FFA07A;
    }
    /* Mars background animation */
    .mars-bg {
      position: absolute;
      top: -50px;
      left: -50px;
      width: 150%;
      height: 150%;
      background: url('https://i.imgur.com/fG4hS3r.png') no-repeat center center / contain;
      animation: rotateMars 60s linear infinite;
      opacity: 0.2;
      z-index: 0;
    }
    @keyframes rotateMars {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    /* Sections */
    section { padding: 80px 20px; max-width: 1200px; margin: 0 auto; }
    h2 { font-family: 'Orbitron', sans-serif; color: #FF4500; text-align: center; margin-bottom: 40px; font-size: 2.5rem; }
    .cards { display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; }
    .card {
      background: #1a0a0a;
      border: 1px solid #FF4500;
      border-radius: 15px;
      padding: 20px;
      width: 250px;
      text-align: center;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 0 20px #FF4500;
    }

    /* Footer */
    footer {
      background: #0D0D0D;
      text-align: center;
      padding: 40px 20px;
      border-top: 1px solid #FF4500;
      font-size: 0.9rem;
      color: #FFA07A;
    }

    /* Floating space particles */
    .particle {
      position: absolute;
      width: 2px;
      height: 2px;
      background: #00FFFF;
      border-radius: 50%;
      opacity: 0.6;
      animation: floatParticle linear infinite;
    }
    @keyframes floatParticle {
      0% { transform: translateY(0px); opacity: 0.6; }
      50% { opacity: 1; }
      100% { transform: translateY(-800px); opacity: 0; }
    }
  </style>
</head>
<body>

  <header>
    <div class="mars-bg"></div>
    <h1>RLXMR</h1>
    <p>Take it easy. Relax… on Mars.</p>
  </header>

  <section id="about">
    <h2>About RLXMR</h2>
    <p style="text-align:center; max-width:700px; margin: 0 auto;">
      RLXMR is a fun crypto coin for space dreamers, Mars enthusiasts, and anyone who loves to chill. Explore Mars, enjoy the content, and relax—it’s all about fun here!
    </p>
  </section>

  <section id="mars-facts">
    <h2>Mars Fun Facts</h2>
    <div class="cards">
      <div class="card">
        <h3>Olympus Mons</h3>
        <p>Tallest volcano in the solar system at 22 km high.</p>
      </div>
      <div class="card">
        <h3>Red Planet</h3>
        <p>Mars gets its color from iron oxide (rust) on its surface.</p>
      </div>
      <div class="card">
        <h3>Thin Atmosphere</h3>
        <p>95% of Mars’ atmosphere is carbon dioxide.</p>
      </div>
      <div class="card">
        <h3>Martian Day</h3>
        <p>A day on Mars lasts 24 hours and 39 minutes.</p>
      </div>
    </div>
  </section>

  <section id="community">
    <h2>Community & Fun</h2>
    <p style="text-align:center; max-width:700px; margin: 0 auto;">
      Share your Mars memes, fan art, and creative posts. Relax and enjoy the Martian vibe!
    </p>
  </section>

  <footer>
    For fun only. Chill, enjoy Mars, and relax. <br>
    RLXMR © 2025
  </footer>

  <script>
    // Create floating space particles
    for(let i=0;i<100;i++){
      let particle = document.createElement('div');
      particle.className = 'particle';
      particle.style.left = Math.random() * window.innerWidth + 'px';
      particle.style.top = Math.random() * window.innerHeight + 'px';
      particle.style.animationDuration = (5 + Math.random() * 10) + 's';
      document.body.appendChild(particle);
    }
  </script>

</body>
</html>
