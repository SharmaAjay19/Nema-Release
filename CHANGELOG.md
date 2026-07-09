<!--
  PUBLIC CHANGELOG for the Nema app.

  Keep every entry USER-FACING: describe what changed for the person using the
  app. Do NOT include internal ticket numbers, code paths, module names,
  unreleased-feature hints, or any secret/architecture detail.

  Conventions (see AGENTS.md in Nema-Internal):
    - Versioning: Semantic Versioning  MAJOR.MINOR.PATCH  (starts at 1.0.0).
    - One section per release, newest first.
    - Heading format:  ## Nema vX.Y.Z — YYYY-MM-DD
    - Group changes under: Added / Changed / Fixed / Security / Removed.
    - Link the version heading to its GitHub Release/tag where possible.
-->

# Changelog

All notable, user-facing changes to the Nema app are documented here.
This project follows [Semantic Versioning](https://semver.org/) (`MAJOR.MINOR.PATCH`).

## [Unreleased]

- Work in progress toward the next release.

## Nema v1.0.0 — 2026-07-09

First public release of Nema.

### Added
- Notebooks-as-chats with instant, texting-speed note capture (multiline, image attach).
- Pin (up to 6), archive, and delete notebooks.
- The stream: reverse-chronological notes with day dividers; long-press a note to Copy, Edit, Pin, Star, or Delete (with undo).
- Two-tier search (global / in-notebook) with date-range filters (Today / This week / This month) and a Starred filter; tap a result to jump to the note.
- Per-notebook export to Markdown or JSON.
- Encrypted backup and restore (AES-256-GCM, passphrase-protected).
- Privacy Receipt: Nema makes zero network calls.

### Security
- No INTERNET permission and no native libraries; your notes never leave the device.

<!--
Template — copy this block for each new release:

## Nema vX.Y.Z — YYYY-MM-DD

### Added
- New user-facing capability.

### Changed
- Behavior that changed for existing users.

### Fixed
- Bug fixes users will notice.

### Security
- Security-relevant fixes (describe impact, not exploit details).

### Removed
- Features removed or deprecated.
-->

<!--
## Nema v1.0.0 — YYYY-MM-DD

First public release of Nema.

### Added
- Notebooks-as-chats with instant, texting-speed note capture.
- Pin/unpin to prioritize notebooks.
- Two-tier search (global / in-notebook) with date-range filters.
- Local-first storage with encrypted backup/export.
- Privacy Receipt: Nema makes zero network calls.
-->
