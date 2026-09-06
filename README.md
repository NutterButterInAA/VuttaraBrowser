# Vuttara Browser - Public Releases

This repository is the public distribution endpoint for **Vuttara Browser**.

The development source repository is private. Public users can download verified Windows releases from the **Releases** section.

## Current stable release

**Vuttara Browser 0.3.1**

- Windows x64 installer: `Vuttara-Browser-0.3.1-x64.exe`
- Installer SHA-256: `8B1690EF2528E07BAB75295DE087ADC390422DA339CE500B450B2A498EF5011A`
- Updater installer: `Vuttara-Browser-0.3.1-Update-Installer-x64.exe`
- Updater SHA-256: `8164BA0EC521749B9FC1B1872F1480D0773669DB3C543547944CBA0F73C339C8`
- Website: https://www.nuttabuttainaa.com/vuttara/browser/
- Microsoft Store: https://apps.microsoft.com/detail/9NQ11CCWPNZ3
- Releases: https://github.com/NutterButterInAA/VuttaraBrowser/releases

### 0.3.1 highlights

- Fixed stale **Latest found** updater reporting after an upgrade
- Cleans obsolete downloaded update installers and stale Ready state
- Forces a fresh update check when the installed Vuttara version changes
- Sorts releases semantically instead of trusting API ordering
- Retries transient GitHub, checksum, and download request failures
- Manual checks bypass stale HTTP caches
- Rejects incomplete downloads before installation
- Waits for Windows to confirm the updater process started before Vuttara exits
- Preserves all 0.3.0 AI, Stream Mode, downloads, web apps, fullscreen, translation, privacy, and performance features

The direct GitHub installers are unsigned, so Windows may show an unknown-publisher or reputation warning. Verify the published SHA-256 before installing.

Microsoft Store packages are distributed and updated through Microsoft Store.
