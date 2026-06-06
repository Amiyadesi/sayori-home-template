# Notebook Homepage Template

A static notebook-style personal homepage template. It is meant for a small personal navigation page, portfolio entry, blog home, or tiny project portal.

## Features

- Static HTML, CSS, JavaScript, and JSON only.
- Chinese and English pages under `public/zh/` and `public/en/`.
- Editable navigation, profile, services, sticky notes, and terminal text through JSON files.
- GitHub Pages workflow included. The deploy target is `public/`.
- No private API keys, account data, backend, database, or build step.

## Customize

Edit these files first:

- `public/assets/data/home-zh.json`
- `public/assets/data/home-en.json`
- `public/assets/data/lines-zh.json`
- `public/assets/data/lines-en.json`

Replace the placeholder links:

- `https://example.com/...`
- `https://github.com/your-name`
- `hello@example.com`

Optional:

- Replace sample images in `public/assets/generated/`.
- Replace or remove the favicon files.
- Add music IDs under `music.tracks` in `home-*.json`.
- Remove the terminal layer if you want a quieter homepage.

## Run Locally

```bash
python -m http.server 4177 --bind 127.0.0.1 --directory public
```

Open:

- `http://127.0.0.1:4177/zh/`
- `http://127.0.0.1:4177/en/`

## Deploy

### GitHub Pages

This repository includes `.github/workflows/pages.yml`. Enable GitHub Pages for GitHub Actions in the repository settings, then push to `main`.

### Cloudflare Pages

Use:

- Build command: empty
- Output directory: `public`

## License

MIT. The included sample art is for template/demo use; replace it with your own assets for a production personal site.
