# Styling Guide: Slide Design System

This document outlines the visual design system used across the "Claude Code for Non-Coders" interactive slides. It ensures consistency when creating new slides or updating existing ones.

---

## 🎨 Color Palette

### Base Colors (Shared)
*   **Background (`--bg`):** `#0A0A0A` (Deep Black)
*   **Secondary BG (`--bg2`):** `#111111`
*   **Tertiary BG (`--bg3`):** `#161616`
*   **Primary Text (`--white`):** `#F5F0E8` (Off-white/Cream)
*   **Dimmed Text (`--dim`):** `rgba(245,240,232,0.35)`
*   **UI Border (`--border`):** `rgba(245,240,232,0.08)`

### Functional Colors (Shared)
*   **Warning/Action (`--yellow`):** `#FFD93D`
*   **Primary Accent (`--orange`):** `#FF6B35`
*   **Error/Danger (`--red`):** `#E63946`
*   **Success/Growth (`--green`):** `#5CB87E`

### Module-Specific Accents
Each module uses a unique primary accent color for its labels and highlights:
*   **Module 01:** Orange (`#FF6B35`)
*   **Module 02:** Teal (`#4BBFB3`)
*   **Module 03:** Purple (`#9B8FE8`)
*   **Module 04:** Amber/Gold (`#C8A96E`)

---

## 🔠 Typography

### Fonts
*   **Headlines (`.display`, `.headline`):** `'Bebas Neue', sans-serif`
    *   Characterized by all-caps, condensed, high-impact look.
*   **Body Text (`body`, `.subhead`):** `'Barlow Condensed', sans-serif`
    *   Weight 300 for subheads, 600 for emphasis.
*   **Code/Meta (`.label`, `.mono`):** `'JetBrains Mono', monospace`
    *   Used for slide numbers, labels, and terminal simulations.

---

## 📐 Layout System

### Slide Structure
*   **Container:** Every slide uses a `.slide` class, absolutely positioned inside a `.deck`.
*   **Active State:** `.slide.active` sets opacity to 1.
*   **Padding:** Standardized at `60px 96px` (or similar) to ensure readability on screen shares.

### Key Components
*   **`.label`:** Small, uppercase, tracked-out text at the top of a slide.
*   **`.highlight`:** A yellow-bordered box for core summaries.
*   **`.agenda-list`:** A vertical list showing course progress.
*   **`.browser` / `.claude-layout`:** Specialized CSS used in Module 01 to simulate the Claude interface.

---

## 🛠️ Implementation Notes
*   **Responsiveness:** Fluid typography is achieved using `clamp()` (e.g., `font-size: clamp(44px, 6vw, 88px)`).
*   **Gradients:** Slides often use a subtle radial gradient background to create depth: `radial-gradient(ellipse 70% 50% at 75% 50%, rgba(ACCENT_COLOR, 0.04) 0%, transparent 70%)`.
