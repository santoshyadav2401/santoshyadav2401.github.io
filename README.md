# Santosh Kumar Yadav

Personal portfolio for a Full-Stack Developer based in Nepal. Built with HTML, CSS and JavaScript, inspired by the structure and visual direction of [ayush85.github.io](https://ayush85.github.io/). All professional content comes from Santosh's résumé. Project illustrations are original decorative compositions, not product screenshots.

## Preview locally

Requires Node.js 20 or later. No installation or build is required.

```powershell
node server.mjs
```

Open http://127.0.0.1:4173. You can also open `index.html` directly. Google Fonts is optional; system fonts are used when offline.

## Files

- `index.html`: content and semantic markup.
- `styles.css`: responsive layouts, illustrations and both themes.
- `script.js`: theme preference, mobile navigation and section highlighting.
- `assets/Santosh-Kumar-Yadav-Resume.docx`: updated résumé with original document styling.
- `server.mjs`: local preview server; only public site assets are served.

## Publish to GitHub Pages

The repository is configured for `https://github.com/santoshyadav2401/santoshyadav2401.git` on `main`. Publication was deferred at the owner's request. Sign into GitHub CLI with an account that can write to this repository, then run:

```powershell
git push -u origin main
```

On GitHub, open **Settings → Pages**, select **Deploy from a branch**, then choose **main** and **/ (root)**. Since this repository is named `santoshyadav2401`, the expected Pages URL is `https://santoshyadav2401.github.io/santoshyadav2401/`. A root profile site at `https://santoshyadav2401.github.io/` instead requires a repository named `santoshyadav2401.github.io`.

The repository name also supports GitHub's profile README convention; the website needs Pages enabled separately. Do not commit personal certificates, transcripts or unrelated local images.

## Verification

`npm run check` checks JavaScript syntax. Browser QA covers desktop/mobile layouts, navigation, download, both themes, persisted preference, blocked storage and operation without JavaScript.
