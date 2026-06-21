# Pace Park Group — Notes

Static blog published with GitHub Pages at **https://blog.paceparkgroup.com**.

## Structure

```
.
├── index.html                   # Homepage — hero, Latest Publications, Research Areas, Mission
├── ai-landscape.html            # Post: The AI Industry Landscape (interactive)
├── harness_jobs_analysis.html   # Post: Harness Roles — JD Analysis & Concept Explainer
├── post-template.html           # Starter template for a new post (title + body, Substack style)
├── assets/
│   └── css/
│       └── site.css             # Shared stylesheet (currently pages use inline styles)
├── CNAME                        # Custom domain config (blog.paceparkgroup.com)
└── README.md
```

Each page is a self-contained `.html` file with its styles inlined in a `<head>` `<style>` block, themed to match `assets/css/site.css` (white background, serif headings, `--accent:#ff6719`).

## Adding a post

1. Copy `post-template.html` to a new file, e.g. `my-post.html`, and fill in the title, date, and body.
2. Add the post to the **Latest Publications** list in `index.html`. Insert a new `<li class="post-item">` at the **top** of the `<ul class="posts">` so the list stays sorted newest-first:

   ```html
   <li class="post-item">
   <span class="pdate">June 21, 2026</span>
   <a href="my-post.html">My Post Title</a>
   <p>One-line description.</p>
   </li>
   ```

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy

Pushing to `main` auto-publishes via GitHub Pages (source: `main` / root).
