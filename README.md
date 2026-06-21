# Pace Park Group — Notes

Static blog published with GitHub Pages at **https://blog.paceparkgroup.com**.

## Structure

```
.
├── index.html              # Blog homepage (post list)
├── ai-landscape/
│   └── index.html          # Post: The AI Industry Landscape (interactive)
├── assets/
│   └── css/
│       └── site.css        # Shared site chrome (nav, footer, post cards)
├── CNAME                   # Custom domain config
└── README.md
```

## Adding a post

1. Create a folder for the post slug, e.g. `my-post/`, with an `index.html` inside (gives a clean URL `/my-post/`).
2. Link the shared stylesheet in `<head>`: `<link rel="stylesheet" href="/assets/css/site.css">`.
3. Add the site nav block at the top of `<body>` (copy from any existing page).
4. Add a `<li>` card to the post list in the root `index.html`.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy

Pushing to `main` auto-publishes via GitHub Pages (source: `main` / root).
