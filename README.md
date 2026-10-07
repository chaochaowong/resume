# Chao-Jen Wong · Personal CV

A static personal website. Open `index.html` directly in a browser, or serve this directory with `python3 -m http.server 8000`.

- `index.html`: introduction, portrait, and career flowchart.
- `cjw-resume-bioinfo-2026.html`: existing printable resume.
- `education.html`: education copied from the resume.
- `open-resources.html`: nf-core and Bioconductor contributions and talusR.
- `publications.html`: verified journal articles, first-author highlights, corrections, conference contributions, and work under review.
- `assets/site.css`: shared responsive styling.
- `assets/publications.json`: bibliography metadata for future updates; the HTML bibliography is static and must be updated alongside it.

## Palette

Screen approximations use `RGB = 255 × (1 − CMY) × (1 − K)`:

| Requested color | CMYK | Screen hex |
| --- | --- | --- |
| Raw umber | 46, 63, 87, 32 | `#5e4017` |
| Light glaucous blue | 35, 10, 14, 0 | `#a6e6db` |
| Pale king’s blue | 5, 1, 9, 0 | `#f2fce8` |
| Cream yellow | 0, 28, 68, 0 | `#ffb852` |

The supplied `L0` was interpreted as `K0`, and `co` as `C0`. Print appearance depends on the color profile.

## Publication sources

Checked October 7, 2026 against Europe PMC and PubMed, using full author names and affiliations to exclude other researchers with the initials CJ. Each entry links to its public record. Preprint versions of published papers are omitted. Conference records and the resume-listed manuscript are separated from journal articles. Recent or unindexed work may be missing; this is not a claim of exhaustive coverage.

The portrait was copied from the supplied local `cjwong.jpg` image. No build tools or external runtime dependencies are required.
