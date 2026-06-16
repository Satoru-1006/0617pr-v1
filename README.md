# Birthday Memory Journey

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-live-2ea44f?style=for-the-badge&logo=github)
![Static Site](https://img.shields.io/badge/Static%20Site-HTML%20%2B%20CSS%20%2B%20JS-f97316?style=for-the-badge)
![Responsive](https://img.shields.io/badge/Responsive-Mobile%20First-2563eb?style=for-the-badge)

A cinematic birthday microsite built as a single-page interactive experience. It combines a private letter, staged transitions, a countdown moment, memory photos, and a small exploration sequence into one polished web page that can be opened from any browser.

**Live site:** [https://satoru-1006.github.io/0617pr-v1/](https://satoru-1006.github.io/0617pr-v1/)

![Home preview](./verification-v1-home.png)

## Highlights

- **One-file app shell** - the full experience is delivered from `index.html` with no build step.
- **Interactive story flow** - welcome screen, letter reading, countdown, gift journey, and finale are connected as one guided sequence.
- **Responsive layout** - optimized for desktop and mobile browsers.
- **Memory gallery assets** - local images are packaged in `assets/memory/` and served directly by GitHub Pages.
- **GitHub Pages deployment** - every push to `main` publishes the website automatically through GitHub Actions.

## Preview

| Welcome | Finale |
| --- | --- |
| ![Welcome screen](./verification-v1-home.png) | ![Finale screen](./verification-egg-finale.png) |

## Project Structure

```text
.
├── .github/workflows/pages.yml   # GitHub Pages deployment workflow
├── assets/memory/                # Memory images used by the site
├── index.html                    # Complete static web experience
├── verification-v1-home.png      # Home page verification screenshot
└── verification-egg-finale.png   # Finale verification screenshot
```

## Local Preview

Because the site uses local assets, preview it through a local HTTP server instead of opening the file directly:

```powershell
python -m http.server 8080
```

Then open:

```text
http://127.0.0.1:8080/
```

## Deployment

This repository is deployed with GitHub Pages from the `main` branch using the workflow in `.github/workflows/pages.yml`.

To update the live site:

```powershell
git add .
git commit -m "Update site"
git push
```

GitHub Actions will publish the new version automatically.

## Notes

This is a personal creative web project. The code is public for hosting and presentation, while the written content and media remain personal project material.
