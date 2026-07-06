# True 3D Voxel Maze v1.0.0

True 3D Voxel Maze は、ブラウザだけで動作する単体HTML版の「真の立体迷路」アプリです。平面迷路を一人称視点で歩くタイプではなく、立方体状の solid ボクセル空間の中に empty のチューブ状通路を掘り、その中を無重力状態で探索します。

This is a local browser-based true 3D voxel maze app. It generates a tunnel maze inside a solid voxel block and lets the player move through the carved empty cells in six directions.

## Main features

- Single-file local HTML app
- No external libraries and no build step
- Japanese / English UI switch
- Dark theme interface
- True 3D voxel maze model using solid / empty cells
- First-person raycast rendering on HTML Canvas
- Six maze sizes:
  - 3³ rooms / 7³ voxels
  - 4³ rooms / 9³ voxels
  - 5³ rooms / 11³ voxels
  - 6³ rooms / 13³ voxels
  - 7³ rooms / 15³ voxels
  - 8³ rooms / 17³ voxels
- Seed-based random generation
- Extra path percentage embedded in generated seed text
- Extra-path slider from 0% to 30%
- Default extra-path value: 7%
- Six-direction movement in a zero-gravity-style maze
- 90-degree pitch / yaw rotation
- Keyboard and touch/button controls
- Button coloring that shows whether each direction is open or blocked
- 3D cube minimap showing current position, facing direction, goal position, and distance
- Optional visited-cell markers, enabled by default
- Custom wall coloring with Base and Goal colors
- Goal-colored wall gradient based on distance to the goal
- Responsive layout for desktop and narrow screens

## Recommended environment

Recommended:

- Desktop Google Chrome or Microsoft Edge
- A reasonably modern PC or tablet

The app may also run in other modern browsers. Rendering and maze generation are local browser operations, so performance depends on the device.

## Privacy

Maze generation, play state, rendering, and seed handling are processed locally in the browser. This app does not upload maze data or user operations to a server.

When published via GitHub Pages, GitHub only serves the static files. The actual maze generation and play logic run in the user’s browser.

## Files in this repository

- `index.html` — application body
- `README.md` — project overview
- `USER_GUIDE.md` — detailed user guide
- `CHANGELOG.md` — version history
- `RELEASE_REVIEW.md` — release review notes
- `LICENSE` — MIT License

## Basic usage

1. Open `index.html` in a browser.
2. Select a maze size.
3. Set the extra-path slider, from 0% to 30%.
4. Optionally enter a seed.
5. Press **New Maze**.
6. Rotate with arrow keys or the on-screen buttons.
7. Move forward with Space, or backward with Shift + Space.
8. Reach the goal.

## GitHub Pages

For GitHub Pages publication, place `index.html` and the Markdown documents in the repository root. No build step is required.

## License

MIT License. See `LICENSE`.
