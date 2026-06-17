# spp-site

Source for the **spp** documentation site — the Supervised Prompt Producer plugin for Claude Code.

- **Live site:** <https://jaylbean.github.io/spp-site/>
- **Plugin repo:** <https://github.com/JayLBean/supervised-prompt-producer>
- **Benchmark:** <https://jaylbean.github.io/spp-benchmark/>

## What's here

A [Quarto](https://quarto.org) website (serif-academic theme) with seven pages: Home, Methodology,
Installation, Usage, Commands, Examples, and Scope. Content is sourced from the plugin repo's
`DESIGN.md`, `README.md`, the phase docs, and `ROADMAP.md`.

## Build locally

```sh
quarto preview     # live-reload preview
quarto render      # build _site/
```

## Publishing

`.github/workflows/publish.yml` renders the site on every push to `main` that touches a source
file and pushes `_site/` to the `gh-pages` branch. Enable GitHub Pages on `gh-pages` (root) to
serve it.
