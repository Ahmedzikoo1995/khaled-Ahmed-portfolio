<!-- ANIME-PORTFOLIO.md -->
<!-- Drop this file in your repo root and enable GitHub-Pages for instant hosting -->

<style>
  :root {
    --accent: #ff7ac6;
    --bg: #0d0d1a;
    --card: #1a1a2e;
    --text: #f0f0f0;
  }
  body { background: var(--bg); color: var(--text); font-family: "Segoe UI", sans-serif; }
  h1, h2 { color: var(--accent); }
  .card {
    background: var(--card);
    border-left: 4px solid var(--accent);
    padding: 1rem 1.5rem;
    margin: 1rem 0;
    border-radius: 8px;
    transition: transform .2s;
  }
  .card:hover { transform: translateY(-4px); }
  .tag {
    display: inline-block;
    background: var(--accent);
    color: #000;
    padding: .2rem .6rem;
    border-radius: 999px;
    font-size: .8rem;
    margin: .2rem;
  }
  .skill-bar {
    height: 6px;
    background: #333;
    border-radius: 3px;
    overflow: hidden;
    margin: .3rem 0 .8rem;
  }
  .skill-bar div {
    height: 100%;
    background: var(--accent);
    width: var(--w);
  }
  details { cursor: pointer; margin: 1rem 0; }
  summary { font-weight: bold; color: var(--accent); }
  /* Glitch effect on hover (pure CSS) */
  .glitch {
    position: relative;
    display: inline-block;
  }
  .glitch:hover::before,
  .glitch:hover::after {
    content: attr(data-text);
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background: var(--bg);
  }
  .glitch:hover::before {
    animation: glitch-1 .3s infinite;
    color: #0ff;
    z-index: -1;
  }
  .glitch:hover::after {
    animation: glitch-2 .3s infinite;
    color: #f0f;
    z-index: -2;
  }
  @keyframes glitch-1 { 0%,100%{clip-path:inset(0 0 95% 0);} 20%{clip-path:inset(10% 0 60% 0);} 40%{clip-path:inset(50% 0 10% 0);} 60%{clip-path:inset(90% 0 5% 0);} 80%{clip-path:inset(30% 0 70% 0);} }
  @keyframes glitch-2 { 0%,100%{clip-path:inset(0 0 95% 0);} 20%{clip-path:inset(60% 0 10% 0);} 40%{clip-path:inset(10% 0 50% 0);} 60%{clip-path:inset(5% 0 90% 0);} 80%{clip-path:inset(70% 0 30% 0);} }
</style>

<!--  Hero Section  -->
<div align="center">
  <img src="https://i.giphy.com/media/3o7TKwmnDgQb5jemjK/giphy.gif" width="200" />
  <h1 class="glitch" data-text="Khaled Ahmed">Khaled Ahmed</h1>
  <p><strong>Senior Embedded Software Validation Engineer (HIL & Automotive)</strong></p>
  <p>🇮🇹 Moncalieri, Torino | 📞 +39 331 803 9484 | ✉️ khaled.ahmed@enis.tn</p>
  <a href="https://linkedin.com/in/khaled-ahmed-b157421b2"><img src="https://img.shields.io/badge/-LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white"/></a>
  <a href="https://github.com/YOUR_GITHUB"><img src="https://img.shields.io/badge/-GitHub-181717?style=flat&logo=github&logoColor=white"/></a>
</div>

---

<!--  Quick Nav  -->
<p align="center">
  <a href="#about">About</a> •
  <a href="#skills">Skills</a> •
  <a href="#experience">Experience</a> •
  <a href="#projects">Projects</a> •
  <a href="#contact">Contact</a>
</p>

---

## <span id="about">🌌 About Me</span>
<div class="card">
  <p>5+ years turning ECU nightmares into sweet dreams through <strong>HIL testing</strong>, <strong>Python/CAPL automation</strong> and <strong>diagnostic protocols</strong> (CAN, LIN, Ethernet, SOME/IP, DoIP, UDS).<br>
  I bring PCBs back to life, resurrect 3-year-old blocked test suites, and solder faster than Sanji cooks. Currently validating next-gen automotive software at <strong>Italdesign</strong> while jamming to lofi beats.</p>
</div>

---

## <span id="skills">⚔️ Skill Tree</span>
<div class="card">
  <strong>Protocols</strong><br>
  <span class="tag">CAN</span><span class="tag">LIN</span><span class="tag">Ethernet</span><span class="tag">SOME/IP</span><span class="tag">DoIP</span><span class="tag">UDS</span>
</div>
<div class="card">
  <strong>Tools</strong><br>
  <span class="tag">Vector CANoe</span><span class="tag">vTESTstudio</span><span class="tag">VFlash</span><span class="tag">Lauterbach</span><span class="tag">ODIS</span>
</div>
<div class="card">
  <strong>Languages</strong><br>
  Python
  <div class="skill-bar"><div style="--w:95%"></div></div>
  CAPL
  <div class="skill-bar"><div style="--w:90%"></div></div>
  C/C++
  <div class="skill-bar"><div style="--w:85%"></div></div>
  MATLAB
  <div class="skill-bar"><div style="--w:70%"></div></div>
</div>
<div class="card">
  <strong>Traceability & ALM</strong><br>
  <span class="tag">Codebeamer</span><span class="tag">IBM DOORS</span><span class="tag">Jira</span><span class="tag">Git</span><span class="tag">SharePoint</span>
</div>

---

## <span id="experience">🚀 Experience Timeline</span>

<details open>
<summary><strong>Jun 2023 – Present | Italdesign (Italy)</strong> – Automotive Test Engineer</summary>
<div class="card">
<ul>
  <li>Automated SOME/IP validation over DoIP/TCP/UDP using Python + ENNA framework inside Vector CANoe.</li>
  <li>Maintained bidirectional traceability in Codebeamer; exported live reports to SharePoint.</li>
  <li>Led migration of legacy test infra to Vector toolchain; resurrected 3-year-old blocked tests.</li>
  <li>Executed UDS diagnostics & ECU flashing; climate-chamber tests (-40 °C → +85 °C).</li>
  <li>ADB shenanigans on Android-based head-units; CI pipelines via GitHub Actions.</li>
</ul>
</div>
</details>

<details>
<summary><strong>Apr 2021 – Jun 2023 | Marquardt Group (Tunisia)</strong> – Functional Software Test Engineer</summary>
<div class="card">
<ul>
  <li>HIL validation on VT System & IBB benches; PCB-level measurements; custom test-box design.</li>
  <li>UDS routines, security access, DTC erase, fault-injection robustness tests.</li>
  <li>Reduced onboarding time for new hires from 3 months → 1 month via hands-on dummy projects.</li>
  <li>Improved HIL uptime by 25% through bench optimisation.</li>
</ul>
</div>
</details>

---

## <span id="projects">🎮 Featured Quests</span>

| Thumbnail | Title | Tech | Play |
|-----------|-------|------|------|
| <img src="https://media.giphy.com/media/3o7aCTPPm4OHfRLSH6/giphy.gif" width="80"> | **SOME/IP over DoIP Validator** | Python, CAPL, CANoe | [Source](https://github.com/YOUR_GITHUB/SOMEIP-Validator) |
| <img src="https://media.giphy.com/media/26tn33aiTi1jkl6H6/giphy.gif" width="80"> | **Climate-Chamber Regression Suite** | Python, Jenkins, Codebeamer | [Report](https://YOUR_GITHUB.io/climate-report) |
| <img src="https://media.giphy.com/media/3o7btXcqzgqhqJoH9C/giphy.gif" width="80"> | **PCB Test-Box Designer** | KiCad, C++, VT System | [Docs](https://github.com/YOUR_GITHUB/TestBox) |

---

## <span id="contact">📡 Summon Me</span>
<div class="card" align="center">
  <p>
    <a href="mailto:khaled.ahmed@enis.tn"><img src="https://img.shields.io/badge/-Gmail-EA4335?style=flat&logo=gmail&logoColor=white"/></a>
    <a href="https://linkedin.com/in/khaled-ahmed-b157421b2"><img src="https://img.shields.io/badge/-LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white"/></a>
    <a href="https://github.com/YOUR_GITHUB"><img src="https://img.shields.io/badge/-GitHub-181717?style=flat&logo=github&logoColor=white"/></a>
  </p>
  <p><em>“May your signals always be differential and your grounds noise-free.”</em></p>
</div>

---

<!--  Easter egg  -->
<details>
<summary>🧩 Secret Debug Console</summary>
<pre>
$ id
uid=1337(khaled) gid=1337(embedded) groups=1337(can),100(wireshark)

$ dmesg | grep -i "success"
[    resume] Life: all tests passed – no regression detected
</pre>
</details>