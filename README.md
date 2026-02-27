# KFlow Assets

CDN: https://almadar-kflow-assets.web.app

Static assets for the KFlow knowledge platform — story illustrations, audio, and media files.

## Structure

```
stories/          Story illustration assets
```

## Deployment

Assets deploy automatically via GitHub Actions on push to `main`.
Manual deploy: `firebase deploy --only hosting:kflow-assets`
