# Testa Asaro — 3D Asaro head lighting reference for artists

**A free web app for drawing and painting students: light a 3D Asaro planar head, match it to a reference photo and study light, shadow and values.**

The Asaro head is the classic planar head used in ateliers to teach how light falls on the simplified planes of the face. Testa Asaro puts it in your browser on Mac, iPad and iPhone: orbit around it, place your lights, apply value filters and compare it with any reference image.

> The interface is currently in Italian. Translations are welcome.

## Features

- **3D Asaro planar head** plus basic study shapes; load your own `.glb`, `.gltf`, `.obj` or `.stl` models.
- **Orbit, pan and zoom** with mouse, trackpad or touch.
- **Responsive layout**: side panel on Mac and landscape iPad (collapsible), bottom sheet with tabs on iPhone and portrait iPad.
- **Lighting**: key, fill and rim lights with color and intensity, lighting presets, and HDRI environment lighting (built-in environments or your own `.hdr`, `.jpg`, `.png` panoramas).
- **Materials**: several surface materials, or the original colors of a loaded model.
- **Value studies**: median, posterize, blur and value-scale filters to see big shapes and value groups.
- **Reference image**: floating or split-screen, to compare the head with a photo.
- **Pose and light estimation**: mark a few points on your reference and the app turns the head and places the lights to match it.
- **Presets and settings** saved in the browser.

## Usage

It is a single HTML file with no build step: open `index.html` in a modern browser (Safari, Chrome, Firefox, Edge). It loads [three.js](https://threejs.org/) from a CDN, so the first launch needs an internet connection.

## Credits

Base model: [Asaro-head](https://sketchfab.com/3d-models/asaro-head-27a3328095ca412eaa5dde8a5da9ff3b) by ivan4akir, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), simplified and reoriented for this app. Rendering by [three.js](https://threejs.org/) (MIT).

## History

See [CHANGELOG.md](CHANGELOG.md). Versions before 0.9 were not kept.
