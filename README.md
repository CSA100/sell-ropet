# Ropet Selling Pages

This folder contains a simple GitHub Pages-ready Ropet KAMOMO selling site.

- `docs/index.html` - main customer-facing selling page for parents
- `docs/couples/` - optional direct-link page for young couples
- `docs/parents/` - duplicate direct-link parent page

The `docs/` folder is ready for GitHub Pages.

## GitHub Pages Setup

1. Push this project to a GitHub repository.
2. Open the repository on GitHub.
3. Go to `Settings` -> `Pages`.
4. Under `Build and deployment`, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/docs`
5. Save.

GitHub will publish:

- `/` - main parent-focused selling page
- `/parents/` - same parent-focused selling page
- `/couples/` - optional couples page if you want to share that URL directly

## Local Preview

```bash
python3 -m http.server 8090 --directory docs
```

Then open:

```text
http://localhost:8090
```

## Notes

- The Ropet referral links are already included with `rel="sponsored nofollow"`.
- The YouTube embed uses muted autoplay because browsers block autoplay with sound.
- If the YouTube embed shows Error 153 after deployment, that specific video is likely restricted from third-party embedding.
