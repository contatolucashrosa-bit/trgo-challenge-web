# 🤖 TRGO Challenge

<p align="center">
  <a href="https://github.com/contatolucashrosa-bit/trgo-challenge-web">
    <img src="https://img.shields.io/badge/GitHub-trgo--challenge--web-181717?style=for-the-badge&logo=github">
  </a>
  <a href="https://www.linkedin.com/in/lucas-hochmann-rosa">
    <img src="https://img.shields.io/badge/LinkedIn-Lucas_Hochmann_Rosa-0A66C2?style=for-the-badge&logo=linkedin">
  </a>
  <a href="#-technologies-used">
    <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=111">
  </a>
  <a href="#-technologies-used">
    <img src="https://img.shields.io/badge/Vite-7-646CFF?style=for-the-badge&logo=vite&logoColor=white">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-2ea44f?style=for-the-badge">
  </a>
</p>

<p align="center"><a href="README.md">🇧🇷 Português</a> · 🇺🇸 English</p>

> Interactive math challenges created by Escola SESI Chapecó students for the competitors of **TRGO 2026 — Torneio de Robótica Grande Oeste**.

---

## ⚡ Quick Start

```bash
git clone https://github.com/contatolucashrosa-bit/trgo-challenge-web.git
cd trgo-challenge-web
npm install
npm run dev
```

To build and preview the production version:

```bash
npm run build
npm start
```

---

## 📌 Overview

**TRGO Challenge** is an educational website/game built to entertain and challenge the competitors of **TRGO (Torneio de Robótica Grande Oeste)**, a regional robotics, programming and engineering competition promoted by SESI/SC, held on October 23, 2026 at SENAI Chapecó. After the authors are introduced, the experience takes visitors straight to reasoning challenges in three levels: number sequence, expression building, and logic password.

The project was developed by **Lucas Hochmann Rosa**. **Augusto Belini Gasparetto** and **Maria Paula Rossetti Siqueira** complete the group of Escola SESI Chapecó students running the challenges during the tournament.

---

## ✨ Main Features

- Three challenge modes: easy, medium, and hard.
- Timer with target time per difficulty.
- Answer validation and attempt flow with or without prize eligibility.
- Responsive interface for desktop, tablet, and mobile.
- Sound feedback through the Web Audio API, with a button to enable or disable sounds.
- Visual assets from Escola SESI and the group members.

---

## 🧭 Table of Contents

- [Architecture](#-architecture)
- [Module Map](#-module-map)
- [Technologies used](#-technologies-used)
- [Experience Flow](#-experience-flow)
- [Project Construction Rules](#-project-construction-rules)
- [Requirements](#-requirements)
- [Installation](#-installation)
- [Environment Configuration](#-environment-configuration)
- [Usage](#-usage)
- [Deployment](#-deployment)
- [Disclaimer](#-disclaimer)
- [License](#-license)
- [Author](#-author)

---

## 🏗️ Architecture

```text
trgo-challenge-web/
├── index.html
├── package.json
├── vite.config.js
├── vercel.json
├── public/
│   ├── augusto.png
│   ├── escola-sesi.svg
│   ├── logo-escola-sesi.png
│   ├── lucas.jpg
│   ├── maria.jpg
│   └── math-icons/
│       ├── abaco.png
│       ├── calculadora.png
│       ├── dados.png
│       ├── grafico.png
│       └── operacoes.png
└── src/
    ├── main.jsx
    └── styles.css
```

---

## 🗺️ Module Map

| File | Purpose |
| ------ | ------ |
| `index.html` | HTML entry point and page metadata. |
| `src/main.jsx` | React application, screens, state, and challenge rules. |
| `src/styles.css` | Styles exported from the original experience. |
| `public/` | Images and icons served directly by the browser. |
| `vite.config.js` | Vite configuration, including automatic base path for GitHub Pages. |
| `vercel.json` | Build and output configuration for Vercel deployment. |
| `.github/workflows/deploy-pages.yml` | Automatic GitHub Pages publishing from the `main` branch. |

---

## 🧰 Technologies used

**Interface:** React 19.

**Build:** Vite 7.

**Language:** JavaScript with ES Modules.

**Icons:** Lucide React.

**Audio:** Web Audio API.

---

## 🎲 Experience Flow

The experience starts with the authors' introduction and then unlocks the choice between three difficulty levels:

| Level | Flow | Target time |
| --- | --- | --- |
| Easy | Complete a number sequence. | 30 seconds |
| Medium | Build an expression using every number. | 60 seconds |
| Hard | Solve clues to open a numeric vault. | 90 seconds |

---

## 📐 Project Construction Rules

- Identifiers, functions, states, and file structure are written in English.
- Interface text and documentation are written in Portuguese.
- Code comments are written in Portuguese and reserved for non-obvious decisions - the "why", not the "what".
- The local version preserves the look and flow of the original exported version.
- Development authorship belongs to **Lucas Hochmann Rosa**; the other members appear as part of the presentation group, without code authorship responsibility.

---

## ⚙️ Requirements

- Node.js 24 (LTS)
- npm 10 or newer

---

## 🚀 Installation

```bash
npm install
```

---

## 🔐 Environment Configuration

This project does not use environment variables. The application runs entirely in the browser.

---

## ▶️ Usage

Development server:

```bash
npm run dev
```

Full check:

```bash
npm run check
```

Production build:

```bash
npm run build
npm start
```

---

## 🌐 Deployment

### Vercel

The `vercel.json` file already defines:

| Field | Value |
| --- | --- |
| Build command | `npm run build` |
| Output directory | `dist` |
| Framework | `vite` |

### GitHub Pages

The `.github/workflows/deploy-pages.yml` workflow publishes the `dist` folder when there is a push to the `main` branch.

Expected address after deployment:

```text
https://contatolucashrosa-bit.github.io/trgo-challenge-web/
```

On GitHub, the page should use **GitHub Actions** as the Pages source.

---

## ⚠️ Disclaimer

This project was created for a school presentation and does not represent an official Escola SESI page. It is not an official TRGO page either. Institutional logos and images appear only in the context of the activity presented at TRGO 2026.

The `dist/` directory is generated by the build and should not be committed.

---

## 📄 License

Licensed under MIT. Feel free to use, modify, and distribute, while keeping the copyright notice and crediting **Lucas Hochmann Rosa**.

---

## 👨‍💻 Author

**Lucas Hochmann Rosa**

- Repository: <https://github.com/contatolucashrosa-bit/trgo-challenge-web>
- GitHub: <https://github.com/contatolucashrosa-bit>
- LinkedIn: <https://www.linkedin.com/in/lucas-hochmann-rosa>

Presentation group: Lucas Hochmann Rosa, Augusto Belini Gasparetto, and Maria Paula Rossetti Siqueira.

---
