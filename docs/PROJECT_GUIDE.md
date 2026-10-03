# riding_cities — project guide

Static website for the Riding Cities skateboarding association. Presents its mission and founding members and links to downloadable adult and children’s schedules.

## Scope and source

This guide describes the default branch `main` reviewed on 3 October 2026. Commands were checked against committed manifests and configuration; applications and external integrations were not executed as part of this documentation update.

## Repository map

- `site Riding Cities/index.html`
- `site Riding Cities/css/style.css`
- `site Riding Cities/documents`

## Prerequisites and local use

Clone the repository and enter its root directory:

```sh
git clone https://github.com/sarabranco92/riding_cities.git
cd riding_cities
```

Use a modern browser. No npm install is required for the static frontend. With Python installed, serve the site locally:

```sh
cd "site Riding Cities"
python -m http.server 8000
```

On Windows, use `py -m http.server 8000` if `python` is unavailable. Open http://localhost:8000/. This is a local preview server, not production hosting.

## Configuration and implementation notes

There is no build step, package manifest or application backend. Publish the contents of `site Riding Cities/` as the web root; publishing the repository root will not expose its index page at `/`.

## Verification checklist

Open the home page, check each founder’s image and text, and download both schedules. Confirm the layout at phone, tablet and desktop widths.

No dedicated automated test/spec files were found in the reviewed application tree. Where a test script exists, its presence alone does not establish test coverage.

## Maintenance

Keep this guide in sync when routes, commands, environment variables or hosting paths change. Use development databases/accounts for integration checks. Keep private credentials in server-side environment configuration and out of documentation. No new license or ownership terms are introduced by this guide; retain existing repository notices.
