<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Cameron Rogers | Developer Arc</title>

  <!-- Security Headers (Netlify compatible) -->
  <meta http-equiv="Content-Security-Policy"
    content="default-src 'self'; img-src 'self' data:; style-src 'self' 'unsafe-inline'; script-src 'self';">

  <link rel="stylesheet" href="styles.css" />
</head>

<body>
  <!-- Hero -->
  <section class="hero">
    <h1>Cameron Rogers</h1>
    <p>Software Developer · IT Graduate · Builder</p>

    <div class="actions">
      <button onclick="startJourney()">Start Journey</button>
      <a href="resume.pdf" target="_blank">View Resume</a>
    </div>
  </section>

  <!-- Stats -->
  <section class="stats">
    <h2>Character Stats</h2>

    <div class="stat">
      <span>Problem Solving</span>
      <div class="bar"><div data-level="80"></div></div>
    </div>

    <div class="stat">
      <span>Backend Logic</span>
      <div class="bar"><div data-level="75"></div></div>
    </div>
  </section>

  <!-- Projects -->
  <section class="projects">
    <h2>Battle Records</h2>

    <div class="card">
      <h3>Autonomous Rover</h3>
      <p>Python · Sensors · Raspberry Pi</p>
      <p>Built a rover that navigates obstacles autonomously.</p>
    </div>
  </section>

  <footer>© 2025 Cameron Rogers</footer>

  <script src="app.js"></script>
</body>
</html>

