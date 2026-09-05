# Upgrayedd releases

This repository contains signed macOS release artifacts and the Sparkle update feed for Upgrayedd. Application source code is maintained separately.

## Current release

- Version: 0.2.5 (build 7)
- Requires: macOS 14 or later
- Architectures: Apple silicon and Intel
- Download: [Upgrayedd-0.2.5-7.dmg](https://github.com/bbeaird/upgrayedd-releases/releases/download/v0.2.5/Upgrayedd-0.2.5-7.dmg)
- SHA-256: `87c64e5970de10d3438c38023f271a96c6f14b6e8548e3c9708cda098dcdcc0a`

Version 0.2.5 introduces the native Overview and Detailed Stats pages, a complete optional-upgrade comparison, and improved active-use history. It retires the localhost web dashboard and includes the prior collector, responsiveness, and single-instance fixes. Older immutable releases remain available for reference.

To update an existing installation, choose **Upgrayedd > Check for Updates…**, then approve installation and relaunch. For a first installation, open the DMG and move Upgrayedd.app to `/Applications`.

Upgrayedd processes its performance telemetry locally. When update checks are enabled, the signed update feed receives ordinary HTTPS request metadata but no Upgrayedd telemetry or hardware profile. Downloads, installation, and restarts always require user confirmation.

The signed Sparkle feed is available at [appcast.xml](https://raw.githubusercontent.com/bbeaird/upgrayedd-releases/main/appcast.xml).
