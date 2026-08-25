---
title: Shaoduo Fu
description: Personal homepage of Shaoduo Fu, Tianjin University
---

<style>
  :root {
    --page-bg: #f3f1ec;
    --paper: #ffffff;
    --ink: #1d252c;
    --muted: #5e6870;
    --navy: #244862;
    --navy-dark: #173247;
    --soft-blue: #edf3f6;
    --rule: #b9c6ce;
  }

  * { box-sizing: border-box; }

  html { scroll-behavior: smooth; }

  body {
    margin: 0;
    color: var(--ink);
    background: var(--page-bg);
    font-family: Inter, Arial, "Helvetica Neue", sans-serif;
    font-size: 16px;
    line-height: 1.7;
  }

  body > .container-lg {
    max-width: none !important;
    margin: 0 !important;
    padding: 0 !important;
  }

  .markdown-body {
    color: inherit;
    font-family: inherit;
  }

  .homepage {
    width: min(980px, calc(100% - 40px));
    margin: 30px auto 64px;
    overflow: hidden;
    border-top: 6px solid var(--navy);
    background: var(--paper);
    box-shadow: 0 18px 55px rgba(28, 43, 54, 0.11);
  }

  .site-nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 24px;
    padding: 20px 64px;
    border-bottom: 1px solid #dce3e7;
  }

  .monogram {
    display: grid;
    width: 38px;
    height: 38px;
    place-items: center;
    border: 1px solid var(--navy);
    color: var(--navy-dark) !important;
    font-family: Georgia, "Times New Roman", serif;
    font-weight: 700;
    letter-spacing: 0.04em;
    text-decoration: none !important;
  }

  .nav-links {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-end;
    gap: 8px 24px;
  }

  .nav-links a {
    color: var(--muted) !important;
    font-size: 0.82rem;
    font-weight: 600;
    letter-spacing: 0.055em;
    text-decoration: none !important;
    text-transform: uppercase;
  }

  .nav-links a:hover { color: var(--navy) !important; }

  .hero {
    display: grid;
    grid-template-columns: minmax(0, 1fr) 250px;
    align-items: center;
    gap: 68px;
    padding: 62px 64px 58px;
  }

  .hero h1 {
    margin: 0 0 12px !important;
    padding: 0 !important;
    border: 0 !important;
    color: var(--navy-dark);
    font-family: Georgia, "Times New Roman", serif;
    font-size: clamp(3rem, 7vw, 4.5rem);
    font-weight: 600;
    letter-spacing: -0.045em;
    line-height: 1.03;
  }

  .degree {
    margin: 0 0 26px !important;
    color: var(--muted);
    font-size: 1.08rem;
  }

  .contact-list {
    display: grid;
    gap: 7px;
    margin: 0 0 24px;
    color: var(--ink);
  }

  .contact-list p { margin: 0 !important; }

  .contact-label {
    display: inline-block;
    min-width: 72px;
    color: var(--navy-dark);
    font-weight: 600;
  }

  .contact-list a {
    color: var(--ink) !important;
    text-decoration: none !important;
  }

  .contact-list a:hover { color: var(--navy) !important; }

  .social-links {
    display: flex;
    gap: 11px;
  }

  .social-link {
    display: grid;
    width: 43px;
    height: 43px;
    place-items: center;
    border: 1.5px solid var(--rule);
    border-radius: 50%;
    color: var(--navy-dark) !important;
    background: #fff;
    text-decoration: none !important;
    transition: transform 160ms ease, border-color 160ms ease, background 160ms ease;
  }

  .social-link:hover {
    transform: translateY(-2px);
    border-color: var(--navy);
    background: var(--soft-blue);
  }

  .social-link svg {
    width: 21px;
    height: 21px;
  }

  .portrait {
    display: block;
    width: 250px;
    aspect-ratio: 4 / 5;
    border: 1px solid #cbd5da;
    border-radius: 3px;
    object-fit: cover;
    box-shadow: 14px 14px 0 var(--soft-blue);
  }

  .content-section {
    padding: 38px 64px 42px;
    border-top: 3px solid var(--rule);
  }

  .section-heading {
    display: flex;
    align-items: baseline;
    gap: 14px;
    margin-bottom: 17px;
  }

  .section-number {
    color: var(--navy);
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.12em;
  }

  .content-section h2 {
    margin: 0 !important;
    padding: 0 !important;
    border: 0 !important;
    color: var(--navy-dark);
    font-family: Georgia, "Times New Roman", serif;
    font-size: 1.65rem;
    font-weight: 600;
  }

  .section-placeholder {
    margin: 0 !important;
    color: var(--muted);
    font-style: italic;
  }

  .site-footer {
    padding: 22px 64px;
    border-top: 3px solid var(--navy);
    color: var(--muted);
    background: #f7f9fa;
    font-size: 0.8rem;
    text-align: center;
  }

  @media (max-width: 760px) {
    .homepage {
      width: min(100% - 24px, 980px);
      margin-top: 12px;
    }

    .site-nav {
      align-items: flex-start;
      padding: 18px 24px;
    }

    .nav-links { gap: 6px 14px; }

    .hero {
      grid-template-columns: 1fr;
      gap: 34px;
      padding: 42px 28px 44px;
    }

    .portrait {
      grid-row: 1;
      width: min(220px, 78vw);
      justify-self: start;
    }

    .content-section { padding: 32px 28px 36px; }
    .site-footer { padding: 20px 28px; }
  }

  @media (max-width: 480px) {
    .site-nav { display: block; }
    .monogram { margin-bottom: 16px; }
    .nav-links { justify-content: flex-start; }
    .hero h1 { font-size: 2.75rem; }
  }
</style>

<main class="homepage">
  <nav class="site-nav" aria-label="Primary navigation">
    <a class="monogram" href="#top" aria-label="Back to top">SF</a>
    <div class="nav-links">
      <a href="#profile">Profile</a>
      <a href="#education">Education</a>
      <a href="#publications">Publications</a>
      <a href="#patents">Patents</a>
      <a href="#awards">Awards</a>
    </div>
  </nav>

  <header class="hero" id="top">
    <div>
      <h1>Shaoduo Fu</h1>
      <p class="degree">Doctor of Engineering, Tianjin University</p>

      <div class="contact-list" aria-label="Contact information">
        <p><span class="contact-label">Email</span><a href="mailto:fushaoduo@tju.edu.cn">fushaoduo@tju.edu.cn</a></p>
        <p><span class="contact-label">WeChat</span>F116357</p>
      </div>

      <div class="social-links" aria-label="Academic and social profiles">
        <a class="social-link" href="https://scholar.google.com/citations?user=SNuRYxQAAAAJ&amp;hl=zh-CN&amp;oi=ao" target="_blank" rel="noopener noreferrer" aria-label="Google Scholar" title="Google Scholar">
          <svg viewBox="0 0 24 24" fill="none" aria-hidden="true">
            <path d="M2.5 9.4 12 4l9.5 5.4L12 14.8 2.5 9.4Z" fill="currentColor"/>
            <path d="M6.2 11.6v4.1c0 1.7 2.6 3.1 5.8 3.1s5.8-1.4 5.8-3.1v-4.1L12 14.9l-5.8-3.3Z" fill="currentColor" opacity=".72"/>
            <path d="M21.5 9.5v6" stroke="currentColor" stroke-width="1.6" stroke-linecap="round"/>
          </svg>
        </a>

        <a class="social-link" href="https://orcid.org/my-orcid?orcid=0009-0006-9726-7968" target="_blank" rel="noopener noreferrer" aria-label="ORCID" title="ORCID">
          <svg viewBox="0 0 24 24" aria-hidden="true">
            <circle cx="12" cy="12" r="10" fill="#a6ce39"/>
            <circle cx="8" cy="7.7" r="1.2" fill="#fff"/>
            <path d="M7 10h2v7H7zm3.7 0h3.2c2.6 0 4.4 1.3 4.4 3.5S16.5 17 13.9 17h-3.2v-7Zm2 1.8v3.4h1.1c1.5 0 2.4-.6 2.4-1.7s-.9-1.7-2.4-1.7h-1.1Z" fill="#fff"/>
          </svg>
        </a>

        <a class="social-link" href="https://github.com/YoungBell" target="_blank" rel="noopener noreferrer" aria-label="GitHub" title="GitHub">
          <svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true">
            <path d="M12 .8a11.4 11.4 0 0 0-3.6 22.2c.6.1.8-.2.8-.5v-2.2c-3.3.7-4-1.4-4-1.4-.5-1.4-1.3-1.7-1.3-1.7-1.1-.8.1-.8.1-.8 1.2.1 1.8 1.2 1.8 1.2 1.1 1.8 2.8 1.3 3.5 1 .1-.8.4-1.3.8-1.6-2.6-.3-5.4-1.3-5.4-5.7 0-1.3.5-2.3 1.2-3.1-.1-.3-.5-1.5.1-3.1 0 0 1-.3 3.2 1.2A11 11 0 0 1 12 6c1 0 2 .1 2.9.4 2.2-1.5 3.2-1.2 3.2-1.2.6 1.6.2 2.8.1 3.1.8.8 1.2 1.8 1.2 3.1 0 4.4-2.7 5.4-5.4 5.7.4.4.8 1.1.8 2.1v3.2c0 .3.2.6.8.5A11.4 11.4 0 0 0 12 .8Z"/>
          </svg>
        </a>
      </div>
    </div>

    <img class="portrait" src="/assets/profile.jpg" alt="Portrait of Shaoduo Fu">
  </header>

  <section class="content-section" id="profile">
    <div class="section-heading"><span class="section-number">01</span><h2>Profile</h2></div>
    <p class="section-placeholder">Profile content will be added here.</p>
  </section>

  <section class="content-section" id="education">
    <div class="section-heading"><span class="section-number">02</span><h2>Education</h2></div>
    <p class="section-placeholder">Education details will be added here.</p>
  </section>

  <section class="content-section" id="publications">
    <div class="section-heading"><span class="section-number">03</span><h2>Publications</h2></div>
    <p class="section-placeholder">Publications will be added here.</p>
  </section>

  <section class="content-section" id="patents">
    <div class="section-heading"><span class="section-number">04</span><h2>Patents</h2></div>
    <p class="section-placeholder">Patents will be added here.</p>
  </section>

  <section class="content-section" id="awards">
    <div class="section-heading"><span class="section-number">05</span><h2>Awards</h2></div>
    <p class="section-placeholder">Awards and honors will be added here.</p>
  </section>

  <footer class="site-footer">© 2026 Shaoduo Fu · Hosted with GitHub Pages</footer>
</main>


