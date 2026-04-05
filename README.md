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
site/
  ├── phonescreen.mp4   # Marketing hero (watchland.ca)
  └── watchscreen.mp4
```

## Usage

Images are automatically synced from the Watchland admin panel.

Access via GitHub Pages:

- `https://mcs2k8.github.io/watchland-images-cdn/watchfaces/thumbs/{uuid}.jpg`
- `https://mcs2k8.github.io/watchland-images-cdn/watchfaces/full/{uuid}.jpg`
- Site videos: `https://mcs2k8.github.io/watchland-images-cdn/site/phonescreen.mp4` (and `watchscreen.mp4`)

## Watchland.ca APK (GitHub Releases)

GitHub rejects files over **100 MB** in normal git commits, so the marketing APK is **not** stored in this repo’s tree. It is attached to a **GitHub Release** on this repository instead. The site links to:

`https://github.com/mcs2k8/watchland-images-cdn/releases/latest/download/app-release.apk`

To publish or update the APK: create or edit a [release](https://github.com/mcs2k8/watchland-images-cdn/releases), upload an asset named exactly `app-release.apk`, and publish it as the latest release. The URL above will always point at that file.

For a ready-to-upload binary, this repo may contain a gitignored copy at `.release-upload/app-release.apk` (not committed). You can also restore it from the `watchland2025` monorepo with `git lfs pull` on `projects/watchland-site/public/assets/app-release.apk`.

## Auto-Sync

This repository is automatically updated when watchfaces/collections are synced from the local admin panel.

Last sync: $(date)
