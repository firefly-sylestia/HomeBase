# HomeBase Pro Camera (Android)

A modern Android-first pro camera starter with a cleaner UI and GitHub release-ready automation.

## What works now

- CameraX live preview
- JPEG capture to MediaStore
- Modern Compose overlay with animated pro panel
- Quality/Balanced/Speed mode toggle
- Release pipeline via GitHub Actions on `v*` tags

## Release APK from GitHub tag

1. Push your changes to `main`.
2. Create a tag like `v0.1.1` and push it:
   - `git tag v0.1.1`
   - `git push origin v0.1.1`
3. GitHub Action builds release APK and attaches it to GitHub Release.

## Local build

```bash
./gradlew :app:assembleDebug
./gradlew :app:assembleRelease
```

## Roadmap (next)

- Camera2 RAW DNG capture on capable devices
- Software multi-frame fallback (pseudo-RAW)
- Optional Shizuku-assisted experimental path
- LUT `.cube` import and realtime pipeline
- Full pro tools (ISO, shutter, focus peaking, histogram)
