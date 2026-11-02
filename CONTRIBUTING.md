# Contributing

Thanks for helping improve termfolio.

## Quick start

1. Fork the repo and create a branch: `git checkout -b my-change`.
2. Edit `index.html`. Everything lives in this one file, so there is no build step.
3. Open it in a browser and test every option you touched.
4. Open a pull request and describe what changed, with a screenshot if it is visual.

## Adding a new pixel-art style

Pixel art lives in the `ARTS` object inside the script. Each style is a list of frames, and each frame is a list of strings where `#` is filled and `.` is empty.

1. Add your frames to `ARTS` (2 frames gives the best animation).
2. Add an `<option>` for it in the **Animated art** dropdown.
3. Keep grids under 14×14 so they fit the terminal card.

## Guidelines

- Keep the app dependency-free and fully client-side.
- Escape any user text that ends up in the SVG.
- Keep the SVG output ASCII-only (the generator converts other characters to entities).
