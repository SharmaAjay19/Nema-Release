<!--
  PUBLIC REPO — Nema-Release.
  This repository is the public storefront for the Nema app. It contains ONLY
  the signed release APK (attached to GitHub Releases), checksums, and public
  documentation. NO source code, build files, secrets, or internal docs belong
  here. See AGENTS.md in the private Nema-Internal repo for the full policy.
-->

# Nema

**Chat-style note taking.** Nema turns note-taking into the messaging pattern
you already use every day: **notebooks are chats, notes are messages, and
capturing a thought is as fast as sending a text.**

> **Latest release: [Nema v1.0.1](../../releases/latest)** · Android 8.0+ · fully offline

- 💬 **Texting-speed capture** — open, type, send. Your note is saved instantly.
- 🗂️ **Organize by topic** — a notebook per subject (Gym Log, Food Log, Ideas),
  with pinning so this week's priorities float to the top.
- 🔍 **Find anything** — fast global and in-notebook search with date ranges.
- 🔒 **Private by construction** — Nema makes **zero network calls. Ever.**

> Nema is an Android app. It runs fully offline.

---

## 📥 Download & install

1. Go to the [**latest release**](../../releases/latest).
2. Download `nema-v1.0.1-release.apk`.
3. (Recommended) Verify the download — see **Verifying your download** below.
4. On your Android device, open the APK and allow installation from this source
   if prompted.

> Nema is distributed as a signed APK here. Sideloading requires enabling
> "Install unknown apps" for your browser/file manager.

### Verifying your download

Every release APK ships with a matching `…​.apk.sha256` checksum file. To verify
integrity:

```bash
# Compare the printed hash against the contents of the .sha256 file
sha256sum nema-v1.0.1-release.apk         # Linux / macOS
Get-FileHash nema-v1.0.1-release.apk      # Windows PowerShell (SHA256 by default)
```

The hashes must match exactly. If they don't, do not install the file.

---

## ✨ Features

- **Notebooks-as-chats** with pin/unpin to prioritize.
- **Instant note capture** — nothing ever sits between you and saving a note.
- **Two-tier search** (global / in-notebook) with date-range filters.
- **Local-first storage** that survives reinstall; encrypted local backup/export.
- **Privacy Receipt** — a running statement that Nema has made **0** network calls.

Planned intelligence (future major release): on-device AI redrafting, `/ask`
and `/compact` commands, user-authored Skills, and structured extraction — all
running **on-device**, privacy-first.

---

## 🆕 What's new in v1.0.1

A visual refresh that brings the app fully in line with the Nema design language:
warm paper canvas, deep-green ink, and mint message bubbles. The notebook list
gains a search bar and Pinned / All notebooks sections, the chat view adds a
notebook avatar and a rounded composer, times switch to a friendly 12-hour
format, and search now highlights matched words and shows a result count and
date range. See the [`CHANGELOG.md`](CHANGELOG.md) for the full history.

---

## 🔐 Privacy

Nema v1 requests **no INTERNET permission at all** — the strongest possible
privacy guarantee. Your notes never leave your device. See
[`PRIVACY.md`](PRIVACY.md) if published, or the in-app Privacy Receipt.

---

## 📝 Changelog

See [`CHANGELOG.md`](CHANGELOG.md) for the history of user-facing changes.

---

## 📄 License

Nema is released under the [MIT License](LICENSE) — © 2026 Ajay Sharma.

---

## ℹ️ About this repository

This is the **public release** repository. The application source code is
maintained privately. Issues and feedback about installing or using released
builds are welcome here; the source itself is not published.
