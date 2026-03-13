<p align="center">
  <h1 align="center">Noteriv Themes</h1>
  <p align="center">
    Community themes for <a href="https://noteriv.com">Noteriv</a> — a modern markdown editor.
    <br />
    <a href="#installing">Install</a> · <a href="#creating-a-theme">Create your own</a> · <a href="#contributing">Contribute</a>
  </p>
</p>

<br />

## Themes

### Dark

| Preview | Theme | Description |
|---|---|---|
| ![#0f1923](https://placehold.co/24x24/0f1923/0f1923) ![#e8764d](https://placehold.co/24x24/e8764d/e8764d) | **Midnight Ember** by Jace Sleeman | Deep midnight blues with warm ember accents |
| ![#1a2118](https://placehold.co/24x24/1a2118/1a2118) ![#8cbf6e](https://placehold.co/24x24/8cbf6e/8cbf6e) | **Moss Garden** by Jace Sleeman | Earthy forest greens with natural warmth |
| ![#0a0a12](https://placehold.co/24x24/0a0a12/0a0a12) ![#00e5ff](https://placehold.co/24x24/00e5ff/00e5ff) | **Cyber Neon** by Jace Sleeman | High contrast cyberpunk with neon glows |
| ![#232136](https://placehold.co/24x24/232136/232136) ![#c4a7e7](https://placehold.co/24x24/c4a7e7/c4a7e7) | **Rose Pine Moon** by Community | Soft purple moon tones inspired by Rose Pine |
| ![#1f1520](https://placehold.co/24x24/1f1520/1f1520) ![#e88a6a](https://placehold.co/24x24/e88a6a/e88a6a) | **Sunset Haze** by Community | Warm sunset gradients with dusky purple undertones |
| ![#1c1816](https://placehold.co/24x24/1c1816/1c1816) ![#c4883c](https://placehold.co/24x24/c4883c/c4883c) | **Espresso** by Community | Rich coffee-inspired warm dark theme |

### Light

| Preview | Theme | Description |
|---|---|---|
| ![#f0f4f8](https://placehold.co/24x24/f0f4f8/f0f4f8) ![#2563eb](https://placehold.co/24x24/2563eb/2563eb) | **Arctic Frost** by Community | Icy cool light theme with crisp blues |
| ![#faf8f5](https://placehold.co/24x24/faf8f5/faf8f5) ![#1a6b4e](https://placehold.co/24x24/1a6b4e/1a6b4e) | **Paper & Ink** by Community | Clean minimal theme like pen on paper |

<br />

---

<br />

## Installing

1. Download a `.json` theme file from the [`themes/`](./themes) folder
2. Drop it into your vault at `.noteriv/themes/`
3. Open **Settings > Appearance > Theme** and select it

> Noteriv ships with 10 built-in themes. These community themes are extras you can add on top.

<br />

## Creating a Theme

A theme is a single `.json` file. Here's the full structure:

```jsonc
{
  "id": "my-theme",          // unique, lowercase, kebab-case
  "name": "My Theme",        // display name
  "author": "Your Name",
  "version": "1.0.0",
  "description": "Short description of the vibe",

  "colors": {
    // ── Backgrounds ──
    "bgPrimary":      "#1e1e2e",   // main editor
    "bgSecondary":    "#181825",   // sidebar, status bar
    "bgTertiary":     "#313244",   // hover, inputs

    // ── Borders ──
    "border":         "#45475a",

    // ── Text ──
    "textPrimary":    "#cdd6f4",   // main text
    "textSecondary":  "#bac2de",   // slightly dimmed
    "textMuted":      "#6c7086",   // placeholders, hints

    // ── Accent ──
    "accent":         "#89b4fa",   // links, active states, buttons

    // ── Semantic ──
    "green":          "#a6e3a1",   // success, saved
    "red":            "#f38ba8",   // errors, deletions
    "yellow":         "#f9e2af",   // warnings, unsaved
    "blue":           "#89b4fa",   // info
    "mauve":          "#cba6f7",   // tags, special elements
    "peach":          "#fab387",   // secondary highlights
    "teal":           "#94e2d5",   // tertiary highlights
    "pink":           "#f5c2e7",   // decorative accents

    // ── Scrollbar ──
    "scrollbar":      "#45475a",
    "scrollbarHover": "#585b70"
  }
}
```

<br />

## Contributing

1. **Fork** this repo
2. Add your theme `.json` to `themes/`
3. Update `manifest.json` with your theme entry
4. Open a **PR** — include a screenshot so people can preview it

### Guidelines

- Use a unique `id` that doesn't conflict with built-in themes
- Test your theme in Noteriv before submitting
- Make sure text is readable against all background colors
- Include both a clear `name` and `description`

<br />

---

<p align="center">
  Made for <a href="https://noteriv.com">Noteriv</a>
</p>
