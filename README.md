<div align="center">

# ⏱ Zenith

### *Premium Analog & Digital Timepiece*

**A feature-rich, beautifully designed clock application built with vanilla HTML, CSS, and JavaScript — featuring an analog clock, digital display, stopwatch, countdown timer, world clocks, and a stunning glassmorphic UI.**

<br>

<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
<img src="https://img.shields.io/badge/Zero_Dependencies-22c55e?style=for-the-badge" alt="Zero Dependencies">
<img src="https://img.shields.io/badge/License-MIT-F59E0B?style=for-the-badge" alt="MIT License">

<br><br>

### 🕐 Analog &nbsp;•&nbsp; 🔢 Digital &nbsp;•&nbsp; ⏱ Stopwatch &nbsp;•&nbsp; ⏳ Timer &nbsp;•&nbsp; 🌍 World Clocks

<br>

<img src="https://img.shields.io/badge/Platform-Any_Browser-8b5cf6?style=flat-square" alt="Cross Platform">
<img src="https://img.shields.io/badge/Responsive-Yes-06b6d4?style=flat-square" alt="Responsive">
<img src="https://img.shields.io/badge/Fullscreen_Mode-Supported-ec4899?style=flat-square" alt="Fullscreen">

</div>

---

## 🌟 About The Project

> **Zenith** — the highest point reached, the peak, the moment when the sun is directly overhead.
>
> This clock embodies that idea: **time at its most refined.**

A **single-file**, zero-dependency web application that transforms your browser into a premium timepiece. Designed with a **dark glassmorphic aesthetic**, floating particle network background, and ambient glow effects — it goes far beyond a basic clock demo.

Every feature is **fully functional** — the stopwatch tracks lap splits, the timer plays an alarm, world clocks update live, and all settings apply instantly.

> 💡 **The goal:** *Build the most beautiful and functional browser-based clock — without any frameworks, libraries, or build tools.*

---

## ✨ Feature Showcase

<table>
<tr>
<td width="50%" valign="top">

### 🕐 Analog Clock
- ✅ Precision SVG tick marks (60 minor + 12 major)
- ✅ Glowing hour numbers with highlighted "12"
- ✅ Color-coded hands — **gold** / **cyan** / **red**
- ✅ Counterweight tails on all hands
- ✅ **Smooth mode** (fluid sweep) or **Tick mode** (snap)
- ✅ Pulsing outer ring animation
- ✅ Inner glass reflection effect
- ✅ Dynamically rebuilds on resize

</td>
<td width="50%" valign="top">

### 🔢 Digital Display
- ✅ Large monospaced time readout
- ✅ **12-hour (AM/PM)** or **24-hour** format
- ✅ Full date with weekday
- ✅ Timezone label (auto-detected or manual)
- ✅ Gradient text styling
- ✅ Can be toggled on/off independently

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ⏱ Stopwatch
- ✅ Start / Pause / Resume / Reset
- ✅ **Centisecond precision** (10ms updates)
- ✅ **Lap tracking** with split times
- ✅ Lap diff display (+Δ)
- ✅ Animated lap entry list
- ✅ Live / Paused / Standby status badge
- ✅ Scrollable lap history

</td>
<td width="50%" valign="top">

### ⏳ Countdown Timer
- ✅ Custom **H:M:S** input
- ✅ **Quick presets** — 1m, 3m, 5m, 10m, 15m, 30m
- ✅ Animated **progress bar**
- ✅ **Warning pulse** at 30 seconds (gold)
- ✅ **Danger pulse** at 10 seconds (red)
- ✅ **Melodic alarm** on completion (Web Audio API)
- ✅ Toast notification on finish

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🌍 World Clocks
- ✅ **6 major cities** — New York, London, Dubai, Karachi, Tokyo, Sydney
- ✅ Live-updating times (every second)
- ✅ Country **flag emojis**
- ✅ Offset display from your local timezone
- ✅ Respects your 12h/24h setting
- ✅ Timezone abbreviation labels

</td>
<td width="50%" valign="top">

### ⚙️ Settings Panel
- ✅ **24h / 12h** format toggle
- ✅ **Show / Hide** date
- ✅ **Show / Hide** hour numbers on clock face
- ✅ **Timezone selector** — 12 zones including UTC
- ✅ Custom toggle switches with glow effects
- ✅ All changes apply **instantly**

</td>
</tr>
</table>

---

## 🎨 Visual & UX Features

<details>
<summary><b>🖼️ Interface Design</b></summary>

- **Dark glassmorphic theme** — frosted glass cards with `backdrop-filter: blur()`
- **Ambient floating orbs** — 3 gradient blobs with slow float animation
- **Particle network** — 50 interconnected nodes drifting across the background
- **Consistent design tokens** — all colors via CSS custom properties
- **Poppins + JetBrains Mono** — clean UI font + precise monospace for numbers

</details>

<details>
<summary><b>🔊 Sound System</b></summary>

- **Synthetic tick sound** — generated via Web Audio API oscillator (no external audio files)
- **Timer alarm melody** — 4-note ascending chime (C5 → E5 → G5 → C6)
- **Toggle on/off** from the top bar
- Only works in tick mode (smooth mode has no audible ticks)
- Audio context initializes on first user click (browser autoplay policy)

</details>

<details>
<summary><b>⛶ Fullscreen Mode</b></summary>

- Strips the top bar and side panel
- Clock scales to **80% of viewport** (up to 600px)
- Hands scale proportionally using `calc()` with CSS variable
- Digital time enlarges for readability
- Perfect for **desk display** or **presentation mode**
- Toggle with the fullscreen button in the top bar

</details>

<details>
<summary><b>📱 Responsive Design</b></summary>

- **Desktop** (>860px) — side-by-side layout: clock + panel
- **Tablet** (≤860px) — stacks vertically, panel goes full width
- **Mobile** (≤400px) — clock shrinks to 240px, smaller fonts
- Clock face **rebuilds SVG markers** on resize for pixel-perfect rendering
- All controls remain accessible at every breakpoint

</details>

<details>
<summary><b>🔔 Toast Notifications</b></summary>

- Non-intrusive slide-in from the right
- 3 types: `success` (green), `info` (cyan), `warning` (gold)
- Auto-dismiss after 3 seconds with fade-out animation
- Used for: sound toggle, smooth/tick switch, timezone changes, timer completion

</details>

---

## 🧩 Architecture

```
zenith/
│
└── 📄 index.html          ← Everything in one file
    │
    ├── <style>            ← 500+ lines of CSS
    │   ├── CSS Variables (design tokens)
    │   ├── Ambient background & particles
    │   ├── Clock face, hands, markers
    │   ├── Digital display
    │   ├── Cards & side panel
    │   ├── Stopwatch, Timer, World Clocks
    │   ├── Settings (toggles, selects)
    │   ├── Toast notifications
    │   ├── Fullscreen mode
    │   └── Responsive breakpoints
    │
    ├── <script>           ← 400+ lines of vanilla JS
    │   ├── State management (single object)
    │   ├── Clock face builder (dynamic SVG)
    │   ├── Clock update loop (requestAnimationFrame)
    │   ├── Stopwatch engine (performance.now precision)
    │   ├── Timer engine (setInterval + alarm)
    │   ├── World clocks (Intl API)
    │   ├── Particle system (Canvas 2D)
    │   ├── Sound engine (Web Audio API)
    │   ├── Toast system
    │   └── Settings & control wiring
    │
    └── No external files, no CDN, no build step
```

### Key Technical Decisions

| Decision | Reason |
|:---------|:-------|
| **Single file** | Zero setup — open in any browser instantly |
| **`requestAnimationFrame`** for clock | 60fps smooth second hand, no jank |
| **`performance.now()`** for stopwatch | Sub-millisecond precision, immune to clock drift |
| **Web Audio API** for sounds | No external audio files, synthetic generation |
| **CSS Custom Properties** | Consistent theming, easy to reskin |
| **Dynamic SVG markers** | Pixel-perfect at any clock size |
| **Canvas particles** | GPU-accelerated, smooth 60fps animation |
| **Intl.DateTimeFormat** | Timezone-aware time without any library |

---

## 🚀 Getting Started

### Option 1 — Just Open It

```bash
# Clone the repository
git clone https://github.com/abdulbasit-25/zenith.git

# Open in your browser
# macOS
open zenith/index.html

# Windows
start zenith/index.html

# Linux
xdg-open zenith/index.html
```

### Option 2 — Local Server (for best experience)

```bash
# Using Python
cd zenith
python3 -m http.server 8000
# → http://localhost:8000

# Using Node.js (npx)
npx serve .
# → http://localhost:3000

# Using PHP
php -S localhost:8000
```

> ⚠️ A local server is recommended for the **best experience**, though the file works perfectly when opened directly.

---

## ⚙️ Technologies

<div align="center">

| Technology | Purpose |
|:-----------|:--------|
| **HTML5** | Structure & semantic markup |
| **CSS3** | Styling, animations, glassmorphism, responsiveness |
| **JavaScript (ES6+)** | All logic, DOM manipulation, state management |
| **Web Audio API** | Synthetic tick & alarm sounds |
| **Canvas 2D** | Particle network background |
| **Intl API** | Timezone-aware date/time formatting |
| **CSS Custom Properties** | Design token system |
| **SVG (dynamic)** | Clock face tick marks |
| **requestAnimationFrame** | 60fps rendering loop |

</div>

### 📚 Browser Compatibility

| Browser | Status |
|:--------|:-------|
| Chrome 80+ | ✅ Full Support |
| Firefox 80+ | ✅ Full Support |
| Safari 14+ | ✅ Full Support |
| Edge 80+ | ✅ Full Support |
| Mobile Chrome | ✅ Full Support |
| Mobile Safari | ✅ Full Support |

---

## 📸 Feature Preview

### Clock Modes

```
┌─────────────────────────────┐     ┌─────────────────────────────┐
│   ⚡ SMOOTH MODE (default)  │     │   🔄 TICK MODE             │
│                             │     │                             │
│     Second hand sweeps      │     │     Second hand snaps       │
│     continuously at 60fps   │     │     each second with a      │
│     — fluid, silent         │     │     satisfying bounce       │
│                             │     │     — audible tick optional │
└─────────────────────────────┘     └─────────────────────────────┘
```

### Stopwatch Flow

```
[Standby] ──▶ Start ──▶ [Running] ──▶ Pause ──▶ [Paused] ──▶ Resume ──▶ [Running]
                  │                          │
                  │                          ├──▶ Lap (saves split)
                  │                          │
                  │                          └──▶ Reset ──▶ [Standby]
                  │
                  └──▶ Lap (saves split)
```

### Timer Flow

```
[Stopped] ──▶ Start ──▶ [Running] ──▶ 0:00 ──▶ [Done! + Alarm + Toast]
                  │               │
                  ├──▶ Pause ──▶ [Paused] ──▶ Resume
                  │
                  └──▶ (auto-pauses inputs)
```

---

## 🔮 Roadmap

<details>
<summary><b>🎨 Visual Enhancements</b></summary>

- 🔹 Multiple **color themes** (light, dark, midnight, ocean, sunset)
- 🔹 **Custom clock face styles** (minimal, roman numerals, dots-only)
- 🔹 Hand style options (classic, modern, skeleton)
- 🔹 Background pattern options (particles, stars, gradient, solid)

</details>

<details>
<summary><b>⏱ Stopwatch Enhancements</b></summary>

- 🔹 **Fastest / Slowest / Average** lap highlighting
- 🔹 Lap **delete** individual entries
- 🔹 **Export** laps as CSV
- 🔹 Countdown mode (count down from a set time)

</details>

<details>
<summary><b>⏳ Timer Enhancements</b></summary>

- 🔹 **Multiple simultaneous** timers
- 🔹 **Repeat** mode (auto-restart after completion)
- 🔹 Custom **alarm sound** selection
- 🔹 Timer **name labels**

</details>

<details>
<summary><b>🌍 World Clocks</b></summary>

- 🔹 **Add/remove** custom cities
- 🔹 Drag to **reorder**
- 🔹 Day/night **indicator** (☀️/🌙)
- 🔹 Show **date** for each city

</details>

<details>
<summary><b>💾 Persistence & Data</b></summary>

- 🔹 **LocalStorage** for settings persistence
- 🔹 Remember last used **timer duration**
- 🔹 Save **stopwatch sessions**
- 🔹 **Export/Import** all settings

</details>

<details>
<summary><b>🔧 Technical</b></summary>

- 🔹 **PWA support** (installable, offline)
- 🔹 **Keyboard shortcuts** (Space = start/pause, L = lap, R = reset, F = fullscreen)
- 🔹 **Web Worker** for particle system
- 🔹 **Reduced motion** media query support

</details>

---

## 📊 Project Stats

<div align="center">

| Metric | Value |
|:-------|:------|
| **Total Lines** | ~1,000+ |
| **External Dependencies** | 0 |
| **External CDNs** | 0 (Google Fonts optional) |
| **Build Step Required** | No |
| **Minimum Browser** | Chrome 80 / Firefox 80 / Safari 14 |
| **File Size** | ~25 KB (uncompressed) |

</div>

---

## ⚠️ Project Status

<div align="center">

### 🟢 Stable / Active Development

*Zenith is fully functional and ready for daily use. New features are being actively developed.*

</div>

---

## 🤝 Contributing

Contributions, suggestions, and improvements are **welcome**.

### How to Contribute

```bash
# 1. Fork the repository

# 2. Create a feature branch
git checkout -b feature/my-feature

# 3. Make your changes
#    (remember: everything stays in one file!)

# 4. Commit with a clear message
git commit -m "Add dark theme toggle"

# 5. Push to your fork
git push origin feature/my-feature

# 6. Open a Pull Request
```

> 💡 **Areas where contributions are especially welcome:**
> - 🎨 New color themes
> - ⌨️ Keyboard shortcuts
> - 📱 Further mobile optimizations
> - 🧪 Cross-browser testing
> - 🌍 Additional world clock cities
> - ♿ Accessibility improvements

---

## 📜 License

This project is licensed under the **MIT License**.

See the [`LICENSE`](LICENSE) file for complete license information.

---

## 👨‍💻 Author

<div align="center">

<br>

### **Abdul Basit**

*Frontend Developer • C++ Enthusiast • Software Engineering Student*

<br>

<table>
<tr>
<td align="center" width="120">

📧 **Email**

</td>
<td align="center" width="120">

🌐 **Portfolio**

</td>
<td align="center" width="120">

🐙 **GitHub**

</td>
</tr>
<tr>
<td align="center">

[abdulbasit.alpha25@gmail.com](mailto:abdulbasit.alpha25@gmail.com)

</td>
<td align="center">

[abdulbasit-archer.vercel.app](https://abdulbasit-archer.vercel.app/)

</td>
<td align="center">

[@abdulbasit-25](https://github.com/abdulbasit-25)

</td>
</tr>
</table>

<br>

**My Projects:**

| Project | Description |
|:--------|:------------|
| [🤖 R.A.Y.N](https://github.com/abdulbasit-25/rayn-oop-chatbot) | C++ OOP console chatbot with MathBot, file handling & admin system |
| [⏱ Zenith](https://github.com/abdulbasit-25/zenith) | Premium analog & digital clock — stopwatch, timer, world clocks |

<br>

</div>

---

<div align="center">

## ⭐ Support The Project

If Zenith made your browser tab a little more beautiful:

<br>

[⭐ Star](https://github.com/abdulbasit-25/zenith/stargazers) &nbsp;&nbsp;•&nbsp;&nbsp;
[🍴 Fork](https://github.com/abdulbasit-25/zenith/fork) &nbsp;&nbsp;•&nbsp;&nbsp;
[🐛 Report Issues](https://github.com/abdulbasit-25/zenith/issues) &nbsp;&nbsp;•&nbsp;&nbsp;
[💡 Suggest Features](https://github.com/abdulbasit-25/zenith/issues) &nbsp;&nbsp;•&nbsp;&nbsp;
[🤝 Contribute](https://github.com/abdulbasit-25/zenith/pulls)

<br><br>

---

# ⏱ Zenith

### *Premium Analog & Digital Timepiece*

**Built with vanilla HTML, CSS & JavaScript ❤️**

`Zero Dependencies` • `Single File` • `Glassmorphic UI` • `60fps`

<br>

*Thank you for visiting the project!*

</div>
