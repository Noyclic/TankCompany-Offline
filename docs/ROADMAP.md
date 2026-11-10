# Roadmap

This roadmap tracks verified progress. A milestone is not complete until its evidence or test is recorded.

## M0 — Repository and evidence intake
- [x] Create public repository and document project scope.
- [ ] Identify exact game version and package/application ID.
- [ ] Record XAPK archive contents and sizes.
- [ ] Identify engine and native library layout from metadata.
- [ ] Record device/Android version used for the installed copy.

## M1 — Client architecture research
- [ ] Determine whether the client is Unity, Unreal, or another engine.
- [ ] Inventory ABI folders and native library names.
- [ ] Identify whether the app uses split APKs, OBB, or Play Asset Delivery.
- [ ] Separate local configuration/assets from server-dependent features.
- [ ] Write findings with file names, hashes, tool versions and confidence levels.

## M2 — Independent local backend skeleton
- [ ] Define local account/profile schema.
- [ ] Define garage and vehicle data schema using original placeholder data.
- [ ] Add localhost-only Node.js service.
- [ ] Add automated tests and safe save/load behavior.
- [ ] Add an admin-only local development interface.

## M3 — Standalone offline battle prototype
- [ ] Define original battle state and tick model.
- [ ] Add vehicle movement and collision prototype.
- [ ] Add aiming, firing, reload and damage simulation.
- [ ] Add bot navigation and combat behavior.
- [ ] Add a small original test map and a repeatable simulation test.

## M4 — Compatibility feasibility review
- [ ] Review documented/authorized integration points.
- [ ] Determine whether original-client offline operation is technically and legally viable.
- [ ] Do not bypass authentication, anti-cheat, encryption, DRM or access controls.
- [ ] If compatibility is not viable, keep focus on the standalone offline experience.

## Current status

Only repository setup and planning are complete. No APK analysis or implementation has been verified yet.
