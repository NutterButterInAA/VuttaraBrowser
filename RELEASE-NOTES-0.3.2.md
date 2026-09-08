# Vuttara Browser 0.3.2

Released: 2026-09-08

Vuttara Browser 0.3.2 is a maintenance, extension-compatibility, and tab UX release built from the validated 0.3.1 / Build 36 baseline.

## Extension updates and Extension Store

- Improves Extension Store update reliability, history, and background update state handling.
- Adds Extension Store discovery controls with search, filters, sorting, visible-result counts, and clear/reset controls.
- Preserves Vuttara's verified extension update engine and publisher/update approval safeguards.

## Extension compatibility

- Improves extension popup handoff for external HTTP/HTTPS authorization flows.
- Adds popup-context `chrome.tabs.create()` compatibility when Electron does not provide it natively.
- Keeps extension-signed package files untouched.
- Fixes real-world extension authorization flows such as MissXss "Connect with Kick" in Vuttara.

## Tabs

- Horizontal tabs now compress adaptively as the strip fills instead of requiring horizontal scrolling.
- Keeps the New Tab `+` button directly beside the tab strip.
- Restores an accessible Close Tab button on very small tabs through hover/focus overlay behavior.
- Preserves tab mute/unmute behavior.
- Locked vertical tabs now reserve page layout space on both the left and right.
- Collapsed locked vertical tabs reserve only their collapsed width.
- Auto-hide vertical tabs remain overlay-based and do not shift page content.

## Version display

- New Tab and Settings/About now use runtime version/build information.
- Vuttara Browser 0.3.2 reports Build 37.
- Microsoft Store package version, executable FileVersion, and ProductVersion are all 0.3.2.0.

## Update channels

- Direct/GitHub installations continue using Vuttara's GitHub update channel.
- Microsoft Store installations continue using Microsoft Store-managed updates.
- The two installation channels remain side-by-side safe with separate profiles/data.

## Microsoft Store validation

- Windows App Certification Kit overall result: PASS.
- Required WACK failures: 0.
- The optional Electron/Chromium "Blocked executables" compatibility test remains the only optional failure.

## Platform

- Windows 10/11 x64
