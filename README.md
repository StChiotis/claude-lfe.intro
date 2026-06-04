# Claude-LFE — Introduction

An interactive, single-page introduction to **Claude-LFE** — built as a self-contained HTML presentation (no build step, no dependencies beyond a web font).

### ▶︎ Live deck
**https://stchiotis.github.io/claude-lfe.intro/**

Navigate with the arrow keys, on-screen controls, or swipe. Best viewed full-screen.

### The framework it promotes
This deck is the front door to the framework itself:

**→ https://github.com/StChiotis/claude-lfe**

> clone it · try to break it · make it stronger

---

## How it's hosted

This repo is published with **GitHub Pages**. Everything is static — `index.html` plus its `scenes/`, `assets/`, and `uploads/` folders.

A workflow at `.github/workflows/deploy.yml` redeploys the site automatically on every push to `main`. To enable it once:

**Settings → Pages → Build and deployment → Source: _GitHub Actions_**

That's it — every commit thereafter republishes the live deck.

## Structure

```
index.html          the presentation (entry point)
deck-stage.js        slide stage / navigation
scenes/
  lfe.css            shared design system
  deck.css           deck layout & animation
  image-slot.js      image drop component
assets/              presenter imagery
uploads/             logos & brand marks
```

## Local preview

It's plain static files, so any static server works:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

---

Made with the Claude-LFE framework.
