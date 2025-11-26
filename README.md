<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FrogoBlitz ⚡ $FROGO</title>
  <meta name="description" content="The fastest frog on Solana. One leap. One moon.">
  
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@700;900&family=Rajdhani:wght@500;700&display=swap" rel="stylesheet">
  
  <style>
    :root {
      --neon: #39ff14;
      --dark: #0a0a0a;
      --glass: rgba(20, 20, 20, 0.7);
    }
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      background: #000;
      color: #fff;
      font-family: 'Rajdhani', sans-serif;
      overflow-x: hidden;
      background: linear-gradient(135deg, #000 0%, #001a0d 100%);
    }

    /* Header */
    header {
      position: fixed;
      top: 0;
      width: 100%;
      background: rgba(0,0,0,0.8);
      backdrop-filter: blur(15px);
      padding: 20px 0;
      z-index: 1000;
      border-bottom: 1px solid rgba(57,255,20,0.3);
    }
    nav {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 0 30px;
    }
    .logo {
      font-family: 'Orbitron', sans-serif;
      font-size: 2.2rem;
      background: linear-gradient(90deg, var(--neon), #00ffff);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
    nav ul {
      display: flex;
      list-style: none;
      gap: 30px;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: 700;
      font-size: 1.1rem;
      transition: 0.3s;
      position: relative;
    }
    nav a:hover {
      color: var(--neon);
    }
    nav a::after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      bottom: -6px;
      left: 0;
      background: var(--neon);
      transition: 0.4s;
    }
    nav a:hover::after { width: 100%; }

    /* Hero */
    .hero {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 0 20px;
      position: relative;
    }
    .hero h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: 9rem;
      font-weight: 900;
      background: linear-gradient(45deg, var(--neon), #00ffff, var(--neon));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-size: 200%;
      animation: glow 6s infinite;
      margin-bottom: 20px;
    }
    .hero p {
      font-size: 1.8rem;
      max-width: 800px;
      margin: 20px 0;
      opacity: 0.9;
      line-height: 1.6;
    }
    .btn {
      padding: 18px 50px;
      margin: 15px;
      font-size: 1.4rem;
      font-weight: bold;
      border-radius: 50px;
      text-decoration: none;
      display: inline-block;
      transition: all 0.4s;
    }
    .btn-primary {
      background: var(--neon);
      color: #000;
      box-shadow: 0 0 40px rgba(57,255,20,0.7);
    }
    .btn-primary:hover {
      transform: translateY(-8px) scale(1.05);
      background: #00ff9d;
    }
    .btn-outline {
      border: 3px solid var(--neon);
      color: var(--neon);
    }
    .btn-outline:hover {
      background: var(--neon);
      color: #000;
    }

    /* Features */
    .features {
      padding: 100px 20px;
      max-width: 1200px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 40px;
    }
    .card {
      background: var(--glass);
      backdrop-filter: blur(15px);
      border: 1px solid rgba(57,255,20,0.3);
      border-radius: 20px;
      padding: 40px 30px;
      text-align: center;
      transition: all 0.4s;
      box-shadow: 0 10px 30px rgba(0,0,0,0.5);
    }
    .card:hover {
      transform: translateY(-15px);
      border-color: var(--neon);
      box-shadow: 0 20px 50px rgba(57,255,20,0.3);
    }
    .card h3 {
      font-size: 1.8rem;
      margin-bottom: 15px;
      color: var(--neon);
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 50px 20px;
      background: #000;
      color: #666;
      font-size: 0.9rem;
    }

    /* Animations */
    @keyframes glow {
      0%, 100% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
    }

    @media (max-width: 768px) {
      .hero h1 { font-size: 5rem; }
      .hero p { font-size: 1.3rem; }
      nav ul { gap: 15px; }
      nav a { font-size: 1rem; }
    }
  </style>
</head>
<body>

  <header>
    <nav>
      <div class="logo">FROGOBLITZ</div>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Tokenomics</a></li>
        <li><a href="#">Roadmap</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <h1>FROGOBLITZ</h1>
    <p>The fastest frog on Solana. One leap to the moon. Powered by community, fueled by speed.</p>
    <div style="margin-top: 40px;">
      <a href="https://jup.ag/swap?in=SOL&out=YOUR_CA" class="btn btn-primary">BUY $FROGO</a>
      <a href="https://t.me/frogoblitz" class="btn btn-outline">JOIN TELEGRAM</a>
    </div>
  </section>

  <section class="features">
    <div class="card">
      <h3>Lightning Fast</h3>
      <p>Built on Solana — the fastest blockchain. Transactions in milliseconds, near-zero fees.</p>
    </div>
    <div class="card">
      <h3>Community Owned</h3>
      <p>100% fair launch. No presale. No team tokens. Just pure community power.</p>
    </div>
    <div class="card">
      <h3>Moon Ready</h3>
      <p>Strong holders, viral memes, and unstoppable momentum. This frog jumps high.</p>
    </div>
  </section>

  <footer>
    © 2025 FrogoBlitz • Community Driven • DYOR • Not Financial Advice
  </footer>

</body>
</html>