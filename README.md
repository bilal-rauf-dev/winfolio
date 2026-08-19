<div align="center">

# 🖥️ AXIOM OS

### An interactive, desktop-style developer portfolio — in a single HTML file

*A lock screen. A login. A boot sequence. A fully click-around desktop.*
*Not a website that describes a developer — a website that behaves like an OS.*

[![Made with HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](#)
[![Made with CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](#)
[![Vanilla JS](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](#)
[![No Framework](https://img.shields.io/badge/dependencies-zero-22c7a0?style=for-the-badge)](#)
[![Single File](https://img.shields.io/badge/build-single--file-5b7cfa?style=for-the-badge)](#)

</div>

---

## ✨ What is this?

**Axiom OS** is a self-contained, single-page portfolio built to look and *feel* like a real operating system — lock screen, sign-in animation, boot sequence, desktop icons, a taskbar, a start menu, widgets, a command palette, and a window manager that lets you drag, resize, minimize, maximize, and snap real "apps."

Every "app" is a window into the same portfolio content — About, Skills, Projects, Experience, Blue Team casework, Résumé, Contact — plus a couple of just-for-fun extras (a working **Terminal** and **Minesweeper**) that make the whole thing feel alive instead of static.

> 🎯 Built for **Bilal Rauf** — Full-Stack Developer & Blue Team security practitioner — but the shell itself is fully data-driven, so it can be re-skinned for anyone.

---

## 🧩 Feature Tour

| 🔐 Lock & Boot | 🪟 Window Manager | 🎨 Personalization |
|---|---|---|
| Live clock lock screen, click-to-sign-in animation, and a short boot sequence before the desktop loads | Draggable, resizable windows with minimize / maximize / close, snapping, and a live task view (`F2`) | 5 wallpapers, accent colors, and a light/dark theme toggle — all saved to `localStorage` |

| 🚀 Start Menu & Search | ⌨️ Command Palette | 📱 Responsive |
|---|---|---|
| A start menu and pinned taskbar for launching apps | `Ctrl/⌘ + K` opens a fuzzy command palette to jump to any app or action | Desktop window chrome gracefully adapts down to mobile layouts |

### 🖼️ The Apps

| App | What it does |
|---|---|
| 👤 **About** | Bio, focus areas, stack, and status ("Open to opportunities") |
| 📊 **Skills** | Animated capability meters grouped by category |
| 📁 **Projects** | Project index with descriptions and live links |
| 💼 **Experience** | Career timeline |
| 🛡️ **Blue Team** | Security casework — malware triage samples, detection engineering notes, incident-report write-ups |
| ⌨️ **Terminal** | A real mini shell — try `help`, `whoami`, `skills`, `projects`, `neofetch`, `theme`, `accent` |
| 🗂️ **Files** | File-explorer-style content browser |
| 📄 **Résumé** | Downloadable CV |
| ✉️ **Contact** | Contact form / links |
| 📝 **Notes** | Simple scratch notes app |
| 🧮 **Calculator** | A working calculator |
| 💣 **Minesweeper** | Yes, really — a fully playable game |
| ⚙️ **Settings** | Theme, wallpaper, accent color, and motion preferences |

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl / ⌘ + K` | Open the command palette |
| `F2` | Toggle task view |
| `Ctrl / ⌘ + W` | Close the active window |
| `Alt + \`` | Cycle between open windows |
| `Esc` | Close whatever panel/palette/menu is open |

---

## 🖥️ Terminal Commands

Open the **Terminal** app and try:

```
help        → list all commands
whoami      → short introduction
skills      → capability summary
projects    → project index
exp         → experience timeline
security    → blue team casework
contact     → how to reach me
open [app]  → launch an application
theme [d|l] → switch appearance
accent [n]  → change accent color
neofetch    → system summary
date        → current date and time
clear       → wipe the screen
```

*Tab completes commands, and ↑ / ↓ walk through your command history — just like a real shell.*

---

## 🚀 Getting Started

No build step, no `npm install`, no framework. It's one HTML file.

```bash
# Clone the repo
git clone https://github.com/bilal-rauf-dev/axiom-os.git
cd axiom-os

# Just open it
open index.html      # macOS
start index.html      # Windows
xdg-open index.html   # Linux
```

Or, for a live-reload dev experience, serve it with anything static:

```bash
npx serve .
# or
python3 -m http.server
```

---

## 🎨 Customize It

Everything content-related lives in a single `PROFILE` object near the top of the script — no need to touch markup or CSS to make it yours.

```js
const PROFILE = {
  name: "Your Name",
  role: "Your Role",
  focus: "What you focus on",
  location: "Your City, Country",
  email: "you@example.com",
  summary: "A short bio...",
  links: { github: "...", linkedin: "..." },
  skills: [ /* ... */ ],
  projects: [ /* ... */ ],
  experience: [ /* ... */ ],
  cases: [ /* blue team write-ups */ ],
};
```

Wallpapers and accent colors are defined the same way, in `WALLS` and `ACCENTS` — add or edit entries and they show up automatically in **Settings**.

---

## 🛠️ Tech Stack

<div align="center">

![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/-Vanilla%20JS-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Google Fonts](https://img.shields.io/badge/-Google%20Fonts-4285F4?style=flat-square&logo=googlefonts&logoColor=white)

</div>

- **Space Grotesk** for display headings
- **Manrope** for UI text
- **JetBrains Mono** for the terminal and numeric/mono content
- Pure CSS custom properties for theming (dark/light + 5 accent-driven wallpapers)
- Zero runtime dependencies — no React, no bundler, no build tools

---

## 📬 Contact

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bilal-rauf-dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bilal-rauf-dev)

</div>

---

<div align="center">

*If Axiom OS boots up cleanly for you, consider dropping a ⭐ on the repo.*

</div>
