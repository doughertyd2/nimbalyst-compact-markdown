# Markdown Sizing

A small Nimbalyst extension that makes agent-transcript markdown a bit more compact — a toned-down version of the default heading and body type scale.

Nimbalyst's default markdown sizes (from `MarkdownRenderer.tsx`) vs. this extension:

| Element | Default | This extension |
|---------|---------|----------------|
| body    | 0.9375rem | 0.875rem |
| h1      | 1.875rem  | 1.6rem  |
| h2      | 1.5rem    | 1.3rem  |
| h3      | 1.25rem   | 1.15rem |
| h4      | 1.125rem  | 1.02rem |
| h5      | 1rem      | 0.9375rem |
| h6      | 0.875rem  | 0.85rem |

Heading weights, the h1 underline, and the `--nim-border` color are preserved, so it stays theme-aware.

## How it works

Styles-only extension: `index.css` is loaded globally via the manifest `styles` field and targets `.markdown-content`. `index.js` is a required no-op entry point.

## Install

Install through Nimbalyst (Extensions → install from GitHub URL / folder). Enable it, then reload.

## Tuning

Edit the `font-size` values in `index.css` and reload the extension. Each line notes the Nimbalyst default for reference.

## License

MIT
