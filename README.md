# Scribe of Lagash — Website

The marketing site for **Scribe of Lagash**, a series of small, focused, free [Obsidian](https://obsidian.md) plugins for writers who would rather be *writing* than configuring.

The site is a single static page: no build step, no dependencies, no framework.

## The plugins

| Plugin | What it does | Obsidian | Source |
| --- | --- | --- | --- |
| **Visualization** | See every chapter and scene as a card. StoryLines, Plot matrix, Characters, Locations and Chronological views. | [Community plugins](https://community.obsidian.md/plugins/scribe-of-lagash-visualization) | [GitHub](https://github.com/aescanes/scribe-of-lagash-visualization) |
| **Goals and Stats** | Daily writing goal, statistics, writing-session timer and word/character counts in the file explorer. | [Community plugins](https://community.obsidian.md/plugins/scribe-of-lagash-goals-stats) | [GitHub](https://github.com/aescanes/scribe-of-lagash-goals-stats) |
| **Focus** | Hides everything except the page you are writing. Distraction-free, Typewriter, Spotlight and Deep work modes. | [Community plugins](https://community.obsidian.md/plugins/scribe-of-lagash-focus) | [GitHub](https://github.com/aescanes/scribe-of-lagash-focus) |

Each plugin works on its own; they are designed to complement each other. Requires Obsidian 1.10.0 or later.

## Project structure

```
.
├── index.html     # The whole site: markup, inline styles and a small lightbox script
├── img/           # Screenshots (.webp) shown in the feature sections
│   ├── vis-*.webp     # Visualization
│   ├── goals-*.webp   # Goals and Stats
│   └── focus-*.webp   # Focus
└── .nojekyll      # Tells GitHub Pages to serve files as-is (no Jekyll processing)
```

## Running locally

Open `index.html` in a browser, or serve the folder with any static server:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Editing

- **Content and styles** live in `index.html`; styles are mostly inline.
- **Fonts**: Inter and Lora, loaded from Google Fonts. Code-style text uses a monospace system stack.
- **Palette**: purple `#81096b` / `#b851a5` on a warm paper background `#f6f1e8`.
- **Screenshots**: add `.webp` files to `img/` and reference them with `data-full` on the wrapping button so they open in the lightbox.

## Deployment

Because the site is fully static and includes a `.nojekyll` file, it can be hosted on GitHub Pages or any static host by publishing the repository root.

## About

Made by [Alejandro Escanes](https://github.com/aescanes), software engineer and writer. "Scribe" is the writer at the center of every plugin; "Lagash" nods to *Nippur de Lagash*, the classic Argentine comic.

If you find the plugins useful, you can [buy me a coffee](https://ko-fi.com/O3J528W3FZ).

## License

The Scribe of Lagash plugins are free and open source under the MIT license.
