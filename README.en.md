# Graphix

Plot functions and change their parameters live: move around, zoom, read values, and let the app find zeros, extremums and intersections.

*Version française : [README.md](README.md)*

![Graphix](screenshots/1.jpg)

## Phone version

- The graph is on top, functions and sliders below.
- Drag one finger to move around, **pinch with two fingers** to zoom (or the − and + buttons).
- Exported files are saved to the phone's Downloads/NeoDex folder.
- The same functions as on PC (same id `neodex.graphix`).

## Write a function

Up to **6 functions** (f, g, h…), each with its colour; a click on the colour square shows or hides it. Writing is natural:

- `2x`, `3sin(x)`, `(x+1)(x-1)`: multiplication can be implied;
- `x^2`, `x²`, `x³`, `|x|`, `sin x`, `2,5` (decimal comma) or `2.5`;
- functions `sin cos tan asin acos atan sinh cosh tanh sqrt abs ln log exp floor ceil round sign min max mod`, constants `pi` (or `π`) and `e`.

A mistake is underlined in red, and the tooltip says what's wrong. Expressions are read by a small home-made parser: nothing is run as code.

## Parameters

Sliders **a**, **b** and **c** (from -10 to 10, or a typed value) change the curves live. **t** is time: ▶ animates it, to watch `sin(x + t)` move.

## The view

- **Drag** to move, **wheel** to zoom around the mouse, **⌂** to go back to the centre.
- **Hover** shows x and the value of each function.
- **Dotted derivatives** adds each curve's derivative.
- Gaps and asymptotes (`1/x`, `tan x`) are not joined.
- **Export as PNG** saves the graph image.

## Key points and table

- **Key points**: zeros, minimums, maximums and intersections in the visible area (marked with a white square); a click centres the view on it.
- **Table of values**: x and each function, at the grid step.

## Data

Functions, sliders and view are kept in the plugin's folder. Permission: `storage` only.

## Sequences, scatter plots, area and 3D

- **Sequence**: write with `n` (`n^2/10`), or `1 ; u*1.1` (u0 = 1, each term = previous × 1.1).
- **Scatter plot**: `(1;2) (2;3.5) (4;7)`, with its dashed least-squares trend line, equation and r.
- **Area under the curve**: shades the area between a curve and the x axis and gives the integral; bounds accept `pi/2`.
- **3D**: an expression with `x` and `y` (`sin(x)*cos(y)`) switches to 3D. Drag to rotate, wheel to zoom.
