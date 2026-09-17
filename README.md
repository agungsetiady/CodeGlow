# CodeGlow — Code Beautifier & Formatter

<img width="1366" height="599" alt="image" src="https://github.com/user-attachments/assets/b2c4dfc9-dc7c-4fef-82c3-6a46ded9c387" />

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

**CodeGlow** is a lightweight, zero-dependency serverless web application designed to format, beautify, and minify multi-language source code instantly. Built with modern web standards and tailored for high performance, CodeGlow transforms messy, unformatted, or minified code into clean, readable, and perfectly structured code in seconds.

---

## 🌟 Overview & Purpose

In daily developer workflows, engineers frequently handle unformatted JSON payloads, inline SQL queries, minified CSS/JS scripts, or messy HTML markup. Existing online tools often come with bloated interfaces, intrusive advertisements, slow server-side response times, or strict privacy concerns due to remote payload processing.

**CodeGlow** was built to solve these problems by providing:
- **100% Client-Side Processing**: All formatting, minification, and comment stripping happen locally in your browser. Your code never hits an external server.
- **Zero Configuration**: Open `index.html` in any browser or deploy instantly on GitHub Pages, Vercel, or Netlify.
- **Instant Productivity**: Clean, modern dual-pane UI with keyboard shortcuts, auto-gutter line tracking, and live statistics.

---

## 💥 Problems Solved

| Problem | How CodeGlow Solves It |
| :--- | :--- |
| **Privacy Risks**: Uploading proprietary or sensitive code to third-party web formatters. | Runs completely on the client side using browser JavaScript engines. No backend servers, logs, or analytics tracking. |
| **Bloated & Slow UI**: Heavy ad-ridden formatters that take time to load and lag during large file inputs. | Uses lightweight native Tailwind styling, dynamic syntax highlighting via `highlight.js`, and fast `js-beautify` processing. |
| **Messy Comment Pollution**: Needing to strip heavy comments, legacy notes, or debug blocks before deploying/sharing. | Integrated AST-aware multi-language comment stripping (`//`, `/* */`, `#`, `<!-- -->`) that protects string literals and regexes. |
| **Broken JSON Debugging**: Opaque JSON error messages when parsing malformed API responses. | Precise line and column error reporting for malformed JSON payloads. |

---

## ✨ Features

- 🎨 **Multi-Language Support**:
  - **Web Markup**: HTML, XML
  - **Stylesheets**: CSS, SCSS, LESS
  - **JavaScript Stack**: JS (ES6+), JSX, TypeScript, JSON
  - **Database & Backend**: SQL (with clause alignment), PHP, Python
  - **Config & Docs**: YAML, Markdown, Shell/Bash
- 🛠️ **Beautify & Minify**:
  - Customizable Indentation: 2, 4, or 8 spaces, or Tab characters.
  - Option to preserve double blank lines or remove all extra spacing.
  - Smart comment stripping (lines, blocks, and docstrings).
  - Compact code minification for Web, JSON, and SQL.
- 🌓 **Themes & UI Polish**:
  - Dark Mode and Light Mode with system preference detection and persistency (`localStorage`).
  - Dual-pane layout (Input vs. Output) with independent word wrap toggles.
  - Panel expansion (focus on input or output only).
  - Real-time line number gutters and character/byte count statistics.
- ⚡ **Developer Utilities**:
  - One-click Code Swap (Output → Input) for iterative processing.
  - Quick sample code loading per language for instant testing.
  - Copy to Clipboard and direct File Download (`.html`, `.json`, `.sql`, etc.).
  - Fullscreen mode support (with browser fallback).
  - Keyboard shortcut: `Ctrl + Enter` / `Cmd + Enter` to trigger Beautify immediately.

---

## 🚀 Quick Start & Usage

Because **CodeGlow** is a static client-side web application, installation takes less than a minute.

### Running Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/agungsetiady/CodeGlow.git
   cd CodeGlow

