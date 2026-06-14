# GitHub Pages Deployment

This project is ready to deploy from the `docs/` folder.

## What will be published

- `/` - main parent-focused Ropet selling page
- `/parents/` - same parent-focused selling page as a direct URL
- `/couples/` - optional Ropet selling page for young couples

The older experimental files outside `docs/` will not be published if GitHub Pages is configured to serve from `/docs`.

## Deploy Steps

1. Create a GitHub repository.
2. Push this folder to the repository.
3. In GitHub, open `Settings` -> `Pages`.
4. Under `Build and deployment`, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/docs`
5. Save.

GitHub will give you a Pages URL after the first deployment finishes.

## Test Locally

From this project folder:

```bash
python3 -m http.server 8090 --directory docs
```

Then open:

```text
http://localhost:8090
```

## Notes

- YouTube autoplay is muted because browsers block autoplay with sound.
- If the embedded YouTube video still shows Error 153 after deployment on GitHub Pages, the video is likely restricted from embedding by YouTube or the video owner.
- Both selling pages already include the Ropet referral link with `rel="sponsored nofollow"`.
