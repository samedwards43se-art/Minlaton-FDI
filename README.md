# Minlaton GFDI Calculator

A single-page web app that turns a weather observation (temperature, humidity or dew point, wind speed) into a McArthur Grassland Fire Danger Index (GFDI), Mark 4, assuming 100% curing.

## Formula

GFDI = 2 · exp(−23.6 + 5.01·ln C + 0.0281·T − 0.226·√RH + 0.633·√V)

- C = curing (fixed at 100%)
- T = air temperature (°C)
- RH = relative humidity (%)
- V = wind speed (km/h)

## Important notes

- The SA Grain Harvest Code of Practice cease-harvest threshold has been GFDI 35 measured at a 2 m working height, with wind measured at 2 m and not converted. Bureau of Meteorology station wind is measured at 10 m and will usually read higher. Check the current Code, Grain Producers SA and the CFS before making harvest decisions.
- The app does not fetch live data. Copy readings in by hand.
- This is an aid only, not an official tool.

## Run locally

Open `index.html` in a browser. There are no dependencies or build step.

## Host on GitHub Pages

1. Push this repository to GitHub.
2. Go to Settings, then Pages.
3. Under Build and deployment, choose "Deploy from a branch", select `main` and `/ (root)`, then Save.
4. After a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Licence

MIT
