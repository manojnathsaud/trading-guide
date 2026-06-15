# 📈 Trading Guide

A static, multi-page educational website covering the fundamentals through advanced
concepts of technical trading. Built with plain HTML and a shared CSS stylesheet using
a dark, GitHub-inspired theme — no build step or JavaScript framework required.

> ⚠️ **Disclaimer:** This guide is for educational purposes only. Trading involves risk.
> Always do your own research before making any financial decisions.

## 📚 Contents

| Page | Topic |
|------|-------|
| [Home](index.html) | Chapter overview and navigation |
| [Page 1](TradingGuidePage1/TradingGuidePage1.html) | Trading Foundations |
| [Page 2](TradingGuidePage2/TradingGuidePage2.html) | Professional Trading System |
| [Page 3](TradingGuidePage3/TradingGuidePage3.html) | Institutional Price Action Strategy |
| [Page 4](TradingGuidePage4/TradingGuidePage4.html) | The 4-Candle Reversal Setup |
| [Page 5](TradingGuidePage5/TradingGuidePage5.html) | The 7 Phases of a Market Cycle |
| [Page 6](TradingGuidePage6/TradingGuidePage6.html) | Power of 3 (PO3) Trading Model |
| [Page 7](TradingGuidePage7/TradingGuidePage7.html) | Complete Trading Strategies & Case Studies |

## 🗂️ Project Structure

```
.
├── index.html                      # Home page with the chapter grid
├── styles.css                      # Shared dark-theme stylesheet
├── TradingGuidePage1/
│   ├── TradingGuidePage1.html
│   └── images/                     # Page-specific images
├── TradingGuidePage2/
│   ├── TradingGuidePage2.html
│   └── images/
└── ...                             # Pages 3–7 follow the same pattern
```

Each chapter lives in its own folder alongside a sibling `images/` folder. Pages
reference their own images with relative paths like `src="images/<name>"`, and link to
shared assets (such as `styles.css`) and other pages using a `../` prefix.

## 🚀 Running Locally

Because the site is fully static, you can open `index.html` directly in a browser.
To serve it over HTTP (recommended so all relative paths resolve exactly as on GitHub
Pages), run a simple static server from the repository root:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000> in your browser.

## 🤝 Conventions

- Keep image filenames URL-safe: lowercase, hyphenated, no spaces or special characters.
- Place each page's images inside that page's own `images/` folder.
- Add images near the top of a `.section-card`, right after its `<h2>`, with a
  descriptive `alt` attribute.