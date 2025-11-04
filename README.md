 <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Ritik's GitHub Profile README</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Inconsolata&family=Roboto+Mono&display=swap');

  /* Base Reset */
  * {
    box-sizing: border-box;
  }

  body {
    margin: 0;
    background-color: #12121e;
    color: #c7c7d9;
    font-family: 'Roboto Mono', monospace;
    line-height: 1.5;
    min-height: 100vh;
    padding: 20px;
  }

  /* Container */
  .container {
    max-width: 900px;
    margin: 0 auto;
  }

  /* Header Banner */
  .header-banner {
    background: linear-gradient(135deg, #332b45 10%, #a15141 90%);
    border-radius: 15px;
    color: #fff;
    font-family: 'Inconsolata', monospace;
    text-align: center;
    padding: 60px 20px 40px;
    position: relative;
    box-shadow: 0 6px 12px #1f1a2d88;
  }
  .header-banner .greeting {
    font-size: 2rem;
    font-weight: 700;
    margin-bottom: 8px;
  }
  .header-banner .highlight-dot {
    color: #f7c161;
    font-size: 2rem;
    font-weight: 900;
    margin-left: 8px;
  }
  .header-banner .subtitle {
    font-size: 1.1rem;
    font-weight: 400;
    opacity: 0.85;
  }
  /* Placeholder for an SVG landscape */
  .header-banner svg {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 120px;
    z-index: 0;
  }

  /* Stats badges container */
  .stats-badges {
    margin: 15px 0 30px;
    display: flex;
    gap: 15px;
    justify-content: center;
  }
  .stats-badge {
    background-color: #1f1f37;
    border-radius: 6px;
    padding: 8px 16px;
    color: #7efc8a;
    font-weight: 700;
    font-size: 0.9rem;
    cursor: default;
    user-select: none;
    box-shadow: 0 0 10px #2f3f4f88;
  }

  /* Description paragraph with emojis */
  .description {
    max-width: 760px;
    margin: 0 auto 40px;
    font-size: 1rem;
    line-height: 1.6;
    text-align: center;
  }
  .description span {
    font-size: 1.2rem;
    line-height: 1;
    vertical-align: middle;
    margin: 0 4px;
  }

  /* Technology Stack */
  .tech-stack {
    text-align: center;
    margin-bottom: 50px;
  }
  .tech-stack h2 {
    margin-bottom: 15px;
    font-weight: 600;
    color: #d9d9f0;
    font-size: 1.3rem;
  }
  .badges-row {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 8px;
  }
  .badge {
    padding: 6px 10px;
    border-radius: 5px;
    font-weight: 700;
    font-family: monospace;
    color: white;
    user-select: none;
    box-shadow: 0 0 5px #0008;
    transition: transform 0.15s ease;
  }
  .badge:hover {
    transform: translateY(-3px);
    box-shadow: 0 5px 15px #ffaaaabb;
  }
  /* Colors inspired by original logos */
  .badge.cc { background-color: #004f9f; }
  .badge.java { background-color: #d7432a; }
  .badge.cpp { background-color: #00599c; }
  .badge.html5 { background-color: #e44d26; }
  .badge.css3 { background-color: #264de4; }
  .badge.bootstrap { background-color: #7952b3; }
  .badge.heroku { background-color: #6762a6; }
  .badge.javascript { background-color: #f0db4f; color: #222; }
  .badge.nodejs { background-color: #6cc24a; color: #222; }
  .badge.react { background-color: #61dafb; color: #222; }
  .badge.mongodb { background-color: #4db33d; }
  .badge.mysql { background-color: #00758f; }
  .badge.github { background-color: #333; }

  /* GitHub Stats Section */
  .github-stats {
    background-color: #181826;
    border-radius: 12px;
    padding: 30px 25px;
    box-shadow: 0 0 30px #3a3a5a7d inset;
    max-width: 900px;
    margin: 0 auto;
  }
  .github-stats h2 {
    color: #e0aaff;
    font-weight: 700;
    text-align: center;
    margin-bottom: 25px;
  }

  .stats-container {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    justify-content: center;
  }

  /* Left stats box */
  .stats-left {
    background: #211f2f;
    padding: 25px 30px;
    border-radius: 10px;
    width: 320px;
    color: #b5b5dc;
    font-family: monospace;
    box-shadow: 0 0 15px #48146466;
  }
  .stats-left h3 {
    margin: 0 0 20px;
    color: #f0aaff;
    font-weight: 600;
    font-size: 1.1rem;
  }
  .stats-list {
    list-style: none;
    padding-left: 0;
    margin: 0;
  }
  .stats-list li {
    margin-bottom: 12px;
    font-size: 0.95rem;
    display: flex;
    align-items: center;
    color: #d7d7f0;
  }
  .stats-list li span.icon {
    margin-right: 10px;
    font-size: 1.15rem;
  }

  /* Grade Circle */
  .grade-circle {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    border: 3.5px solid #a48dff;
    color: #a48dff;
    font-weight: 900;
    font-size: 1.8rem;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 25px auto 0;
  }

  /* Language Usage - Right side */
  .stats-right {
    background: #211f2f;
    border-radius: 10px;
    width: 530px;
    padding: 25px 30px;
    box-shadow: 0 0 15px #48146466;
  }
  .stats-right h3 {
    margin: 0 0 20px;
    color: #f0aaff;
    font-weight: 600;
    font-size: 1.1rem;
  }
  .language-bar {
    margin-bottom: 18px;
  }
  .language-bar label {
    display: block;
    color: #c1c1e8;
    font-weight: 600;
    margin-bottom: 5px;
    font-size: 0.95rem;
  }
  .language-bar .bar-bg {
    background-color: #393958;
    border-radius: 10px;
    height: 16px;
    overflow: hidden;
  }
  .language-bar .bar-fill {
    height: 100%;
    border-radius: 10px 0 0 10px;
  }
  .bar-javascript {
    width: 60.81%;
    background-color: #f7df1e;
    box-shadow: 0 0 8px #f7df1eaa;
  }
  .bar-c {
    width: 37.83%;
    background-color: #004f9f;
    box-shadow: 0 0 8px #004f9faa;
  }
  .bar-cpp {
    width: 1.36%;
    background-color: #00599c;
    box-shadow: 0 0 8px #00599caa;
  }

  /* Bottom stats badges */
  .bottom-stats {
    margin-top: 35px;
    display: flex;
    justify-content: center;
    gap: 30px;
    flex-wrap: wrap;
  }
  .stat-card {
    background: #211f2f;
    border-radius: 12px;
    padding: 25px 30px;
    width: 220px;
    text-align: center;
    box-shadow: 0 0 15px #48146466;
    font-family: monospace;
    user-select: none;
  }
  .stat-card .number {
    font-size: 2.7rem;
    font-weight: 900;
    color: #ff5f85;
    margin-bottom: 5px;
  }
  .stat-card .label {
    font-size: 1rem;
    color: #bbb;
    white-space: pre-line;
    line-height: 1.3;
  }

  /* Helper Icons (Unicode emojis) */
  .icon-star::before { content: "⭐"; margin-right: 8px; }
  .icon-commit::before { content: "📅"; margin-right: 8px; }
  .icon-pr::before { content: "🔀"; margin-right: 8px; }
  .icon-issue::before { content: "🐛"; margin-right: 8px; }
  .icon-contrib::before { content: "🚀"; margin-right: 8px; }
  
  /* Responsive */
  @media (max-width: 768px) {
    .stats-container {
      flex-direction: column;
      align-items: center;
    }
    .stats-left,
    .stats-right {
      width: 100%;
      max-width: 600px;
    }
    .bottom-stats {
      flex-direction: column;
      gap: 20px;
      align-items: center;
    }
  }
</style>
</head>
<body>
<div class="container">

  <!-- Header Banner -->
  <section class="header-banner" aria-label="Profile Banner - Hi, I'm Ritik">
    <div class="greeting">Hi, I'm Krish Kumar<span class="highlight-dot">●</span></div>
    <div class="subtitle">A Web Developer in making</div>

    <!-- Optional SVG background shape -->
    <svg viewBox="0 0 900 150" preserveAspectRatio="none" aria-hidden="true">
      <path fill="#432e35" d="M0 0 L300 150 L600 10 L900 150 L900 0 Z"/>
    </svg>
  </section>

  <!-- Stats badges: Visits / Repos / Commits this month -->
  <div class="stats-badges" aria-label="Visits, Repositories and Commits statistics">
    <div class="stats-badge" title="Total visits">Visits 50</div>
    <div class="stats-badge" title="Repositories">Repos 05</div>
    <div class="stats-badge" title="Commits this month">Commits this month 70</div>
  </div>

  <!-- Description / About me -->
  <p class="description" aria-label="About Me">
    I&apos;m a 2nd year student pursuing Bachlor&apos;s in Computer Science <span>🎓</span> from A.P.J. Kalam University <span>🏫</span>. I&apos;m a passionate learner who&apos;s always willing to learn and work across technologies and domains <span>⭐</span>. I love to explore new technologies and leverage them to solve real-life problems <span>💡</span>. Apart from that I also love to explore new things <span>🙌</span>. I&apos;m currently into Web Development <span>🌐</span> and working on my Data Structures and Algorithms skills <span>🤓</span>.
  </p>

  <!-- Technology Stack -->
  <section class="tech-stack" aria-label="Technology Stack">
    <h2>Technology Stack 🛠</h2>
    <div class="badges-row">
      <span class="badge c">C</span>
      <span class="badge cpp">C++</span>
      <span class="badge html5">HTML5</span>
      <span class="badge css3">CSS3</span>
      <span class="badge bootstrap">Bootstrap</span>
      <span class="badge javascript">JavaScript</span>
      <span class="badge git">Git</span>
      <span class="badge github">GitHub</span>
    </div>
  </section>

  <!-- GitHub Stats -->
  <section class="github-stats" aria-label="GitHub Statistics">
    <h2>My GitHub Stats 🐙</h2>
    <div class="stats-container">

      <!-- Left Stats -->
      <div class="stats-left" role="region" aria-labelledby="githubstatsTitle">
        <h3 id="githubstatsTitle">Krish Kumar's GitHub Stats</h3>
        <ul class="stats-list">
          <li><span class="icon icon-star"></span> Total Stars: 7</li>
          <li><span class="icon icon-commit"></span> Total Commits (2021+): 397</li>
          <li><span class="icon icon-pr"></span> Total PRs: 106</li>
          <li><span class="icon icon-issue"></span> Total Issues: 38</li>
          <li><span class="icon icon-contrib"></span> Contributed to: 33</li>
        </ul>

        <div class="grade-circle" aria-label="Github Grade A Plus">A+</div>
      </div>

      <!-- Right Stats - Language Usage -->
      <div class="stats-right" role="region" aria-labelledby="langusageTitle">
        <h3 id="langusageTitle">Most Used Languages</h3>
        <div class="language-bar" aria-label="JavaScript usage 60.81%">
          <label>JavaScript</label>
          <div class="bar-bg"><div class="bar-fill bar-javascript"></div></div>
        </div>
        <div class="language-bar" aria-label="C usage 37.83%">
          <label>C</label>
          <div class="bar-bg"><div class="bar-fill bar-c"></div></div>
        </div>
        <div class="language-bar" aria-label="C++ usage 1.36%">
          <label>C++</label>
          <div class="bar-bg"><div class="bar-fill bar-cpp"></div></div>
        </div>
      </div>

    </div>

    <!-- Bottom Stats -->
    <div class="bottom-stats" role="contentinfo" aria-label="Contribution and streak statistics">
      <div class="stat-card" aria-label="Total Contributions: 888 from Sep 22, 2016 to Present">
        <div class="number">888</div>
        <div class="label">Total Contributions<br />Sep 22, 2016 - Present</div>
      </div>
      <div class="stat-card" aria-label="Current Streak: 1 day">
        <div class="number">1</div>
        <div class="label">Current Streak</div>
      </div>
      <div class="stat-card" aria-label="Longest Streak: 145 days from Jan 9 to Jun 2">
        <div class="number">145</div>
        <div class="label">Longest Streak<br />Jan 9 - Jun 2</div>
      </div>
    </div>
  </section>

</div>
</body>
</html>