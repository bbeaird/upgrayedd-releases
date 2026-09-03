# Upgrayedd releases

This repository contains signed macOS release artifacts and the Sparkle update feed for Upgrayedd. Application source code is maintained separately.

## Current release

- Version: 0.2.1 (build 3)
- Requires: macOS 14 or later
- Architectures: Apple silicon and Intel
- Download: [Upgrayedd-0.2.1-3.dmg](https://github.com/bbeaird/upgrayedd-releases/releases/download/v0.2.1/Upgrayedd-0.2.1-3.dmg)
- SHA-256: `8576a90afdcc2675276aab1e3b24e53ced810ec5c1928bee4bb7151b7b419bc0`

Version 0.2.0 build 2 is superseded because its background collector could not load the Sparkle framework after installation. Version 0.2.1 runs the collector from the signed application bundle and is the supported release.

Upgrayedd processes its performance telemetry locally. When update checks are enabled, the signed update feed receives ordinary HTTPS request metadata but no Upgrayedd telemetry or hardware profile. Downloads, installation, and restarts always require user confirmation.

The signed Sparkle feed is available at [appcast.xml](https://raw.githubusercontent.com/bbeaird/upgrayedd-releases/main/appcast.xml).
