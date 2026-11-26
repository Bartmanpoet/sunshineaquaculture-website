# Sunshine Aquaculture website

The website for sunshineaquaculture.com: research, education, sustainable aquaculture and conservation.

Plain HTML and CSS, no framework or build step. Hosted on Cloudflare Pages, which republishes the site every time this repository changes.

## Files

| File | Page |
| --- | --- |
| `index.html` | Home |
| `seed-tank.html` | Seed Tank (coming next) |
| `videos.html` | Videos (coming next) |
| `about.html` | About (coming next) |
| `contact.html` | Contact (coming next) |
| `css/style.css` | Shared colors, fonts and layout for every page |
| `images/` | Web-sized images only. Full-size originals stay in the media library. |

## Editing

- Text: open the page's `.html` file and change the words between the tags.
- Colors: change the values at the top of `css/style.css`.
- Anything marked `PLACEHOLDER` still needs your real content.

To preview locally, open `index.html` in a browser.

## How publishing works

- Cloudflare Pages builds the live site from the `main` branch.
- Preview work goes on another branch first. Cloudflare gives each preview its own address.
- When a preview is approved, it is merged into `main` **as a new commit** (`git merge --no-ff`).
  Cloudflare skips a commit it has already built as a preview, so a plain fast-forward
  can leave the live site on an older version.
