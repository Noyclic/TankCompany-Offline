# Client research log

Use this document for reproducible, evidence-based observations. Do not paste proprietary code, secrets, personal data or large decompiled dumps.

## Rules for recording a finding

For each finding, record:
- **Date**
- **Game version / package ID**
- **Input artifact** (filename only; do not commit the artifact)
- **Tool and version**
- **Observation**
- **Evidence** (metadata, file name, hash, screenshot with private data removed)
- **Confidence** (low / medium / high)
- **Open questions**

Clearly distinguish an observation from a hypothesis. Do not guess protocol details from library names alone.

## Initial state

No client artifacts have been inspected in this repository yet.

## Questions to answer

1. What is the exact Android package/application ID and version?
2. Which engine and scripting/runtime stack does the app use?
3. Which ABIs are packaged (for example arm64-v8a or armeabi-v7a)?
4. Are resources stored in the XAPK's APKs, OBB files, or asset-delivery packs?
5. Which features appear to require a remote service, based on lawful static inspection and normal app behavior?
6. Is there a supported offline mode or documented integration interface?

## Findings

_Add dated findings below. Keep raw proprietary artifacts off the public repository._
