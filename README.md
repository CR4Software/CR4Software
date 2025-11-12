<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Cameron Rogers — GitHub Portfolio</title>
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#9aa7bf;
      --accent:#06b6d4;
      --glass: rgba(255,255,255,0.04);
      --radius:14px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background:linear-gradient(180deg,var(--bg) 0%, #071023 100%);
      color:#e6eef8;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding:32px;
      display:flex;
      align-items:center;
      justify-content:center;
      font-size:16px;
    }
    .container{
      width:100%;
      max-width:1000px;
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:18px;
      padding:28px;
      box-shadow: 0 8px 30px rgba(2,6,23,0.6);
      border:1px solid rgba(255,255,255,0.03);
    }
    header{
      display:flex;
      gap:18px;
      align-items:center;
    }
    .avatar{
      width:84px;height:84px;border-radius:14px;background:linear-gradient(135deg,var(--accent), #7c3aed);
      display:flex;align-items:center;justify-content:center;font-weight:700;font-size:28px;color:#041027;flex:0 0 84px;
    }
    h1{margin:0;font-size:24px}
    p.lead{margin:6px 0 0;color:var(--muted)}

    .grid{
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:20px;
      margin-top:20px;
    }
    .card{background:var(--card);padding:18px;border-radius:12px;border:1px solid var(--glass)}

    /* Skills */
    .skills{display:grid;gap:12px}
    .skill{display:flex;flex-direction:column;gap:6px}
    .skill .meta{display:flex;justify-content:space-between;font-size:13px;color:var(--muted)}
    .bar{height:10px;background:rgba(255,255,255,0.06);border-radius:999px;overflow:hidden}
    .bar > i{display:block;height:100%;background:linear-gradient(90deg,var(--accent), #7c3aed);border-radius:999px}

    /* Projects */
    .projects{display:flex;flex-direction:column;gap:12px}
    .project{padding:12px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.01), transparent);border:1px solid rgba(255,255,255,0.02)}
    .project h4{margin:0 0 6px}
    .project p{margin:0;color:var(--muted);font-size:14px}
    .links{margin-top:12px;display:flex;gap:8px}
    .btn{padding:8px 12px;border-radius:8px;background:transparent;border:1px solid rgba(255,255,255,0.06);font-weight:600;font-size:14px;color:var(--accent);text-decoration:none}

    /* Sidebar */
    .bio{line-height:1.5;color:var(--muted)}
    .contact{margin-top:12px;display:flex;flex-direction:column;gap:8px}
    .chip{display:inline-block;padding:6px 10px;border-radius:999px;background:rgba(255,255,255,0.02);border:1px solid rgba(255,255,255,0.02);font-size:13px}

    footer{margin-top:18px;color:var(--muted);font-size:13px;text-align:center}

    @media (max-width:880px){
      .grid{grid-template-columns:1fr;}
      body{padding:18px}
    }
  </style>
</head>
<body>
  <main class="container" role="main">
    <header>
      <div class="avatar">CR</div>
      <div>
        <h1>Cameron Rogers — Information Technology & New Grad</h1>
        <p class="lead">Graduating Spring 2025 from Middle Georgia State University • Passionate about IT support, systems administration, and software tools for automation</p>
      </div>
    </header>

    <div class="grid">
      <section>
        <div class="card">
          <h3>About me</h3>
          <p class="bio">Hello — I’m Cameron, an Information Technology graduate (Spring 2025) with hands-on experience in troubleshooting, endpoint support, scripting, and small-scale automation projects. I enjoy bridging hardware and software — Raspberry Pi projects, basic networking, and web-based tooling are some of my go-to areas.</p>
        </div>

        <div class="card" style="margin-top:14px">
          <h3>Skills</h3>
          <div class="skills" style="margin-top:12px">
            <div class="skill">
              <div class="meta"><span>IT Support & Systems</span><span>85%</span></div>
              <div class="bar"><i style="width:85%"></i></div>
            </div>

            <div class="skill">
              <div class="meta"><span>Networking (TCP/IP, DHCP, Wi‑Fi)</span><span>78%</span></div>
              <div class="bar"><i style="width:78%"></i></div>
            </div>

            <div class="skill">
              <div class="meta"><span>Programming (Python, Java)</span><span>74%</span></div>
              <div class="bar"><i style="width:74%"></i></div>
            </div>

            <div class="skill">
              <div class="meta"><span>Web (HTML, CSS, JavaScript)</span><span>70%</span></div>
              <div class="bar"><i style="width:70%"></i></div>
            </div>

            <div class="skill">
              <div class="meta"><span>Tools: Git, Linux, VSCode</span><span>80%</span></div>
              <div class="bar"><i style="width:80%"></i></div>
            </div>
          </div>
        </div>

        <div class="card" style="margin-top:14px">
          <h3>Selected projects</h3>
          <div class="projects">
            <article class="project">
              <h4>Raspberry Pi LED Controller</h4>
              <p>GPIO-driven LED controller with Python scripts and web UI hosted on the Pi. Demonstrates hardware interfacing and basic automation.</p>
              <div class="links">
                <a class="btn" href="#">View Repo</a>
                <a class="btn" href="#">Live Demo</a>
              </div>
            </article>

            <article class="project">
              <h4>IT Support Ticketing Scripts</h4>
              <p>Small collection of scripts to parse and summarize support tickets (CSV → summary), built with Python and pandas.</p>
              <div class="links">
                <a class="btn" href="#">View Repo</a>
              </div>
            </article>

            <article class="project">
              <h4>Personal Website / Resume</h4>
              <p>A single-page portfolio and downloadable resume designed to present skills clearly to recruiters and hiring managers.</p>
              <div class="links">
                <a class="btn" href="#">View Site</a>
              </div>
            </article>

          </div>
        </div>

      </section>

      <aside>
        <div class="card">
          <h3>Contact</h3>
          <div class="contact">
            <div><strong>Email</strong><div class="chip">cameron.rogers@example.com</div></div>
            <div><strong>Location</strong><div class="chip">Warner Robins, GA / Georgia</div></div>
            <div><strong>GitHub</strong><div class="chip">github.com/cameron-rogers</div></div>
            <div><strong>LinkedIn</strong><div class="chip">linkedin.com/in/cameron-rogers</div></div>
          </div>
        </div>

        <div class="card" style="margin-top:14px">
          <h3>Quick facts</h3>
          <ul style="margin:8px 0 0 18px; color:var(--muted)">
            <li>Middle Georgia State University — Information Technology (Class of 2025)</li>
            <li>Familiar: Windows, Linux, basic server tasks</li>
            <li>Tools: Git, VSCode, Raspberry Pi, Sense HAT</li>
          </ul>
        </div>

        <div class="card" style="margin-top:14px;text-align:center">
          <h3>Resume</h3>
          <p style="color:var(--muted);margin:6px 0 10px">Download the PDF resume or link it from your GitHub repo.</p>
          <a class="btn" href="#">Download Resume</a>
        </div>
      </aside>
    </div>

    <footer>
      Built with HTML & CSS • Want this tuned for GitHub README.md (Markdown) or a GitHub Pages site? I can convert it for you.
    </footer>
  </main>
</body>
</html>
