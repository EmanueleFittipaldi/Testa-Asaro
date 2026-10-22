# Changelog

Versions follow [Semantic Versioning](https://semver.org/): `0.x` during private development, `1.0.0` for the first public release.

## [Unreleased]

## [0.18.0] - 2026-10-23
### Added
- Timed poses tab: duration (30 s, 1, 3, 5, 10, 15 min or custom), number of poses, same model or random models (built-in and uploaded), sound, pause/skip/stop. At every change the view and lights are randomized (at most two lights, moderate intensity). On-screen countdown with controls.
- Shadowbox: three-sided box (back wall, floor, one side wall, left or right) with a chosen color; it receives the model's cast shadows and bounces colored light onto it (spherical-harmonics approximation, adjustable).
### Removed
- Median and posterize filters.

## [0.17.0] - 2026-10-22
### Fixed
- Median strength now grows smoothly along the whole slider: the number of passes used to change at fixed points and made the effect dip slightly before rising again.

## [0.16.0] - 2026-10-22
### Fixed
- The lighting preset matching the current lights is now highlighted, so the app visibly starts with Rembrandt selected; it deselects as soon as you tweak a light.

## [0.15.0] - 2026-10-22
### Changed
- The side panel on Mac, landscape iPad and landscape phones now has the same tabs as the phone sheet (Lights, Material, Environment, Reference, Head and model) to jump straight to a section instead of scrolling.
- Removed the subtitle under the app title.

## [0.14.0] - 2026-10-22
### Changed
- Median is gentler: the slider now spans from subtle to strong in smaller steps.
### Fixed
- Moving the median, posterize or blur sliders now updates the reference image in the side-by-side and stacked layouts live (it only refreshed when toggling a filter before).

## [0.13.0] - 2026-10-22
### Changed
- Median rewritten: 7x7 window with a true median (bisection on luminance), up to 6 passes; much stronger and edge-preserving.
- Posterize rewritten: bands are computed on the real tonal range of the image ("Distribute tones", on by default), with a contour-cleaning slider and anti-aliased band edges.
- Ambient light slider removed: ambient light now comes only from the optional environment image (HDRI). The light estimator no longer fits an ambient term.
### Fixed
- Filters (median, posterize, blur, grayscale) now also apply to the reference image in the side-by-side and stacked layouts, not only in floating mode.

## [0.12.0] - 2026-10-22
### Changed
- Bottom sheet on iPhone and portrait iPad now follows the finger continuously while dragging the grip, then snaps smoothly to peek / half / full (velocity-aware). A tap on the grip still cycles the states.

## [0.11.0] - 2026-10-22
### Added
- Adaptive layout for Mac, iPad and iPhone: on iPhone and portrait iPad the controls live in a bottom sheet (peek / half / full height) with tabs (Lights, Material, Environment, Reference, Head and model); on Mac and landscape iPad the side panel stays, narrower on medium screens, and can be hidden with a button below the zoom controls.
- Landscape phones get a narrow side panel without the title.
- Touch screens: larger buttons, sliders and inputs; text inputs no longer trigger page zoom.

## [0.10.0] - 2026-10-22
### Fixed
- Removed the black gap that appeared after loading a reference image (the page can no longer scroll).

## [0.9.0] - 2026-10-21
### Added
- Estimated light intensity calibrated on the brightness of the reference image; wider sliders (intensity up to 4, ambient up to 150%).
- Presets, materials and settings also saved to the account, not only in the browser.
- HDRI environment lighting: 5 built-in environments, upload of `.hdr`/`.jpg`/`.png` panoramas, strength and rotation, background, key light on the brightest point.
- Model carousel: Asaro head and basic shapes (permanent), uploaded models saved and removable.

## [0.1.0 – 0.8.0]
- Asaro model, orbit view with pan and zoom, lights and presets, materials, filters (median, posterize, blur, value scale), floating and split-screen reference image, pose and light estimation from points on the reference. Files of these versions were not kept.
