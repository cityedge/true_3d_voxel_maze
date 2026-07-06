# Changelog

## v1.0.0

### Added

- Initial public release.
- Added local single-file HTML app `True 3D Voxel Maze`.
- Added Japanese / English UI switching.
- Added dark theme UI.
- Added true 3D solid / empty voxel maze model.
- Added first-person Canvas raycast rendering.
- Added six maze sizes:
  - 3³ rooms / 7³ voxels
  - 4³ rooms / 9³ voxels
  - 5³ rooms / 11³ voxels
  - 6³ rooms / 13³ voxels
  - 7³ rooms / 15³ voxels
  - 8³ rooms / 17³ voxels
- Added DFS / recursive backtracker maze generation.
- Added extra-path generation slider from 0% to 30%.
- Added default extra-path value of 7%.
- Added seed encoding that stores the extra-path setting in the seed text.
- Added random seed generation when the seed field is blank.
- Added copyable current seed display.
- Added 90-degree pitch and yaw rotation.
- Added forward and backward movement.
- Added keyboard controls:
  - Arrow keys for rotation
  - Space for forward movement
  - Shift + Space for backward movement
- Added touch/button controls.
- Added direction buttons that show open / blocked status with color.
- Added exploration information panel.
- Added cube minimap showing current position, heading direction, goal position, and distance.
- Added visible goal marker when the goal is in line of sight.
- Added optional visited-cell markers, enabled by default.
- Added simple marker shadow when a floor-like surface exists below the marker.
- Added custom Base / Goal wall coloring.
- Added goal-distance-based wall color blending.
- Added wall brightness adjustment by face orientation.
- Added responsive layout that moves the side panel below the maze on narrow screens.
- Added detailed user guide.
- Added README, CHANGELOG, RELEASE_REVIEW, and MIT LICENSE files.

### Fixed during release preparation

- Removed the central crosshair / plus mark from the maze view.
- Replaced midpoint-only outline visibility checking with two-point visibility checking at 1/3 and 2/3 of each edge, reducing false outline extension from hidden openings.
- Replaced fixed extra-path levels with a 0–30% slider, because the same percentage has different practical impact depending on maze size.
- Tuned visited markers for better readability in straight corridors.

### Notes

- The app is designed around procedural 3D voxel mazes rather than fixed maze maps.
- Seeds are intended for reproduction within the same app version and generator behavior.
- Seed compatibility across future versions is not guaranteed.
- Save data, maze import/export, and score tracking are not included in v1.0.0.
