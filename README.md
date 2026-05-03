# HomeBase Pro Camera (Android)

A modern Android-first professional camera app starter focused on:

- CameraX capture with manual controls (core v1)
- RAW-first architecture with fallback strategy roadmap
- LUT/filter pipeline (`.cube` support planned; starter presets in v1)
- iOS-inspired modern UI with smooth Compose animations

## Current status (v1)

This repository now contains a runnable Android app with:

- Jetpack Compose UI (Material 3)
- Camera preview via CameraX `PreviewView`
- Photo capture to MediaStore (JPEG)
- Pro controls in UI (EV and zoom wired; ISO/shutter/focus scaffolding)
- Live filter intensity slider with free starter filters
- Settings mode presets: **Quality**, **Balanced**, **Performance**
- Architecture prepared for RAW/LUT expansion

## Build

```bash
./gradlew assembleDebug
```

## Run

Open in Android Studio Hedgehog+ and run `app` on Android 10+ device.

## Roadmap highlights

- RAW DNG capture on supported hardware via Camera2 interop
- Multi-frame pseudo-RAW fallback pipeline on unsupported devices
- Optional Shizuku-assisted advanced controls experiment (device/root dependent)
- `.cube` LUT import/export and GPU real-time render pipeline
- Full pro controls: ISO, shutter, WB/Kelvin+tint, focus peaking, histogram, zebras
- Non-destructive editor with curves/HSL/noise reduction

## LUT source plan (free)

Recommended free LUT sources to support in-app import:

- IWLTBAP free LUT packs
- RocketStock free LUT packs
- LUTCalc / community `.cube`

(Integration UI and parser are planned next.)
