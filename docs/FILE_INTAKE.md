# File intake: what to send for analysis

We do **not** need the full 1 GB XAPK uploaded to GitHub or this chat. Keep the original archive unchanged on your device/PC and work on a copy.

## Step 1 — Inspect the XAPK as an archive

Use 7-Zip on Windows or ZArchiver on Android to open the `.xapk` file. Do not install, patch or modify it for this first pass.

Send a screenshot or plain-text listing of the archive's top-level contents. We are looking for names and sizes such as:
- `manifest.json`
- one or more `.apk` files
- `.obb` files
- `Android/` or asset-pack directories

Do not upload the actual APK/OBB/XAPK publicly.

## Step 2 — Extract only metadata locally

If present, inspect `manifest.json` and share its non-sensitive fields:
- package name / package ID
- app version and version code
- split APK names
- OBB file names and sizes

Do not share account identifiers, authentication tokens, private URLs, device identifiers or other personal data.

## Step 3 — Identify the APK layout

If you can use a PC, open the APK with 7-Zip and send a listing of:
- `lib/` directory and its ABI subdirectories
- native library **filenames and sizes only**
- top-level directories such as `assets/`, `res/`, `META-INF/`

Do not upload proprietary library binaries or decompiled source. If a particular metadata file is needed later, we will ask for a narrowly scoped, non-sensitive report instead.

## Step 4 — Optional local hashes

A SHA-256 hash can identify the exact file version without sharing the file itself.

Windows PowerShell:
```powershell
Get-FileHash .\TankCompany.xapk -Algorithm SHA256
```

Linux/macOS:
```bash
sha256sum TankCompany.xapk
```

## What to send first

1. Screenshot of the XAPK opened as an archive, or a text listing of its top-level entries.
2. The manifest's package name and version, if visible.
3. Your Android version and device model (optional).

That is enough to choose the next inspection step. Avoid uploading the entire 1 GB archive.
