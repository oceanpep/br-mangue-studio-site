# BR-MANGUE Studio website

Public project site and direct downloads for BR-MANGUE Studio:
[oceanpep.github.io/br-mangue-studio-site](https://oceanpep.github.io/br-mangue-studio-site/).
The site is a static HTML and CSS project with no build step or runtime
JavaScript dependency.

## Pages

- `index.html` — project overview and direct platform downloads
- `downloads.html` — operating-system requirements, file sizes, and checksums
- `guide.html` — input preparation and simulation workflow
- `articles.html` — reference study, paper draft, and test records
- `benchmark-cmma-anadem-20260917.html` — measured performance and methods
- `projects.html` — current release and verification status

The model implementation, source documentation, and paper draft are maintained
in the [BR-MANGUE Studio source repository](https://github.com/oceanpep/br-mangue-studio).

## Preview locally

From this directory, start a simple local web server with:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000` in a browser. Stop the server with `Ctrl+C`.

## Update a download

Keep the download link, displayed file size, and SHA-256 checksum in
`downloads.html` in sync with the files in `downloads/`. Recalculate and verify
the checksum after replacing an executable. Do not add research rasters,
personal files, or unpublished results to this public repository.

## Publishing

The `main` branch is the GitHub Pages publishing source. Once a change is
committed and pushed, GitHub Pages publishes the static site automatically.
