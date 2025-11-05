# Watchland Images CDN

Static image hosting for Watchland watch faces and collections.

## Structure

```
watchfaces/
  ├── thumbs/   # Thumbnail previews (200x200, ~10-15KB)
  └── full/     # Full resolution images
collections/
  ├── thumbs/   # Collection thumbnails
  └── full/     # Collection full images
```

## Usage

Images are automatically synced from the Watchland admin panel.

Access via GitHub Pages:
- `https://YOUR_USERNAME.github.io/watchland-images-cdn/watchfaces/thumbs/{uuid}.jpg`
- `https://YOUR_USERNAME.github.io/watchland-images-cdn/watchfaces/full/{uuid}.jpg`

## Auto-Sync

This repository is automatically updated when watchfaces/collections are synced from the local admin panel.

Last sync: $(date)
