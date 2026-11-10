# TankCompany-Offline

**An independent preservation and offline-research project for Tank Company.**

The goal is to investigate whether an offline, locally hosted experience inspired by Tank Company can be built, with local profiles, a garage, AI-controlled opponents and battles—while documenting what is and is not technically possible.

> **Status: research / bootstrap.** No working private server, original-client compatibility, battle simulation, or recovered backend is claimed yet.

## Project goals

- Inspect a legally obtained copy of the Android app and document its architecture.
- Identify client-side systems, local data formats and documented network interfaces.
- Build original server-side components for local profiles, garage data and bot battles.
- Test whether the original client can be supported without bypassing authentication, access controls, encryption or other technical protections.
- If original-client compatibility is not feasible or appropriate, build a standalone offline prototype with original code and replaceable data.

## Repository map

- `docs/ROADMAP.md` — milestones and current status.
- `docs/REVERSE_ENGINEERING.md` — evidence-based findings and unknowns.
- `docs/FILE_INTAKE.md` — what to extract and share for analysis.
- `docs/CONTRIBUTING.md` — how to contribute safely.

## First milestone

Collect a small metadata bundle from the XAPK before attempting to upload large game files. See [File intake](docs/FILE_INTAKE.md).

## Important boundaries

This is an independent, non-commercial preservation/research effort and is not affiliated with or endorsed by the game's publisher. The repository must contain only original project code, original documentation, and materials that we have permission to redistribute.

Do **not** commit:
- APK/XAPK/OBB files or extracted proprietary game assets;
- proprietary source code, decompiled source dumps, credentials, tokens, private keys or personal data;
- server addresses or protocol material obtained through unauthorized access;
- tools or patches intended to defeat authentication, anti-cheat, encryption, DRM or access controls.

We can document high-level, lawfully observed behavior and implement an independent local simulation. Any test of original-client compatibility must use authorized interfaces and must not impersonate or attack live services.

## Development approach

Node.js is the planned language for a local service/prototype. Android/Gradle tooling will be considered only if a legitimate client-side companion or diagnostic app becomes necessary. Python and standard archive tools may be used for local metadata inspection.

## Disclaimer

Tank Company and related names/assets belong to their respective owners. This project does not provide the original game, restore publisher services, or guarantee compatibility with any released client.
