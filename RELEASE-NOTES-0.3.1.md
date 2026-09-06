# Vuttara Browser 0.3.1

Released: 2026-09-06

## Updater reliability

- Fixed **Latest found** showing a stale previously downloaded version after Vuttara had already upgraded.
- Cleans obsolete downloaded updater installers and stale Ready state when the installed version is already equal to or newer than the downloaded package.
- Stores the Vuttara version associated with the last update check so an old cooldown cannot suppress the first check after upgrading.
- Tracks the newest visible release separately from installable update candidates, so an up-to-date browser still reports the correct latest published version.
- Sorts release candidates by semantic version instead of depending on GitHub API result order.
- Adds retry handling for transient network failures and HTTP 408, 425, 429, 500, 502, 503, and 504 responses.
- Manual checks use no-cache headers and a cache-busting query so a newly published release can be discovered promptly.
- Detects incomplete installer downloads before SHA-256 validation and installation.
- Prevents concurrent duplicate update checks.
- Waits for Windows to confirm the verified updater process spawned before Vuttara exits. If launching fails, Vuttara remains open and the verified package stays ready to retry.

## Update control

- Vuttara still never downloads, installs, or restarts for an update without user action.
- GitHub/NSIS installations continue using Vuttara's verified GitHub updater.
- Microsoft Store installations continue using Microsoft Store-managed updates only.

## Preserved 0.3.0 features

All Vuttara Browser 0.3.0 features remain included, including Vuttara AI, web AI chats, AI research tools, translation, per-site zoom, context tools, tab previews, the expanded Downloads Center, Stream Mode, installable web apps, true monitor fullscreen, performance improvements, and profile/channel isolation.
