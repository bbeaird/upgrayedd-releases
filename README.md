# Upgrayedd releases

This repository contains signed macOS release artifacts and the Sparkle update feed for Upgrayedd. Application source code is maintained separately.

## Current release

- Version: 0.2.2 (build 4)
- Requires: macOS 14 or later
- Architectures: Apple silicon and Intel
- Download: [Upgrayedd-0.2.2-4.dmg](https://github.com/bbeaird/upgrayedd-releases/releases/download/v0.2.2/Upgrayedd-0.2.2-4.dmg)
- SHA-256: `56987be1d66c375f1605cd882732c3cf93ffecaff487da3fdbc2f8e8d69063c9`

Version 0.2.0 build 2 is superseded because its background collector could not load the Sparkle framework after installation. Version 0.2.1 build 3 fixed that collector path but is superseded because its visible dashboard could enter a SwiftUI layout loop and consume a full CPU core. Version 0.2.2 build 4 fixes both defects and is the supported release.

Upgrayedd processes its performance telemetry locally. When update checks are enabled, the signed update feed receives ordinary HTTPS request metadata but no Upgrayedd telemetry or hardware profile. Downloads, installation, and restarts always require user confirmation.

The signed Sparkle feed is available at [appcast.xml](https://raw.githubusercontent.com/bbeaird/upgrayedd-releases/main/appcast.xml).
