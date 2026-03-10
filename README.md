# CNC Programming Learning Portal

An interactive, self-paced learning portal for aspiring CNC programmers. Built as a single-page HTML application and hosted via GitHub Pages — no backend, no dependencies, no install required.

Live Demo: https://rigarcia07.github.io/web-cnc/

---

## What It Is

A structured 3-month career track covering everything a junior CNC programmer needs to know — from coordinate systems and G-code fundamentals to Fusion 360 CAM and job-ready skills. Progress is tracked interactively with checkboxes that persist across sessions.

---

## Features

- **12-week curriculum** across 3 phases: Foundations → Real Programs → CAM + Capstone
- **Interactive progress tracking** — checkboxes save to localStorage automatically
- **Per-week completion %** displayed on each card
- **Collapsible week cards** to reduce scroll fatigue
- **Embedded NCViewer** live G-code simulator in the sidebar
- **Curated resource links** — PDFs, YouTube tutorials, tools, and forums — all validated
- **Critical Safety panel** always visible in the sidebar
- **Makerspace / industrial dark UI** — optimized for readability on any screen

---

## Curriculum Overview

| Phase | Weeks | Topics |
|-------|-------|--------|
| 01 — Foundations | 1–4 | Axes, coordinate systems, G0/G1, arcs, canned cycles, work offsets |
| 02 — Real Programs | 5–8 | Tool length offsets, feeds & speeds, drilling/tapping cycles, subprograms |
| 03 — CAM + Capstone | 9–12 | Fusion 360 CAM, advanced operations, capstone project, job prep |

---

## Hosting on GitHub Pages

1. Create a new GitHub repository
2. Upload `index.html` to the root of the `main` branch
3. Go to **Settings → Pages** in your repository
4. Under **Source**, select `Deploy from a branch` → choose `main` → `/ (root)`
5. Click **Save** — your site will be live at `https://yourusername.github.io/repo-name`

> GitHub Pages can take 1–2 minutes to deploy on first push. Subsequent updates are usually faster.

---

## Project Structure

```
/
└── index.html      # The entire application — fully self-contained
```

Everything lives in a single `index.html` file. Fonts load from Google Fonts CDN. No build step, no npm, no framework, no additional files needed.

---

## Local Development

No server required. Just open `index.html` directly in any modern browser:

```bash
# Option 1 — open directly
open index.html

# Option 2 — serve locally (avoids any iframe restrictions)
npx serve .
# or
python3 -m http.server 8080
```

---

## Browser Support

Works in all modern browsers. Requires JavaScript enabled for checkbox progress tracking and week card toggling.

| Browser | Support |
|---------|---------|
| Chrome / Edge | ✅ Full |
| Firefox | ✅ Full |
| Safari | ✅ Full |
| Mobile (iOS / Android) | ✅ Responsive |

---

## Progress Persistence

Checkbox state is saved to `localStorage` under the key `cncRoadmapV3`. Progress persists across sessions on the same device and browser. Clearing browser data will reset progress.

---

## Contributing

Found a broken link or outdated resource? Open an issue or submit a pull request. All resource links have been manually validated as of March 2026.

---

## License

This project is for educational use. All linked external resources (YouTube, PDFs, tools) remain the property of their respective owners.
