# nlc_visualizer

Interactive web app to visualize and numerically compute nonlocal curvature of curves in R^3.

## What it does

Computes the nonlocal curvature vector k_s(z) of a parametric curve via Monte Carlo integration over the space of disks, and visualizes the s -> 1 convergence of the rescaled vector k~_s := (1-s)k_s/c_3 to the classical curvature vector (c_3 = pi^2*sqrt(2) ~ 13.96).

Accompanies Dan Zimmerman’s paper "The asymptotics of nonlocal curvature for curves."

## Deploy

Fully static — `index.html` + `assets/`. Serve with any static host:

- Cloudflare Pages: connect this repo, build output directory `/`
- GitHub Pages: Settings -> Pages -> Deploy from branch -> `main`, `/ (root)`
- Or locally: `npx serve .`

Three.js loads from CDN (jsdelivr); all computation runs locally in the browser.
