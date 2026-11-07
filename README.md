# Diwali sky lanterns in pure HTML + CSS · Day 12 of 100

A night sky full of rising, swaying Diwali lanterns (kandil), a glowing moon,
twinkling stars and a row of diyas with flickering flames, then a gold
"Happy Diwali" reveal. One file. Only HTML and CSS keyframes: no JavaScript,
no canvas, no libraries.

## Run it

Open `index.html` in any modern browser (Chrome 125+ for the CSS `mod()` maths).

## How it works

- 28 lanterns are the same `<i>` element. A single custom property `--i`
  drives their position, size, speed and sway through `mod()` in `calc()`.
- `rise` moves each lantern up with the `translate` property, `sway` rocks it
  with `transform`, `flick` makes the inner flame breathe.
- The stars are two tiled `radial-gradient` layers that twinkle out of phase.
- The diyas are `<b>` elements; their flames are `::before` with a skew + scale loop.
- The gold text reveals with a `clip-path` keyframe, then pulses its glow.

Files:
- `index.html`: the whole animation
- `preview.jpg`: the finished frame

Made by @hack.n.code, Day 12 of 100.
