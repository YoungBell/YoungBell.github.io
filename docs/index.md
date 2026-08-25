---
title: Shaoduo Fu
---

<style>
  :root {
    --ink: #262626;
    --muted: #666;
    --link: #1a5fb4;
    --line: #dedede;
  }

  * { box-sizing: border-box; }
  html { scroll-behavior: smooth; }
  body {
    margin: 0;
    color: var(--ink);
    background: #fff;
    font-family: Arial, "Helvetica Neue", sans-serif;
    font-size: 16px;
    line-height: 1.65;
  }
  .page {
    width: min(820px, calc(100% - 40px));
    margin: 0 auto;
    padding: 56px 0 40px;
  }
  .profile {
    display: grid;
    grid-template-columns: minmax(0, 1fr) 160px;
    align-items: center;
    gap: 48px;
    padding-bottom: 28px;
  }
  .profile h1 {
    margin: 0 0 6px;
    font-family: Georgia, "Times New Roman", serif;
    font-size: clamp(2.6rem, 7vw, 4rem);
    font-weight: 600;
    letter-spacing: -0.045em;
    line-height: 1.08;
  }
  .subtitle { margin: 0 0 14px; color: var(--muted); }
  .links { display: flex; flex-wrap: wrap; gap: 8px 18px; }
  .links a, .page a { color: var(--link); text-decoration: none; }
  .links a:hover, .page a:hover { text-decoration: underline; }
  .avatar {
    width: 160px;
    height: 160px;
    border-radius: 8px;
    object-fit: cover;
    border: 1px solid var(--line);
  }
  .page section {
    padding: 24px 0;
    border-top: 1px solid var(--line);
  }
  .page h2 {
    margin: 0 0 12px;
    font-family: Georgia, "Times New Roman", serif;
    font-size: 1.5rem;
    font-weight: 600;
  }
  .page p { margin: 0 0 10px; }
  .page ul, .page ol { margin: 0; padding-left: 1.35rem; }
  .page li + li { margin-top: 8px; }
  .placeholder { color: var(--muted); }
  .page footer {
    padding-top: 20px;
    border-top: 1px solid var(--line);
    color: var(--muted);
    font-size: 0.82rem;
    text-align: center;
  }
  @media (max-width: 620px) {
    .page { width: min(100% - 28px, 820px); padding-top: 34px; }
    .profile { grid-template-columns: 1fr; gap: 22px; }
    .avatar { grid-row: 1; width: 120px; height: 120px; }
  }
</style>

<main class="page">
  <header class="profile">
    <div>
      <h1>Shaoduo Fu</h1>
      <p class="subtitle">Personal Homepage</p>
      <nav class="links" aria-label="Profile links">
        <a href="https://github.com/YoungBell">GitHub</a>
      </nav>
    </div>
    <img class="avatar" src="https://avatars.githubusercontent.com/u/175574657?v=4" alt="Shaoduo Fu">
  </header>

  <section id="about">
    <h2>About Me</h2>
    <p class="placeholder">个人简介待补充。可以在这里介绍你的研究方向、专业背景，以及目前关注的问题。</p>
  </section>

  <section id="interests">
    <h2>Research Interests</h2>
    <ul>
      <li class="placeholder">研究方向待补充</li>
    </ul>
  </section>

  <section id="education">
    <h2>Education</h2>
    <ul>
      <li class="placeholder">教育经历待补充</li>
    </ul>
  </section>

  <section id="publications">
    <h2>Publications</h2>
    <ol>
      <li class="placeholder">论文与学术成果待补充</li>
    </ol>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <ul>
      <li><a href="https://github.com/YoungBell">GitHub Projects</a> — <span class="placeholder">项目介绍待补充</span></li>
    </ul>
  </section>

  <section id="awards">
    <h2>Awards</h2>
    <ul>
      <li class="placeholder">奖项与荣誉待补充</li>
    </ul>
  </section>

  <footer>© 2026 Shaoduo Fu · Hosted with GitHub Pages</footer>
</main>

