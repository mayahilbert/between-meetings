# Between Meetings prototype

Open `index.html` directly in a browser, or serve this folder with any static web server.

Reference viewport: **1440px wide**. The composition scales to a stacked mobile layout below 800px.

## Interactions

- Scroll the outlined black text window independently from the main page.
- Select the envelope to animate it open and reveal the Vimeo-style video placeholder.
- Select any circular play control to toggle play/pause state.
- Click a video poster/play overlay to reveal and start the responsive Vimeo embed. Poster URLs can be set directly with each frame's `data-poster` attribute; otherwise the page attempts to load the Vimeo oEmbed thumbnail and falls back to the labeled placeholder.
- Drag the filmstrip or use its subtle arrow buttons to loop manually through the stills.
- Text for the looping copy and browser window is embedded in clearly marked `String.raw` blocks in `script.js`, so it is available immediately without a network request. Both are skipped by screen readers by default and can be exposed with their visible “Read” controls.
- Drag the white invitation document; it leaves a persistent, opaque paper trail capped at 20 outlined sheets.
- Select links in that document to spawn draggable email, form, and notes panels. These panels do not leave a trail.
- Use the header and footer links for smooth page navigation.

All raster artwork is intentionally represented by labeled placeholders, as requested.
