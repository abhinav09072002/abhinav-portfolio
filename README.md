# Abhinav Verma — Personal Portfolio Website

A premium, founder-style personal portfolio website with manual dark/light mode toggle, custom cursor, scroll animations, and a full résumé section.

---

## 📁 File Structure

```
abhinav-portfolio/
├── index.html          ← Main website (single file, no build needed)
├── resume.pdf          ← Place your resume PDF here (rename to resume.pdf)
└── README.md           ← This file
```

---

## 🚀 Getting Started

### Option 1 — Open directly in browser
Just double-click `index.html`. Everything works offline except Google Fonts (requires internet for first load).

### Option 2 — Local server (recommended)
```bash
# Python
python -m http.server 8000

# Node.js
npx serve .
```
Then open http://localhost:8000

---

## 🌙 Features

- **Manual Dark / Light mode toggle** — button in top-right nav bar
- **Custom magnetic cursor** — dot + trailing ring (auto-disabled on mobile)
- **Scroll-triggered fade-up animations** — every section reveals on scroll
- **Full Résumé section** — skills, experience, education, certifications, achievements
- **Download Resume button** — links to `resume.pdf` in the same folder
- **Fully responsive** — mobile, tablet, desktop
- **Zero dependencies** — pure HTML/CSS/JS, no frameworks, no build step

---

## ✏️ Customization

### Update your resume PDF
Replace `resume.pdf` in this folder with your actual PDF file (keep the same filename).

### Update links
In `index.html`, search for these placeholders and update:
- `github.com/AbhinavVerma` → your GitHub URL
- `linkedin.com/in/AbhinavVerma` → your LinkedIn URL
- `akv09072002@gmail.com` → your email
- `+91 80907 43945` → your phone

### Change theme default
In the `<script>` section, find:
```js
const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
```
Replace with `let isDark = true;` to always start dark, or `let isDark = false;` for always light.

---

## 🎨 Design System

- **Fonts**: DM Serif Display (headings) + DM Sans (body)
- **Colors**: Monochrome — `#fafaf8` light bg / `#0e0e0c` dark bg
- **Accent**: Inverted button (fg on bg)
- **Spacing**: 7rem section padding, generous whitespace throughout

---

## 🌐 Deployment

**Netlify** (easiest): Drag and drop the `abhinav-portfolio/` folder at netlify.com/drop

**GitHub Pages**:
```bash
git init
git add .
git commit -m "Portfolio"
gh repo create abhinav-portfolio --public --source=. --push
# Enable Pages in repo Settings → Pages → main branch
```

**Vercel**: `npx vercel` in the folder

---

Built with care. No frameworks. No fluff.
