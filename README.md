# Noel Jais Manuel – Portfolio

A cinematic, 3D neo-noir personal portfolio for a BCA student specialising in cybersecurity, with a focus on cloud security.

The page opens like a film title sequence: a slow camera push through light shafts and smoke, then one scene per screen as you scroll.

## Scenes

| Scene | What it shows |
| --- | --- |
| Home | Name, one-line introduction and quick buttons |
| About | Short introduction and photo |
| Education | BCA at Marian College Kuttikkanam (Autonomous) and higher secondary education |
| Internship | Eight-week internship at ipsr solutions ltd: foundations, cloud, DevOps, security, team workshop and NoirPlay |
| Security Labs | Six lab reports across cloud security, ethical hacking and IoT security |
| Projects | NoirPlay, Smart Campus Lost & Found, Python To-Do in Docker and IP Subnet Calculator |
| Skills | Cloud, DevOps, security, networking and programming tools |
| Certificates | Ten certificates; click one to open it full size (IDs are blurred) |
| Contact | Email, GitHub and LinkedIn |

## Features

- 3D background built with Three.js: light shafts, drifting smoke and dust, and a camera that moves forward as you scroll.
- Each scene pushes in as it arrives and flies past the lens as it leaves.
- Fixed navigation bar with the current scene highlighted.
- One scene per screen with snap scrolling on desktop and laptops.
- Tabbed panels for Internship and Projects so each scene fits one screen.
- Certificate viewer with keyboard support (Esc closes it).
- Responsive from small phones to large desktop monitors, with no sideways scrolling.
- Respects the "reduce motion" setting of the device.

## Tech

- Plain HTML, CSS and JavaScript in a single file, with no build step.
- [Three.js](https://threejs.org/) r128, loaded from cdnjs.
- Google Fonts: Bodoni Moda and Karla, with system fallbacks.
- Photo and certificates are embedded in the file, so it works as one file.

## Run locally

1. Download `index.html`.
2. Open it in a modern browser (Chrome, Edge, Firefox or Safari).

An internet connection is needed for the 3D library and the fonts.

## Deploy

The file is named `index.html`, so it works on any static host.

**GitHub Pages**
1. Create a repository and upload `index.html` and this `README.md`.
2. Go to Settings, then Pages.
3. Choose the main branch and the root folder, then save.

**Vercel or Netlify**
1. Import the repository, or drag the folder into the dashboard.
2. Leave the build command empty and the output folder as the root.

## Customise

All content is in `index.html`; search for the scene you want to change.

- **Text, links and email:** edit the matching `<section>`.
- **Colours:** change the variables at the top of the `<style>` block (`--lamp`, `--blood`, `--bone`, `--ink`).
- **Photo and certificates:** these are embedded images. To replace one, swap its `src` with your own image file or a new base64 data URI. Hide any certificate ID before publishing.
- **Navigation links:** edit the `<nav class="nav">` block and match each link to a section `id`.

## Project files

```
index.html   the whole website
README.md    this file
```

## Notes

- Scenes are designed to fit one screen. If you add a lot of text to a scene, the page falls back to normal scrolling for that screen size.
- Browsers without WebGL still show all content; only the 3D background is missing.
