# HRL X macOS 27 V2.0 — Apple Design System & Liquid Canvas

> Production-grade Apple Human Interface Guidelines (HIG) + macOS 27 Liquid Glassmorphism component library and interactive desktop canvas engineered for HRL International web properties.

---

## 1. Overview

**HRL X macOS 27 V2.0** translates Apple's latest macOS 27 liquid design language into ultra-performant, zero-dependency HTML, CSS, and vanilla JavaScript. It delivers authentic glass physics, parabolic dock magnification, window chrome with operational traffic light controls, Spotlight search, Control Center, and responsive bento grids.

### Key Highlights
- **Authentic Liquid Glassmorphism**: Multi-layer specular lighting, multi-stop backdrop filters (`backdrop-filter: blur(28px) saturate(190%)`), and dynamic border refraction.
- **Apple HIG Color Palette**: Pure macOS system colors (`#0071E3` System Blue, `#34C759` System Green, `#FF3B30` System Red, `#FF9500` System Orange, `#AF52DE` System Purple) harmonized with HRL Signature Crimson (`#D1002D`).
- **Mathematical Parabolic Dock**: Dynamic SVG/icon scaling based on Gaussian distance curves relative to mouse coordinates.
- **Operable Window Chrome**: Authentically styled traffic lights (Close, Minimize, Expand) with hover glyphs, draggable titlebars, and sidebar panes.
- **Zero-Emoji Architecture**: Pure SVG vector glyphs and SF Symbols inspired icon sets for a crisp, enterprise-grade aesthetic.
- **Adaptive Dark / Light Themes**: Native CSS custom properties adhering to Apple system contrast ratios.

---

## 2. Directory Structure

```
HRL-X-MacOS-27-V2.0/
├── assets/
│   ├── icons/             # Apple & system SVG icons
│   ├── wallpapers/        # Liquid glass desktop wallpapers
│   └── logo.png           # HRL Corporate Emblem
├── css/
│   ├── apple-tokens.css   # System variables, color palettes, blur tokens & typography
│   ├── apple-macos-27.css # Reusable Apple UI components (Buttons, Cards, Windows, Bento)
│   └── desktop.css        # macOS 27 Canvas (Menubar, Dock, Spotlight, Control Center)
├── js/
│   └── apple-macos-27.js  # Dock magnification math, window dragging, spotlight & controls
├── index.html             # Interactive desktop showcase & live Component Explorer
└── README.md              # Complete design system & integration guide
```

---

## 3. Quick Start & Integration

Include the stylesheet tokens and script in your existing or new HTML project:

```html
<!-- 1. Apple Tokens & Component Styles -->
<link rel="stylesheet" href="css/apple-tokens.css">
<link rel="stylesheet" href="css/apple-macos-27.css">

<!-- Optional: macOS Desktop Canvas (Dock, Menu Bar, Spotlight) -->
<link rel="stylesheet" href="css/desktop.css">

<!-- 2. Apple Interactive Controller (at end of body) -->
<script src="js/apple-macos-27.js"></script>
```

---

## 4. Component Reference & Snippets

### A. Window Chrome with Traffic Lights

```html
<div class="apple-window" style="width: 600px; height: 400px;">
  <div class="apple-titlebar">
    <div class="apple-traffic-lights">
      <div class="traffic-light close" title="Close"></div>
      <div class="traffic-light minimize" title="Minimize"></div>
      <div class="traffic-light expand" title="Zoom"></div>
    </div>
    <div class="apple-window-title">System Console — HRL Core</div>
    <div style="width: 52px;"></div>
  </div>
  <div class="apple-window-content">
    <p>Window content rendered with authentic frosted liquid glass backdrop.</p>
  </div>
</div>
```

### B. Apple Capsule Buttons

```html
<!-- Primary Apple Blue -->
<button class="apple-btn apple-btn-primary">Get Started</button>

<!-- HRL Signature Crimson -->
<button class="apple-btn apple-btn-crimson">Consult Executive</button>

<!-- Frosted Secondary Glass -->
<button class="apple-btn apple-btn-secondary">Learn More</button>

<!-- Compact Toolbar Button -->
<button class="apple-btn apple-btn-glass apple-btn-sm">Export</button>
```

### C. Bento Grid & Liquid Cards

```html
<div class="apple-bento-grid">
  <!-- Card with Specular Hover Glow -->
  <div class="apple-bento-card bento-span-8">
    <div class="apple-badge">macOS 27 Architecture</div>
    <h3 style="margin-top: 14px; font-size: 24px; font-weight: 600;">Autonomous HRL Core</h3>
    <p style="color: var(--apple-text-secondary); margin-top: 8px;">
      Deep reinforcement learning agent stack running at zero human latency.
    </p>
  </div>
  
  <div class="apple-bento-card bento-span-4">
    <div class="apple-badge">System Status</div>
    <div style="font-size: 36px; font-weight: 700; color: var(--apple-green); margin-top: 14px;">99.98%</div>
    <p style="color: var(--apple-text-secondary); font-size: 13px;">Enterprise SLA Uptime</p>
  </div>
</div>
```

### D. Segmented Controls

```html
<div class="apple-segmented-control">
  <button class="apple-segment-btn active">Overview</button>
  <button class="apple-segment-btn">Architecture</button>
  <button class="apple-segment-btn">Tokens</button>
  <button class="apple-segment-btn">Security</button>
</div>
```

### E. Apple Toggle Switches

```html
<label class="apple-toggle">
  <input type="checkbox" checked id="systemGpuToggle">
  <span class="apple-toggle-slider"></span>
</label>
```

---

## 5. Keyboard Shortcuts

- **⌘ + Space** (or **Ctrl + Space**): Open Spotlight Search
- **Esc**: Dismiss Spotlight Search / Close Active Popups

---

## 6. License & Credits

- Designed for **HRL International** (`hrl-international-website-`).
- Adheres to Apple Human Interface Guidelines and macOS design principles.
