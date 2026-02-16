# Project styles overview

This repository contains the compiled CSS used by the site. The README below summarizes the key variables, major component classes, and a minimal usage example so the CSS in `Main.css` is easy to understand and reuse.

**Files**
- **CSS:** [Main.css](Main.css) — theme variables, component rules, and utility classes.

**Colors & tokens**
- **Primary:** `--main-color` = `#2780e6`
- **Hover:** `--hover-color` = `#1e63b3`
- **Success:** `--success-color` = `#43b581`
- **Danger:** `--danger-color` = `#982929`
- Background and card shading, modal, input shading and other tokens are defined via HSL variables in `:root` and theme selectors.

**Fonts**
- `--main-font`: 'gg sans', Whitney, 'Helvetica Neue', Helvetica, Arial, sans-serif
- `--code-font`: Consolas, 'gg mono', 'Liberation Mono', Menlo, Courier, monospace

**Notable classes (examples)**
- Buttons: `button_a22cb0` with modifiers `primary_a22cb0`, `secondary_a22cb0`, `active_a22cb0`, `critical-primary_a22cb0`.
- Look variants: `lookFilled__201d5`, `lookOutlined__201d5`, `lookLink__201d5` (used with color modifiers like `colorGreen__201d5`).
- Inputs: `wrapper__72c38` (focus outlines use `--hsl-main-color`), `input__0f084` placeholders use `--text-muted`.
- Containers/cards: many `.container_*`, `.card_*`, and `.wrapper_*` classes use `--hsl-card-shading` / `--hsl-popout-shading` tokens.

**Usage (minimal example)**
Include the stylesheet in your HTML and apply classes to elements:

```html
<!doctype html>
<html>
	<head>
		<link rel="stylesheet" href="Main.css">
	</head>
	<body>
		<button class="button_a22cb0 primary_a22cb0">Primary button</button>
		<button class="lookFilled__201d5 colorGreen__201d5">Success</button>
		<div class="wrapper__72c38">
			<input class="input__0f084" placeholder="Type here...">
		</div>
	</body>
</html>
```

**Tips**
- To change the theme colors, override the `--main-color`, `--hover-color`, and related variables (either in `:root` or in theme-specific selectors).
- Use the `look*` variants for semantic buttons and the `wrapper__72c38` / `container_*` classes for inputs and panels to get the correct focus and shading styles.

If you want, I can also:
- add a short visual preview screenshot (if you provide one), or
- convert key class names into a smaller reference table.

**Published URL (GitHub Pages)**

You can import the stylesheet directly from the Pages site:

```html
<link rel="stylesheet" href="https://hropiberhtaz.github.io/main.css">
```

Or via CSS import:

```css
@import url("https://hropiberhtaz.github.io/main.css");
```



