# PASHA FLIX MIX

A minimal Android / Android TV / Fire TV browser-to-player app.

## What this fork keeps

- A home screen with only user-added streaming websites.
- Add a website by entering its URL; saved websites remain on the home screen.
- An embedded WebView browser with the upstream ad and pop-up blocking implementation.
- TV remote pointer / air-mouse navigation and touchscreen support.
- Automatic stream detection and hand-off to the built-in native video player.
- Full-screen playback using the upstream Media3-based player.

## What this fork hides or disables

The catalog, IPTV, sports, downloads, casting, VPN/WARP startup, source directories, account-like extras and general settings are not part of the minimal home experience. The underlying upstream code is retained where needed by the browser and native player.

## Build

GitHub Actions builds separate APKs for Android phones and Android TV / Fire TV.

- `PashaFlixMix-Android-v*.apk`
- `PashaFlixMix-TV-v*.apk`

The build uses the Android SDK, JDK 17 and the included WARP helper build required by retained upstream networking classes.

## Notes

This app is a browser and media player. It does not host, supply or endorse third-party video sources. Users are responsible for the websites they choose to visit and for complying with applicable law and each site's terms.

The browser's ad filtering is based on domain blocklists and browser-side protections. No blocker can guarantee removal of every advertisement or pop-up on every website. Some websites use DRM, encrypted streams or custom playback systems that may not be available to the native player.

## Upstream

Based on the AnantPlay Android project. See the upstream repository and its license for third-party notices and component attribution.
