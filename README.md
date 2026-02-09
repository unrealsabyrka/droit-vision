# DroitVision

A landing page for DroitVision (卓特视觉) — a Chinese creative content platform specializing in licensed video, music, image, and vector assets for commercial use.

The website presents the company's services and partnerships, featuring a modern gradient-based design with decorative badges and mesh backgrounds.

## Tech Stack

- **HTML5** — semantic markup
- **CSS3** — modular stylesheets with custom properties
- **No build tools** — vanilla HTML/CSS project
- **Custom fonts** — Ping Fang SC (Regular, Medium, Semibold)

## Project Structure

```
droit-vision/
├── index.html                  # Main HTML file
├── assets/
│   ├── fonts/                  # Ping Fang SC font files (.woff2)
│   ├── icons/                  # SVG icons (logo, arrows, partner icons)
│   └── images/                 # Badge decorations, mesh backgrounds, content images
└── styles/
    ├── main.css                # Entry point (imports all styles)
    ├── base/                   # Foundation styles
    │   ├── fonts.css           # @font-face declarations
    │   ├── variables.css       # CSS custom properties
    │   ├── global.css          # Global element styles
    │   ├── normalize.css       # CSS reset
    │   └── utils.css           # Utility classes
    ├── components/             # Reusable components
    │   └── button.css          # Button styles (md, lg variants)
    └── layout/                 # Page sections
        ├── header.css          # Header with logo and CTA
        ├── hero.css            # Hero section with title and description
        ├── partners.css        # Partners section (3-column grid)
        ├── commercial-assets.css # Asset showcase section
        └── footer.css          # Footer with CTA
```

## How to Run

1. Clone or download the repository
2. Open `index.html` in a web browser

No build process or package installation required.

## Responsive Design

The project uses a mobile-first approach with the following breakpoints:

| Breakpoint | Container Width | Viewport |
|------------|-----------------|----------|
| Desktop    | 1200px          | > 1024px |
| Tablet     | 960px           | ≤ 1024px |
| Mobile     | 100%            | ≤ 768px  |
| Small      | 100%            | ≤ 480px  |

Responsive adjustments include:
- Fluid container width
- Adaptive font sizes (16px → 15px → 14px)
- Dynamic padding (15px → 20px → 16px)
- Button size scaling
- Section spacing adjustments
- Hidden decorative badges on mobile

## CSS Architecture

### Custom Properties (CSS Variables)

Defined in `styles/base/variables.css`:

**Colors:**
- `--color-white`, `--color-white-64` — text colors
- `--color-black`, `--color-black-64` — background colors
- `--color-gradient-accent` — yellow-to-blue gradient (buttons, title accent)
- `--color-gradient-badge-bg` — badge background gradient
- `--color-gradient-stroke-width` — border gradient

**Layout:**
- `--container-width` — responsive container (1200px → 960px → 100%)
- `--container-padding-x` — horizontal padding (15px → 20px → 16px)

**Typography:**
- `--font-family` — 'Ping Fang SC', sans-serif
- `--line-height` — 1.6

**Components:**
- `--button-height-md`, `--button-height-lg` — button sizes
- `--border-radius` — 8px
- `--transition-duration` — 0.4s

### Modular CSS

The project follows a layered CSS structure:

1. **Base** — fonts, resets, variables, global styles
2. **Components** — reusable UI elements (buttons)
3. **Layout** — section-specific styles (header, hero, partners, etc.)

All modules are imported via `styles/main.css`.

## Styling Principles

- **CSS Custom Properties** — for consistent theming and responsive values
- **BEM-like naming** — `.block`, `.block-element`, `.block-element-modifier`
- **Gradient accents** — yellow (#F5E774) to blue (#05A3E7) brand gradient
- **Decorative elements** — badges and mesh backgrounds positioned with pseudo-elements
- **No JavaScript** — pure HTML/CSS implementation
- **Smooth transitions** — 0.4s duration on interactive elements
- **Accessibility** — `.visually-hidden` utility for screen readers

## Page Sections

1. **Header** — Logo and "立即进入" (Enter Now) button
2. **Hero** — Main title with gradient accent, description, CTA button, decorative badges
3. **Partners** — 3-column grid showcasing partnership benefits
4. **Commercial Assets** — 4 content categories (video, images, music, vectors)
5. **Footer** — Partnership message and final CTA

## Language

The content is in **Chinese (Simplified)** with `lang="zh-CN"` attribute.

## Author

Zhaslanuly Sabyrzhan (Sabyrka) <br />
Frontend Developer

- GitHub: [github.com/unrealsabyrka](https://github.com/unrealsabyrka)
- Telegram: [@unrealsabyrka](https://t.me/unrealsabyrka)

## License

This project is for portfolio and demonstration purposes only.
