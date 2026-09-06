# Vuttara Browser 0.3.0

Vuttara Browser 0.3.0 is a major feature update focused on AI-assisted browsing, media and multitasking, downloads, page tools, and safer side-by-side distribution through GitHub and Microsoft Store.

## Vuttara AI

- Added the Vuttara AI sidebar with page summarization, key points, explanations, page Q&A, selected-text actions, and a Writing Assistant.
- Added secure provider-specific API-key storage using the Windows-bound Electron secure storage path used by Vuttara profiles.
- Added OpenAI, Groq, Google Gemini, OpenRouter, LM Studio, Ollama, and custom OpenAI-compatible provider options.
- Added integrated web-chat modes for ChatGPT, Gemini, Claude, Copilot, and Perplexity using the normal Vuttara profile session.
- Added persistent native AI conversations, chat search, pinning, renaming, export, and continuation.
- Added multi-tab AI research, source-linked tab citations, tab organization, semantic tab/history/bookmark search, screenshot and image analysis, PDF assistance, AI omnibox commands, and section-specific page analysis.
- Added automatic provider routing, Prefer Free / Prefer Local modes, provider fallback, Local AI Only, usage controls, expanded AI privacy permissions, prompt-injection filtering, and a controlled browser-action agent.
- Added an expanded Writing Assistant with tone and format transformations plus preview/replace/copy/retry controls.

## Tabs, page tools, and translation

- Added element-specific page context menus with improved image, media, link, and editable-field actions.
- Added media Save As support and image tools including Google Lens / image-information actions where applicable.
- Added per-site zoom with keyboard zoom controls and persistent site-specific zoom state.
- Added page translation with Translate / Show Original controls, a toolbar action, and language settings.
- Improved duplicate-tab controls and existing tab-management behavior.
- Added tab preview cards with page thumbnails, title, URL, and tab-state information for horizontal and vertical tabs.

## Stream Mode and fullscreen video

- Added Stream Mode for viewing multiple selected live tabs in a tiled browser layout without creating duplicate stream tabs.
- Added explicit Add to Stream Mode / Remove from Stream Mode controls in horizontal and vertical tab menus.
- Added safe Stream Mode audio controls including Mute All and Solo Current Tab Audio.
- Added safe handling for sleeping or recreated tabs when preparing a Stream Mode layout.
- Added true HTML video fullscreen that uses the entire monitor and hides Vuttara chrome while fullscreen is active.
- Fixed fullscreen exit so the normal browser chrome, page layout, vertical tabs, and Stream Mode layout restore correctly.

## Downloads

- Expanded the Downloads Center with simultaneous-download limits, automatic queuing, priorities, Pause All / Resume All, improved filtering and sorting, progress, speed, ETA, source copying, and completed-file SHA-256 checksums.
- Preserved retry, resume, cancel, open, open-containing-folder, and duplicate-filename safety behavior.

## Installed web apps

- Added Install This Site as App for supported web apps and ordinary websites.
- Added standalone Vuttara-managed app windows using the installing Vuttara profile session.
- Added Start Menu and optional Desktop shortcuts.
- Added `vuttara://apps/` for launching apps, recreating shortcuts, and uninstalling installed web apps.
- Added true fullscreen support inside installed web apps.

## Performance and stability

- Reduced Vuttara-side page-load overhead by caching per-site zoom lookups, batching browser-state updates, and debouncing title/favicon metadata updates.
- Improved omnibox focus/caret stability around menus and tab previews.
- Moved tab previews to a dedicated native overlay so previews no longer resize or re-layer the address-bar chrome.
- Added safer WebContents lookups around fullscreen and Stream Mode to prevent stale/sleeping tabs from causing main-process errors.

## GitHub and Microsoft Store channels

- GitHub/NSIS and Microsoft Store/MSIX installs use separate single-instance locks and separate profile/data locations so both editions can be installed on the same Windows PC.
- GitHub builds continue to use Vuttara's GitHub release updater.
- Microsoft Store builds disable the GitHub application updater and use the Store-specific Updates Center instead.

## Notes

Vuttara Browser remains Windows-first. The direct GitHub installer is unsigned and Windows may display an unknown-publisher or reputation warning. Microsoft Store packages are signed and distributed by Microsoft Store after certification.
