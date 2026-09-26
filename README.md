# stekimboy.github.io

Personal portfolio of Steven Kim: aerospace, simulation and hardware projects.
Live at https://stevenbkim.com/ (GitHub Pages, custom domain; https://stekimboy.github.io/ redirects there).

The site is one `index.html` and one `styles.css` with self-hosted fonts. There
is no build step: open `index.html` in a browser,
or serve the directory (`python3 -m http.server`) to test the font preload and
lazy-loading behaviour as deployed.

Deploy: GitHub Pages from `main`, root. Every "Repository on GitHub" link on the
page points at a public repo.

## Layout

| Path | What |
|---|---|
| `index.html` | All content. Sections: opening, work, experience, skills, contact. |
| `styles.css` | Light "engineering report" layout: vellum ground, Newsreader headings, Geist body, figures on white sheets. |
| `assets/fonts/` | Newsreader (Latin subset, variable) and Geist, both SIL OFL 1.1 (see `OFL.txt`). |
| `assets/plate-*.jpg` | One line-drawing plate per project, shown among its photographs: combustor cutaway, flying-wing three-view, headset exploded view, CoreXY belt path (illustrations, see `NOTICE`). |
| `assets/pfp.jpg` | Profile photo in the opening. |
| `assets/favicon.ico`, `assets/favicon-32.png`, `assets/apple-touch-icon.png` | Site icon (SK monogram on a paper tile). |
| `assets/proj-*`, `assets/rde-*` | One main image or clip per project plus sub-photos, downscaled to about 1400 px wide, metadata stripped. |

## Project images

| Asset | Source |
|---|---|
| `proj-aeroforge-studio.jpg`, `proj-aeroforge-cfd.jpg`, `proj-aeroforge-pressure.jpg`, `proj-aeroforge-fusion.jpg` | `stekimboy/aeroforge-studio`, `docs/media/` and `deliverables/` |
| `proj-goggles-thermal.gif`, `proj-goggles-*.jpg`, `proj-goggles-*-cut.png` | `stekimboy/pi-thermal-goggles`, `assets/` (clip, front and angle views; the `-cut` files are the same photos with the background removed) |
| `proj-rook.jpg`, `proj-rook-cut.png` | `stekimboy/rook-mk2-build`, `docs/images/side-main-view.png`; the `-cut` file has the background removed |
| `proj-rook-cad.jpg` | Render of the CAD assembly from the rook-mk2-build release STEP (meshed with OpenCascade, shaded in three.js) |
| `proj-rook-config.jpg` | Rendered excerpt of `klipper/printer.cfg` from rook-mk2-build |
| `rde-detonation.mp4`, `rde-tecplot-poster.jpg`, `rde-converge-setup.jpg` | `stekimboy/hydrogen-rde-cfd`, `media/` |

To refresh one, re-export from the source repo, downscale, and re-encode
without EXIF (the photos were taken on a phone and carried GPS data before
they were cleaned).

## Licenses

Site code is MIT; content is copyright Steven Kim. Third-party components and
their licenses are listed in `NOTICE`.
