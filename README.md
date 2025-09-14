<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Project Name — One Page</title>
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#38bdf8; --muted:#9aa4b2;
      --glass: rgba(255,255,255,0.03);
    }
    *{box-sizing:border-box}
    body{
      margin:0; font-family:Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: linear-gradient(180deg,#071022 0%, #0b1320 100%); color:#e6eef6;
      -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale;
    }
    .wrap{max-width:980px;margin:40px auto;padding:24px}
    header{display:flex;align-items:center;gap:16px;margin-bottom:22px}
    .logo{
      width:64px;height:64px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#7dd3fc);
      display:flex;align-items:center;justify-content:center;font-weight:700;color:#022;box-shadow:0 6px 24px rgba(2,6,23,.6)
    }
    h1{font-size:1.6rem;margin:0}
    p.lead{color:var(--muted);margin:4px 0 0}
    .grid{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:22px}
    .card{background:var(--card);padding:16px;border-radius:12px;box-shadow:0 6px 22px rgba(2,6,23,.6);border:1px solid rgba(255,255,255,0.03)}
    .features li{margin:10px 0}
    .btn{
      display:inline-block;padding:10px 14px;border-radius:10px;background:linear-gradient(90deg,var(--accent),#60a5fa);color:#022;font-weight:700;text-decoration:none;margin-right:8px;
    }
    .muted{color:var(--muted);font-size:0.95rem}
    footer{margin-top:28px;color:var(--muted);font-size:0.9rem;text-align:center}
    pre{background:var(--glass);padding:12px;border-radius:8px;overflow:auto;color:#dff3ff}
    @media (max-width:880px){
      .grid{grid-template-columns:1fr; }
      header{flex-direction:row}
      .logo{width:56px;height:56px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="logo">PN</div>
      <div>
        <h1>Project Name</h1>
        <p class="lead">Short one-line description — what the project does and who it’s for.</p>
      </div>
    </header>

    <div class="grid">
      <section class="card">
        <h2>About</h2>
        <p class="muted">Brief intro about the project. Mention key purpose, tech stack, and quick context so visitors know what this repo contains.</p>

        <h3 style="margin-top:16px">Features</h3>
        <ul class="features">
          <li>✅ Feature 1 — short phrase</li>
          <li>✅ Feature 2 — short phrase</li>
          <li>✅ Feature 3 — short phrase</li>
        </ul>

        <h3 style="margin-top:14px">Quick start</h3>
        <pre>
git clone https://github.com/your-username/your-repo.git
cd your-repo
# follow README for setup
        </pre>

        <div style="margin-top:12px">
          <a class="btn" href="https://github.com/your-username/your-repo" target="_blank" rel="noopener">View on GitHub</a>
          <a class="btn" href="#" style="background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted)">Live Demo</a>
        </div>
      </section>

      <aside class="card">
        <h3>Project Info</h3>
        <p class="muted"><strong>Language:</strong> JavaScript / React (example)</p>
        <p class="muted"><strong>License:</strong> MIT</p>

        <h4 style="margin-top:16px">Contact</h4>
        <p class="muted">your.email@example.com</p>

        <h4 style="margin-top:14px">Contribute</h4>
        <p class="muted">Fork the repo → make changes → open a PR. Check CONTRIBUTING.md (if any).</p>
      </aside>
    </div>

    <footer>
      Made with ❤️ · © <span id="year"></span> Your Name
    </footer>
  </div>

  <script>
    document.getElementById('year').innerText = new Date().getFullYear();
  </script>
</body>
</html>

