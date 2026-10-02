# BR-MANGUE Studio website

Public project site and direct downloads for BR-MANGUE Studio:
[oceanpep.github.io/br-mangue-studio-site](https://oceanpep.github.io/br-mangue-studio-site/).
The site uses static HTML and CSS, has no build step, and provides English and Brazilian Portuguese pages.

## Pages

English pages are in the repository root; their Portuguese versions are in `pt-br/`.

- `index.html` — project overview and performance summary
- `downloads.html` — downloads, platform requirements, and checksums
- `guide.html` — input preparation and simulation workflow
- `articles.html` — published scientific background and software test records
- `benchmarks.html` — measured performance, methods, and limitations
- `projects.html` — current release and platform status

The model implementation, source documentation, and research materials are maintained in the [BR-MANGUE Studio source repository](https://github.com/oceanpep/br-mangue-studio).

## Preview locally

From this directory, start a simple local web server:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000` in a browser. The Portuguese version is at `/pt-br/`. Stop the server with `Ctrl+C`.

## Update a download

Keep the download link, displayed file size, and SHA-256 checksum in `downloads.html` and `pt-br/downloads.html` in sync with the files in `downloads/`. Recalculate and verify each checksum after replacing an executable. Do not add research rasters, personal files, or unpublished results to this public repository.

## Publishing

The `main` branch is the GitHub Pages publishing source. Once a change is committed and pushed, GitHub Pages publishes the static site automatically.
