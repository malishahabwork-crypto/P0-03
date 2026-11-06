# P0-03 | Personal Portfolio — Implementation Guide

> **For:** Antigravity (AI Assistant)
> **Goal:** Build a simple personal portfolio website step by step, with each commit mapping to one clear task. The intern (M. Ali Shahab) will push each commit to GitHub to demonstrate AI-assisted development.

---

## Project Overview

Build a **single-page personal portfolio website** using only HTML and CSS. No frameworks, no npm, no build tools. The reviewer must be able to run the project by opening `index.html` in a browser — nothing else.

### Final File Structure

```
P0-03/
├── README.md
├── index.html
└── style.css
```

---

## Commit Plan

Each commit below is one task. Complete them **in order**. Do not combine multiple tasks into one commit.

---

### Commit 1 — Project Setup
**Branch:** `main`
**Message:** `chore: initial project setup`

**What to do:**
- The README.md already exists (created on GitHub). Leave it for now.
- Create an empty `index.html` with just the HTML boilerplate:
  ```html
  <!DOCTYPE html>
  <html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>M. Ali Shahab | Portfolio</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
  </body>
  </html>
  ```
- Create an empty `style.css` file.
- Commit both files.

---

### Commit 2 — Navigation & Hero Section
**Branch:** `add-portfolio` ← create this branch before this commit
**Message:** `feat: add navigation and hero section`

**What to do:**
Add inside `<body>` in `index.html`:

```html
<!-- Navigation -->
<nav>
  <div class="nav-logo">Ali Shahab</div>
  <ul class="nav-links">
    <li><a href="#about">About</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- Hero -->
<section id="hero">
  <h1>Hi, I'm <span class="highlight">M. Ali Shahab</span></h1>
  <p class="tagline">Intern Developer · AI-Assisted Builder · Lifelong Learner</p>
  <a href="#contact" class="btn">Get In Touch</a>
</section>
```

Add to `style.css`:
- Reset styles (`* { margin: 0; padding: 0; box-sizing: border-box; }`)
- Font: `font-family: 'Segoe UI', sans-serif`
- Nav: flex layout, sticky top, clean background
- Hero: centered text, full viewport height, background color `#0f172a`, white text
- `.highlight`: accent color `#38bdf8`
- `.btn`: styled call-to-action button

---

### Commit 3 — About Section
**Branch:** `add-portfolio`
**Message:** `feat: add about section`

**What to do:**
Add after the hero in `index.html`:

```html
<section id="about">
  <h2>About Me</h2>
  <p>
    I'm a Computer Science student currently interning and learning AI-assisted
    development. I built this portfolio using HTML, CSS, and GitHub — with help
    from Claude (Anthropic's AI) to accelerate my workflow.
  </p>
</section>
```

Add to `style.css`:
- Section padding: `80px 20px`
- Max width container: `800px`, centered
- `h2` styling with an underline accent

---

### Commit 4 — Skills Section
**Branch:** `add-portfolio`
**Message:** `feat: add skills section`

**What to do:**
Add after about in `index.html`:

```html
<section id="skills">
  <h2>Skills</h2>
  <div class="skills-grid">
    <div class="skill-card">HTML</div>
    <div class="skill-card">CSS</div>
    <div class="skill-card">Git & GitHub</div>
    <div class="skill-card">AI-Assisted Dev</div>
    <div class="skill-card">Problem Solving</div>
    <div class="skill-card">Python (Basics)</div>
  </div>
</section>
```

Add to `style.css`:
- `.skills-grid`: CSS grid, 3 columns, gap between cards
- `.skill-card`: bordered box, centered text, hover effect (slight scale or color change)

---

### Commit 5 — Projects Section
**Branch:** `add-portfolio`
**Message:** `feat: add projects section`

**What to do:**
Add after skills in `index.html`:

```html
<section id="projects">
  <h2>Projects</h2>
  <div class="project-card">
    <h3>Personal Portfolio</h3>
    <p>
      A clean, responsive portfolio page built with HTML and CSS.
      Developed using AI-assisted workflow with Claude and version-controlled
      on GitHub.
    </p>
    <a href="https://github.com/malishahabwork-crypto/P0-03" target="_blank">View on GitHub →</a>
  </div>
</section>
```

Add to `style.css`:
- `.project-card`: white card, box shadow, padding, rounded corners
- Link styling with accent color

---

### Commit 6 — Contact Section & Footer
**Branch:** `add-portfolio`
**Message:** `feat: add contact section and footer`

**What to do:**
Add after projects in `index.html`:

```html
<section id="contact">
  <h2>Contact</h2>
  <p>Feel free to reach out via email or GitHub.</p>
  <a href="mailto:your@email.com" class="btn">Email Me</a>
</section>

<footer>
  <p>Built with HTML, CSS & Claude AI · M. Ali Shahab · 2024</p>
  <a href="https://github.com/malishahabwork-crypto/P0-03" target="_blank">GitHub Repo</a>
</footer>
```

Add to `style.css`:
- Contact section: centered, dark background (`#0f172a`), white text
- Footer: small text, centered, border top

---

### Commit 7 — README Update
**Branch:** `add-portfolio`
**Message:** `docs: update README with project description and run instructions`

**What to do:**
Replace the contents of `README.md` with:

```markdown
# P0-03 | Personal Portfolio

A simple personal portfolio website built with HTML and CSS as part of an
AI-assisted development internship task.

## How to Run

1. Clone the repository:
   git clone https://github.com/malishahabwork-crypto/P0-03.git

2. Open the project folder.

3. Open index.html in any web browser.

No installs. No dependencies. It just works.

## Files

| File         | Description                                      |
|--------------|--------------------------------------------------|
| index.html   | Main page structure — all sections live here     |
| style.css    | All visual styling — layout, colors, typography  |
| README.md    | Project description and instructions (this file) |

## What I Changed (Commit History)

| Commit | Change |
|--------|--------|
| 1 | Project setup — created index.html and style.css |
| 2 | Added navigation bar and hero section |
| 3 | Added about me section |
| 4 | Added skills grid section |
| 5 | Added projects section |
| 6 | Added contact section and footer |
| 7 | Updated README with full documentation |

## Built With

- HTML5
- CSS3
- GitHub (branches, commits, pull requests)
- Claude AI (Anthropic) — used for code generation and guidance
```

---

## Pull Request

Once all 7 commits are pushed on the `add-portfolio` branch:

1. Go to: `https://github.com/malishahabwork-crypto/P0-03`
2. Click **"Compare & pull request"**
3. Set title: `feat: add complete portfolio page`
4. Set description:

```
## What this PR does
Adds a complete personal portfolio page with the following sections:
- Navigation
- Hero
- About
- Skills
- Projects
- Contact & Footer

## Files changed
- index.html — full page structure
- style.css — all styling
- README.md — project docs and run instructions

## How to review
Clone the repo, open index.html in a browser. No setup needed.
```

5. Click **Create pull request**
6. Then click **Merge pull request**

---

## Done Checklist

- [ ] Repository exists on GitHub
- [ ] At least 5 commits with clear messages
- [ ] `add-portfolio` branch created and merged via Pull Request
- [ ] `index.html` and `style.css` are on `main` after merge
- [ ] README explains files and how to run
- [ ] Short demo recorded (use Loom or screen recorder)
- [ ] Handbook entry written explaining each file and each change

