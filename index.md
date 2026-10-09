<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Andrés | My Journey</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #f4f5fc;
      --card: #ffffff;
      --text: #111111;
      --muted: #777777;
      --accent: #ef5350;
      --accent2: #5c6bf0;
    }
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      background: var(--bg);
      font-family: 'Open Sans', sans-serif;
      color: var(--text);
      line-height: 1.7;
      padding: 40px 16px;
    }
    .container { max-width: 900px; margin: 0 auto; }
    .card {
      background: var(--card);
      border-radius: 16px;
      padding: 40px;
      margin-bottom: 30px;
      box-shadow: 0 4px 24px rgba(92, 107, 240, 0.08);
    }
    h2 {
      font-family: 'Poppins', sans-serif;
      font-size: 1.4rem;
      font-weight: 700;
      margin-bottom: 30px;
      position: relative;
      padding-bottom: 12px;
    }
    h2::after {
      content: "";
      position: absolute;
      left: 0; bottom: 0;
      width: 28px; height: 3px;
      background: var(--accent);
      border-radius: 2px;
    }
    h3 {
      font-family: 'Poppins', sans-serif;
      font-weight: 600;
      font-size: 1.1rem;
      margin-bottom: 6px;
    }
    p { color: var(--muted); font-size: 0.95rem; }

    /* About */
    .about { display: flex; gap: 40px; align-items: flex-start; }
    .avatar {
      width: 140px; height: 140px;
      border-radius: 50%;
      object-fit: cover;
      background: #e8e8f0;
      flex-shrink: 0;
    }
    .hello {
      font-family: 'Poppins', sans-serif;
      font-size: 2rem;
      font-weight: 700;
      margin-bottom: 10px;
    }
    .info {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 8px 30px;
      margin: 20px 0 25px;
      font-size: 0.9rem;
    }
    .info span { color: var(--muted); }
    .info b { font-weight: 600; }
    .btn {
      display: inline-block;
      padding: 9px 22px;
      border-radius: 30px;
      color: #fff;
      text-decoration: none;
      font-size: 0.85rem;
      margin-right: 10px;
      margin-bottom: 8px;
    }
    .btn.red { background: var(--accent); }
    .btn.blue { background: var(--accent2); }

    /* Map */
    .map-frame {
      width: 100%;
      height: 450px;
      border: none;
      border-radius: 12px;
    }

    /* Story timeline */
    .stop {
      display: flex;
      gap: 25px;
      align-items: flex-start;
      padding: 20px 0;
      border-bottom: 1px solid #eeeeee;
    }
    .stop:last-child { border-bottom: none; }
    .stop img {
      width: 200px; height: 140px;
      object-fit: cover;
      border-radius: 12px;
      background: #e8e8f0;
      flex-shrink: 0;
    }
    .tag {
      display: inline-block;
      font-size: 0.75rem;
      font-weight: 600;
      color: var(--accent);
      text-transform: uppercase;
      letter-spacing: 0.5px;
      margin-bottom: 4px;
    }

    /* Skills */
    .skills { display: grid; grid-template-columns: 1fr 1fr; gap: 20px 40px; }
    .skill-top {
      display: flex;
      justify-content: space-between;
      font-family: 'Poppins', sans-serif;
      font-size: 0.8rem;
      font-weight: 600;
      text-transform: uppercase;
      margin-bottom: 6px;
    }
    .skill-top span { color: var(--muted); font-weight: 500; }
    .bar { height: 4px; background: #eeeeee; border-radius: 2px; }
    .fill { height: 100%; background: var(--accent); border-radius: 2px; }

    footer { text-align: center; color: var(--muted); font-size: 0.8rem; }

    @media (max-width: 650px) {
      .card { padding: 25px; }
      .about, .stop { flex-direction: column; }
      .stop img { width: 100%; height: 180px; }
      .info, .skills { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <div class="container">

    <!-- ABOUT ME -->
    <section class="card">
      <h2>About Me</h2>
      <div class="about">
        <img class="avatar" src="andresvila_profilepicture.jpg" alt="Photo of Andrés">
        <div>
          <div class="hello">Hi!, I'm Andrés</div>
          <p>Born and raised in a small coastal town on the Mediterranean, I decided to pursue my Data Science studies in Valencia. Now, driven by the impact of what data can do, I am doing my master’s in Business Intelligence and Process Management.</p>
          <a class="btn blue" href="https://www.linkedin.com/in/YOUR-PROFILE" target="_blank">LinkedIn</a>
        </div>
      </div>
    </section>

    <!-- STORY -->
    <section class="card">
      <h2>My Story</h2>

      <div class="stop">
        <img src="benicasim.jpeg" alt="Benicàssim">
        <div>
          <span class="tag">🌊 Benicàssim, Spain</span>
          <h3>Born and raised</h3>
          <p>Grew up by the Mediterranean, where the sea was never more than a few minutes away. I guess I am already missing it...</p>
        </div>
      </div>

      <div class="stop">
        <img src="valencia.jpeg" alt="Valencia">
        <div>
          <span class="tag">🎓 Valencia, Spain</span>
          <h3>B.Sc. Data Science, European University of Valencia</h3>
          <p>Write a few lines about your degree and what got you into data.</p>
        </div>
      </div>

      <div class="stop">
        <img src="regensburg.jpeg" alt="Regensburg">
        <div>
          <span class="tag">💼 Regensburg, Germany</span>
          <h3>Erasmus+ Exchange</h3>
          <p>Moved to the city to study Data Science and discovered how much you can learn about the world from data.</p>
        </div>
      </div>

      <div class="stop">
        <img src="datamaran.jpeg" alt="Datamaran">
        <div>
          <span class="tag">🤖 Valencia, Spain</span>
          <h3>Product Engineer at an sustainability company</h3>
          <p>Product Engineer at a sustainability company: First proper software development experience..</p>
        </div>
      </div>

      <div class="stop">
        <img src="berlin.jpeg" alt="Berlin">
        <div>
          <span class="tag">🏫 Berlin, Germany</span>
          <h3>BIPM at HWR Berlin</h3>
          <p>Drawn by the impact of data and technology, now studying the BIPM Master.</p>
        </div>
      </div>
    </section>

    <!-- SKILLS -->
    <section class="card">
      <h2>My Skills</h2>
      <div class="skills">
        <div>
          <div class="skill-top">Python <span>90%</span></div>
          <div class="bar"><div class="fill" style="width:90%"></div></div>
        </div>
        <div>
          <div class="skill-top">LLMs &amp; NLP <span>85%</span></div>
          <div class="bar"><div class="fill" style="width:85%"></div></div>
        </div>
        <div>
          <div class="skill-top">SQL &amp; Databases <span>80%</span></div>
          <div class="bar"><div class="fill" style="width:80%"></div></div>
        </div>
        <div>
          <div class="skill-top">German <span>40%</span></div>
          <div class="bar"><div class="fill" style="width:40%"></div></div>
        </div>
      </div>
    </section>

    
    <!-- MAP -->
    <section class="card">
      <h2>My Journey</h2>
      <iframe class="map-frame" src="academic_journey_map.html" title="Map of my journey"></iframe>
    </section>


    <footer>© 2026 Andrés · Made for BIPM Data Science at HWR Berlin</footer>
  </div>
</body>
</html>
