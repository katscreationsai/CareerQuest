# ⚔️ CareerQuest: 16-Bit Edition

> **Level Up Your Professional Journey.**
> *A retro-styled, gamified career management interface built with modern web technologies.* 

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Status](https://img.shields.io/badge/status-stable-green.svg) ![Style](https://img.shields.io/badge/style-Pixel%20Art-purple.svg)

## 📖 Overview

**CareerQuest: 16-Bit Edition** reimagines the mundane task of career planning and job tracking as an immersive, retro RPG experience. By leveraging the aesthetic of 90s console gaming—complete with CRT scanlines, pixel-perfect typography, and 8-bit UI components—this application transforms professional development into an engaging adventure.

Designed as a lightweight, single-file application, it combines the nostalgia of the 16-bit era with the responsiveness of modern CSS frameworks.

## ✨ Key Features

*   **Immersive Retro UX**: Authentic CRT scanline overlays, scan-lines, and phosphor glow effects simulated purely via CSS gradients.
*   **Pixel-Perfect Typography**: Integrated `Press Start 2P` and `VT323` fonts for that authentic arcade cabinet feel.
*   **Responsive Gamified UI**: A mobile-responsive layout powered by **Tailwind CSS**, ensuring the game looks good on any device viewport.
*   **Themable Architecture**: Centralized CSS variables for easy palette swapping (currently configured for a 'Dark Sci-Fi' theme).
*   **Interactive Components**: Custom-styled 'Pixel Inputs' and 'Pixel Buttons' with distinct hover and active states that mimic physical arcade controls.

## 🏗 Architecture

CareerQuest utilizes a **Zero-Build Frontend Architecture**. It is designed for portability and ease of use, relying on CDN-delivered assets to function immediately without a complex compilation step.

*   **Structure**: Monolithic HTML Entry Point (`careerquest_16_bit_edition_1.html`) containing structural markup, stylistic logic, and interactive scripts.
*   **Styling Strategy**: Hybrid approach using **Tailwind CSS** for layout/utility and custom **CSS3** for specific pixel-art aesthetic overrides.
*   **State Management**: (Implied) Browser-based DOM manipulation.

## 🛠️ Technical Stack

*   **Core**: HTML5, Vanilla JavaScript
*   **Styling**: 
    *   [Tailwind CSS](https://tailwindcss.com/) (Layout & Utility)
    *   CSS3 Variables (Theming)
*   **Typography**: Google Fonts (`Press Start 2P`, `VT323`)
*   **Icons**: [Lucide Icons](https://lucide.dev/)

## 🚀 Prerequisites & Installation

Since this project uses a standard web technology stack with CDN links, no package manager (npm/yarn) is strictly required to run the application.

### Quick Start

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/your-username/careerquest-16bit.git
    ```
2.  **Launch**
    Simply double-click `careerquest_16_bit_edition_1.html` to open it in your default web browser.

### For Developers (Optional)
If you wish to modify the code, we recommend serving it via a local server to avoid local file restrictions:

```bash
# Using Python
python3 -m http.server 8000

# Using Node's http-server
npx http-server .
```
Then navigate to `http://localhost:8000/careerquest_16_bit_edition_1.html`.

## 💻 Usage Guide

### Customizing the Theme
The visual palette is controlled entirely by CSS variables in the `:root` scope. You can modify these in the `<style>` block to create new "skins" (e.g., Green Monochrome, Cyberpunk Pink).

```css
:root {
    /* Change these hex codes to re-skin the app */
    --bg-color: #202028;       /* Main background */
    --card-bg: #2d2d38;        /* Container background */
    --accent: #50b5ff;         /* Primary highlight */
    --text-main: #ffffff;      /* Text color */
}
```

## 🗺️ Roadmap

*   [ ] **Save States**: Implementation of `localStorage` to persist career data between sessions.
*   [ ] **Quest Log**: A kanban-style board for tracking job applications.
*   [ ] **Skill Tree**: A visualization of acquired professional skills.
*   [ ] **Audio**: Optional 8-bit background music and sound effects on interaction.

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a Pull Request. Ensure all new UI elements adhere to the **Pixel Box** styling guidelines defined in the CSS.
