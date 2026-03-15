# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

Static marketing site for Christensen Software LLC (christensensoftware.com). Single-page site hosted on GitHub Pages with a custom domain. No build step, no framework, no dependencies.

## Repo Structure

- `index.html` — the entire site (HTML + inline CSS, no JS)
- `CNAME` — GitHub Pages custom domain config (`www.christensensoftware.com`)
- `robots.txt` / `sitemap.xml` — SEO files; update sitemap when adding pages
- `Christensen Software Black On White Logo.png` — site logo/favicon

## Deployment

Pushing to `main` deploys automatically via GitHub Pages. There is no build, lint, or test step.

## Development

Open `index.html` in a browser to preview. No local server required, though `python3 -m http.server` works if needed for form testing.

## Key Details

- Contact form submits to Formspree (`formspree.io/f/xykneqko`)
- All styles are inline in `<style>` within `index.html` (no external CSS)
- Schema.org structured data is embedded in the `<head>` as JSON-LD
- Site uses system fonts only (no external font loading)
