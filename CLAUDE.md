# Blue Forest — Hello Site

A one-page, Blue Forest–branded "hello" landing page. Everything lives in `index.html`: plain HTML and inline CSS, no JavaScript and no build step.

## Run it

Open `index.html` in a browser. Nothing needs installing or serving.

## Brand

The branding is a placeholder. No official Blue Forest assets have been supplied yet. When real ones arrive (logo, palette, fonts), drop them in this folder and replace the values below and in `index.html`.

**Colors.** These are defined as CSS custom properties on `:root`. Use the tokens and never hard-code new hex values.

| Token     | Hex       | Use                                |
|-----------|-----------|------------------------------------|
| `--night` | `#0b1d2e` | Top of sky gradient, front treeline |
| `--deep`  | `#12324f` | Mid gradient, logo tree, CTA text  |
| `--blue`  | `#1f5f8b` | Bottom of sky gradient             |
| `--sky`   | `#7fb8d9` | Accents, eyebrow text, logo circle |
| `--mist`  | `#e8f1f6` | CTA button background              |
| `--pine`  | `#1d4d3f` | Mid treeline                       |
| `--moss`  | `#3f7d5f` | Secondary green accent             |
| `--text`  | `#f4f8fb` | Primary text                       |
| `--muted` | `#b7cad8` | Body copy, nav, footer             |

**Type**
- Headings and wordmark: **Fraunces** (500/700) from Google Fonts
- Body and UI: **Inter** (400/500/600) from Google Fonts

**Logo.** This is an inline SVG pine tree in a `--sky` circle, followed by the wordmark "Blue Forest". It's a stand-in until the real mark is supplied.

**Voice.** Warm, calm and brief. The nature imagery (roots, sky, forest) should stay light.

## Page structure

1. **Header:** the logo and wordmark on the left, with placeholder nav links (About / Work / Contact). The nav is hidden below 520px.
2. **Hero:** an eyebrow line ("Welcome"), the `h1` "Hello, world." with a gradient on "world.", a one-sentence lede and a pill-shaped "Say hello" button.
3. **Backdrop:** a fixed starfield (CSS radial gradients) and a fixed three-layer SVG forest silhouette pinned to the bottom.
4. **Footer:** a copyright line.

## Conventions

- Keep it a single file and a single page. Don't add frameworks, bundlers or JS unless asked.
- Load external resources only from Google Fonts. Everything else stays inline.
- The page must be responsive down to 320px wide: use a 16px minimum side gutter, never scroll horizontally, and use `clamp()` for fluid type.
- Mark decorative layers (stars, forest) `aria-hidden="true"` and `pointer-events: none`.
- Keep content above the forest by giving it `z-index: 2`. The forest sits at `z-index: 1`.
- After visual changes, check the page in a browser at desktop and mobile widths.

## Repo

- GitHub: https://github.com/chrisnealy3-sys/blue-forest-practice (private)
- Branch: `main`
