# Vuttara Browser 0.4.0

Released: 2026-09-11

Vuttara Browser 0.4.0 is a larger compatibility, Windows integration, data-continuity, download, extension-isolation, and UI reliability update.

## CAPTCHA and website compatibility

- Preserves and hardens Vuttara's Chromium-compatible network/runtime identity handling used by CAPTCHA and anti-bot challenge flows.
- Keeps the stable-network runtime and Chromium-compatible user-agent behavior in the compiled release.
- Improves compatibility with sites that perform browser, challenge, login, or authorization checks.

## Windows integration

- Improves Windows taskbar identity and Vuttara launch behavior.
- Prevents the normal development launch path from falling back to a plain Electron window.
- Improves Default Browser integration and related Settings controls.

## Downloads

- Adds and hardens **Save Download As** behavior.
- Preserves download manager reliability improvements.

## Microsoft Store and installation safety

- Microsoft Store package version is **0.4.0.0**.
- Strengthens Microsoft Store profile/data continuity when updating.
- Keeps Microsoft Store and Direct/GitHub installations isolated so they can run side by side with separate profiles/data.
- Release packaging explicitly excludes development extension/profile data.
- Store package contains no `VuttaraProfile`, `WebStoreExtensions`, or workspace payload.

## Tabs and interface

- Refines the top chrome/tab spacing so the first tab starts closer to the Vuttara branding.
- Removes runtime layout hacks that previously caused blank/chrome rendering regressions.
- Preserves vertical-tab context-menu, sleep/wake, overlay, and tab-management improvements.

## Extensions and compatibility

- Strengthens extension packaging isolation and release verification.
- Preserves extension authorization/popup compatibility improvements.
- Preserves Chrome Web Store compatibility work and Vuttara's managed extension safeguards.

## Streaming and browser reliability

- Preserves streaming/media compatibility work for Kick, Twitch, and YouTube.
- Preserves blocker/filter compatibility and browser recovery improvements.
- Removes the unfinished Recent Kick Activity UI/polling while keeping normal Kick browser functionality.

## Version/build

- Vuttara Browser **0.4.0**
- Public build **38**
- Microsoft Store package **0.4.0.0**
- Windows x64

## Validation

- Automated pre-release gates passed.
- CAPTCHA compatibility markers verified in both source and compiled output.
- Release extension isolation passed.
- Microsoft Store package manifest validation passed.
- Microsoft Store profile payload scan passed.
- Windows App Certification Kit overall result: **PASS**.

The WACK optional Electron/Chromium “Blocked executables” compatibility test may report matches inside Chromium/Electron resources, but the package's overall certification result is PASS.

## Downloads

- `Vuttara-Browser-0.4.0-x64.exe` — normal Direct/GitHub installer
- `Vuttara-Browser-0.4.0-Update-Installer-x64.exe` — updater installer

Direct/GitHub installers are unsigned. Windows may show an unknown-publisher or reputation warning. Verify the published SHA-256 before installing.
