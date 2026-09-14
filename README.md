# Aurora Forge Converter

**A private-preview Windows tool for bridging WWE 2K19 animation work into WWE 2K20.**

Aurora Forge is being built as a practical modding utility: less mystery clicking, more direct conversion, validation, and repeatable output. This public repository is release-only. It contains compiled downloads, not source code.

## What v0.9.0 Can Do

- Launch as a portable Windows desktop app.
- Accept a decoded WWE 2K19 animation/motion input.
- Accept a matching WWE 2K20 reference animation asset.
- Run the current WWE 2K19 to WWE 2K20 bridge from the app.
- Write a WWE 2K20 YANM20-style output file.
- Read the generated output back immediately after conversion.
- Report real validation data in the app, including output path, byte count, record count, and track count.
- Gate converter access behind Patreon tier verification.

## Verified Build Evidence

The current v0.9.0 private preview was validated before release with the Victory 6100 test material:

- Portable app launched successfully.
- Patreon tier gate verified against the configured paid tier.
- Full internal source-tool test suite passed: `127/127`.
- Packaged conversion path produced a readable WWE 2K20 output.
- Validated output size: `174,976` bytes.
- Validated output structure: `63` records, `62` motion tracks.
- Every generated motion track read back with both required streams.

That means v0.9.0 is not just a UI shell. It runs the real local conversion path and verifies the result structurally.

## What This Release Is

Aurora Forge Converter v0.9.0 is a focused bridge preview:

```text
WWE 2K19 decoded motion -> WWE 2K20 animation output
```

It is intended for controlled testing, modding research, and Patreon-gated early access.

## What This Release Is Not

To keep expectations clean:

- It is not a full WWE 2K25 converter yet.
- It does not include source code.
- It does not modify installed game files directly.
- It does not include copyrighted game assets.
- It does not claim in-game playback for every possible animation file.
- It still requires the correct source/reference assets for the current bridge.

## Patreon Access

The app requires Patreon tier verification before converter tools unlock.

Current access is controlled by the Aurora Forge Patreon campaign and the configured eligible tier. If the app opens but says `LOCKED`, the Patreon account email must be verified against an allowed active tier.

## Download

Get the latest compiled Windows build from the Releases page:

[Aurora Forge Converter Releases](https://github.com/davegranlet/Aurora-Forge-Converter-Releases/releases)

## Source Code

Source code is not published in this repository.

This repo is intentionally limited to:

- release notes
- compiled download assets
- basic public-facing information

## Redistribution

Do not mirror, repackage, sell, or redistribute Aurora Forge Converter without permission.

Aurora Forge is independent modding software and is not affiliated with or endorsed by WWE, 2K, Visual Concepts, or related rights holders.
