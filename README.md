# stekimboy.github.io

Personal portfolio of Steven Kim: aerospace, simulation and hardware projects.
Live at https://stevenbkim.com/ (GitHub Pages, custom domain; https://stekimboy.github.io/ redirects there).

The site is one `index.html` and one `styles.css` with self-hosted fonts and a
single vendored script. There is no build step: open `index.html` in a browser,
or serve the directory (`python3 -m http.server`) to test the font preload and
lazy-loading behaviour as deployed.

Deploy: GitHub Pages from `main`, root. Every "View the repository" link on the
page points at a public repo.

## Layout

| Path | What |
|---|---|
| `index.html` | All content. Sections: hero, work, skills, about, contact. |
| `styles.css` | Dark gallery canvas, hard edges, Geist type, reveal animation. |
| `assets/fonts/` | Geist and Geist Mono, subset variable fonts (SIL OFL 1.1, see `OFL.txt`). |
| `assets/lenis.min.js` | Lenis 1.3.11 smooth scroll (MIT), unmodified. |
| `assets/favicon.ico`, `assets/favicon-32.png`, `assets/apple-touch-icon.png` | Site icon (planet mark). |
| `assets/proj-*`, `assets/rde-*` | One main image or clip per project plus sub-photos, downscaled to about 1400 px wide, metadata stripped. |

## Project images

| Asset | Source |
|---|---|
| `proj-aeroforge-studio.jpg`, `proj-aeroforge-cfd.jpg`, `proj-aeroforge-pressure.jpg`, `proj-aeroforge-fusion.jpg` | `stekimboy/aeroforge-studio`, `docs/media/` and `deliverables/` |
| `proj-goggles-thermal.gif`, `proj-goggles-*.jpg` | `stekimboy/pi-thermal-goggles`, `assets/` (clip, front and angle views flattened onto the card colour) |
| `proj-rook.jpg` | `stekimboy/rook-mk2-build`, `docs/images/side-main-view.png`, flattened onto the card colour |
| `proj-rook-cad.jpg` | Render of the CAD assembly from the rook-mk2-build release STEP (meshed with OpenCascade, shaded in three.js) |
| `proj-rook-config.jpg` | Rendered excerpt of `klipper/printer.cfg` from rook-mk2-build |
| `rde-detonation.mp4`, `rde-tecplot-poster.jpg`, `rde-converge-setup.jpg` | `stekimboy/hydrogen-rde-cfd`, `media/` |

To refresh one, re-export from the source repo, downscale, and re-encode
without EXIF (the photos were taken on a phone and carried GPS data before
they were cleaned).

## Licenses

Site code is MIT; content is copyright Steven Kim. Third-party components and
their licenses are listed in `NOTICE`.
