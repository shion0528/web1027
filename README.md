# Computing for Good

A static website exploring positive applications of computing in healthcare, accessibility and environmental monitoring.

## Pages and assets

| File | Purpose |
| --- | --- |
| `index.html` | Project introduction and links to the three topics |
| `health.html` | Computing and healthcare |
| `accessibility.html` | Computing and web accessibility |
| `environment.html` | Computing and environmental monitoring |
| `assets/site.css` | Shared styling and responsive layouts |
| `assets/vendor/bootstrap/` | Local Bootstrap 5.3.8 CSS, JavaScript and licence |

All pages share navigation and a consistent theme. Topic pages link to relevant primary sources. Bootstrap is included locally, so the site does not require a CDN or a build step.

## Preview locally

Open `index.html` in a browser. Keep the HTML files and the `assets` folder together.

For an optional HTTP preview, run this command from the project folder with Python 3:

```bash
python -m http.server 14731 --bind 127.0.0.1
```

Then open `http://127.0.0.1:14731/index.html`. Stop the server with Ctrl+C. On systems where the Python 3 command is `python3`, use that command instead of `python`.

On Windows, `启动预览.cmd` looks for a working Python 3 installation through `py -3` or `python` and starts the same local preview. Keep its window open while browsing.

## Publish with GitHub Pages

1. Put this folder's contents in the repository root, with `index.html` and `assets` next to each other.
2. Commit and push the files to your repository.
3. Open **Settings → Pages → Build and deployment**.
4. Choose **Deploy from a branch**, select your publishing branch and **/(root)**, then save.
5. Once deployment completes, open the website URL supplied by GitHub and check all four pages.

## Third-party software

Bootstrap is distributed under its MIT licence. The original licence is retained at `assets/vendor/bootstrap/LICENSE`.
