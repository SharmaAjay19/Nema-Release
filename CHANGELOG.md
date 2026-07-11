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

## Nema v2.0.0 — 2026-07-10

The first on-device AI release. Notebooks get intelligent while your notes stay
on your device.

### Added
- **AI Redraft (✨)** in the composer — tidy, shorten, expand, or rewrite as bullets before sending. Your original wording is always kept.
- **/ask** — ask a question and get an answer grounded only in that notebook's notes, with tappable source chips.
- **/compact** — summarize a notebook into a short recap.
- **Extraction rules** — describe in plain language what to pull from your notes; Nema drafts the structure, shows sample extractions to confirm, then builds a live **Extracts** table with per-day rollups, tap-to-source, inline editing, and CSV export.
- **Skills** — author reusable prompts and attach them to notebooks. Run them on demand, on a schedule, or automatically when you add a note (with a one-tap suggestion chip). Skill permissions default to read-only; writing and archiving are opt-in per skill, and every action is undoable.
- **Privacy Receipt & Sealed Mode** — see every network egress (only the optional model download) and block it entirely with Sealed Mode.
- On-demand model download (resumable) to enable the AI features.

### Changed
- Nema now requests the INTERNET permission solely for the optional, user-initiated model download. With no model downloaded, the app makes no network calls and works fully offline, exactly like v1.

### Security
- The AI runs entirely on-device. Note content never leaves your device; the download ledger records only host, byte count, and purpose.

## Nema v1.0.1 — 2026-07-09

### Changed
- Refreshed the entire look to match the Nema design language: warm paper canvas, deep-green ink, and mint message bubbles (previously the app inherited the device's system accent colors).
- Notebook list now has a dedicated search bar and Pinned / All notebooks sections.
- Chat view: notebook avatar in the header, subtle dotted wallpaper, and a rounded composer.
- Times now show in 12-hour format (2:14 PM); list timestamps are relative (Yesterday, Mon, Jun 28).
- Search results show the notebook, highlight the matched words, and summarize the result count and date range.

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
