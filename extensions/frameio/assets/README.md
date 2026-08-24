# Assets (bundled)

Files in this folder are packaged into the extension at build time. Only keep what the extension needs at runtime.

## Layout

```
assets/
└── icons/     # Extension & command icons (referenced in package.json)
```

> Onboarding GIFs are **not** bundled. They live on the orphan [`media`](https://github.com/phileastv/frameio_raycast_extension/tree/media) branch and are referenced by absolute URL from `SetupGuide.tsx` and the root `README.md`, so the extension source stays free of large binaries.

### `icons/`

512×512 PNG icons used by `package.json` and OAuth (`auth.ts`):

| File | Used by |
|------|---------|
| `extension-icon.png` | Extension icon |
| `browse-icon.png` | Browse command |
| `search-icon.png` | Search command |
| `last-folder-icon.png` | Open Last Folder command |
| `recent-uploads-icon.png` | Recent Uploads command |

## Editing icons

1. Export a 512×512 PNG
2. Copy the final icon into `icons/` with the matching runtime filename

Photoshop sources for the icons live under `psd/` on the [`media`](https://github.com/phileastv/frameio_raycast_extension/tree/media) branch.
