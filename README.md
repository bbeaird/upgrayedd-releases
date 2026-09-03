# Upgrayedd releases

This repository contains signed macOS release artifacts and the Sparkle update feed for Upgrayedd. Application source code is maintained separately.

## Current release

- Version: 0.2.0 (build 2)
- Requires: macOS 14 or later
- Architectures: Apple silicon and Intel
- Download: [Upgrayedd-0.2.0-2.dmg](https://github.com/bbeaird/upgrayedd-releases/releases/download/v0.2.0/Upgrayedd-0.2.0-2.dmg)
- SHA-256: `2480c550ed0be8bfc37d7460aaa1a961c3b90a116ee274b9ea8c52abbed54e88`

Upgrayedd processes its performance telemetry locally. When update checks are enabled, the signed update feed receives ordinary HTTPS request metadata but no Upgrayedd telemetry or hardware profile. Downloads, installation, and restarts always require user confirmation.

The signed Sparkle feed is available at [appcast.xml](https://raw.githubusercontent.com/bbeaird/upgrayedd-releases/main/appcast.xml).
