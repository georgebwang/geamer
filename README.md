# Geamer

A minimalist LaTeX Beamer theme designed for academic presentations. Clean typography, restrained colour palette, and sensible defaults so you can focus on content. See the [example PDF](geamer-example.pdf) for a preview.

## Design

### Colour Palette

| Role | Colour | RGB |
|------|--------|-----|
| Primary | Main Blue | 0, 59, 113 |
| Secondary | Grey | 142, 144, 144 |
| Text grey | Dark grey | 60, 60, 60 |
| Background | Off-white | 248, 249, 251 |

A curated set of accent colours (navy, ruby, coral, cranberry, kelly, etc.) is included for plots and highlights.

### Typography

- **Body text:** Roboto Light — a clean sans-serif that reads well on screen
- **Math digits:** Euler (via `eulervm`) — elegant numerals that pair well with sans-serif body text
- **Kerning:** Microtypographic adjustments via `microtype`
- **Line spacing:** 1.2x for readability

### Layout

- **Background:** Subtle off-white (`248, 249, 251`) rather than pure white, reducing harshness under projector lighting
- **Frame titles:** Left-aligned, large, in primary blue. Frame subtitles render inline in italics when present
- **Blocks:** Rounded with backgrounds derived from the primary blue for visual cohesion
- **Lists:** Square bullets (level 1), circles (level 2), arrows (level 3). Natural item spacing is built in — no manual `\vspace` adjustments needed
- **Footer:** Right-aligned short title and page number in dark navy, set at `\footnotesize`
- **Navigation:** Smoothbars section navigation at the top, styled to blend with the background
- **Margins:** 15pt left and right

### Bibliography

- Author-year citation style via `natbib` with round parentheses (BibTeX backend)
- Footnote-sized reference list
- Author names in primary blue, no bibliography icons
- Appendix page numbering resets via `appendixnumberbeamer`

### Convenience Commands

| Command | Description |
|---------|-------------|
| `\mc` | Shorthand for `\multicolumn` |
| `\red{text}` | Red-coloured text |
| `\setfsize` | Captures current font size for use with `\thead` in tables |

## Usage

### Quick Start

Copy `geamer.tex` into your project directory and add to your Beamer preamble:

```latex
\input{geamer.tex}
```

### Persistent Installation

To reuse across projects without copying, store `geamer.tex` in a fixed location and import it:

```latex
\usepackage{import}
\import{/path/to/geamer/}{geamer.tex}
```

**Windows users:** use forward slashes (`/`) in paths, not backslashes (`\`). For example: `\import{C:/Users/xxx/Documents/}{geamer.tex}`.

Alternatively, place it in your local `texmf` directory (e.g., `~/texmf/tex/latex/geamer/`) for automatic discovery by your TeX distribution.
