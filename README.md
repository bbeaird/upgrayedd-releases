# Upgrayedd releases

This repository contains signed macOS release artifacts and the Sparkle update feed for Upgrayedd. Application source code is maintained separately.

## Current release

- Version: 0.2.7 (build 9)
- Requires: macOS 14 or later
- Architectures: Apple silicon and Intel
- Download: [Upgrayedd-0.2.7-9.dmg](https://github.com/bbeaird/upgrayedd-releases/releases/download/v0.2.7/Upgrayedd-0.2.7-9.dmg)
- SHA-256: `e9366c6509494949cb544daed77021d371787b2b338628f28d99f52807d4b3e3`

Version 0.2.7 adds the Now tab with grouped activities and pressure-aware review suggestions. Dashboard refresh pauses when hidden; bounded queries reduce historical analysis overhead. Older immutable releases remain available for reference.

This is a **manual-download release**. Open the DMG and move Upgrayedd.app to `/Applications`, replacing the older app. Telemetry and preferences remain in your Library. The existing signed automatic-update feed is unchanged and does not offer 0.2.7.

Upgrayedd processes its performance telemetry locally. When update checks are enabled, the signed update feed receives ordinary HTTPS request metadata but no Upgrayedd telemetry or hardware profile. Downloads, installation, and restarts always require user confirmation.

The signed Sparkle feed is available at [appcast.xml](https://raw.githubusercontent.com/bbeaird/upgrayedd-releases/main/appcast.xml).
