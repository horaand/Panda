# CSS Panda (HTML + CSS)

A tiny demo that draws a panda face with a blinking animation using pure HTML/CSS.

## Project Structure
panda/
├─ index.html
└─ style.css

## Quick Start
1. Put the HTML into `index.html` and the CSS into `style.css`.
2. Ensure this line is in the `<head>` of `index.html`:
   <link rel="stylesheet" href="style.css">
3. Open `index.html` in your browser.

## Customize
- Size: edit `.panda { width: 200px; height: 200px; }`
- Background: edit `body { background: #f2f2f2; }`
- Blink speed: change `.eyeball { animation: blink 3s infinite; }` (e.g., `2s`)
- Face ring: tweak `.panda { box-shadow: 0 0 0 10px #000; }`

## How It Works
- Centering via flexbox on `body` (`display:flex; justify-content:center; align-items:center; height:100vh; margin:0;`)
- Circles/ovals via `border-radius:50%`
- Blink via `@keyframes blink` scaling the `.eyeball` on Y
- Nose centered with `left:50%` + `transform: translateX(-50%)`

## Troubleshooting
- No styles? Check the `style.css` path.
- Not centered? Keep `height:100vh; margin:0;` on `body`.
- Animation not running? Ensure `animation: blink ...` matches `@keyframes blink`.
