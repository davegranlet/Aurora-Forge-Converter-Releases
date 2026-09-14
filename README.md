# Aurora Forge Converter Releases

**Compiled Windows downloads for Aurora Forge Converter.**

This public repository is release-only. It contains compiled EXE downloads and public release notes. Source code, converter internals, research tools, and support workers are private.

## Current Release: 1.0.0a

`1.0.0a` is the current compiled Windows preview build.

Download:

- `aurora-forge-converter.1.0.0a.exe`

## What 1.0.0a Can Do

- Launch as a portable Windows desktop app.
- Gate converter access behind Patreon tier verification.
- Build a 2K20-ready package folder for the verified Victory 6100 path.
- Accept a decoded WWE 2K19 motion body.
- Accept the matching 2K19 event `0FOP` file.
- Accept known-good WWE 2K20 reference `ACTS` and `EVD` files.
- Write converted package output under `Root\Animation\Victory`.
- Produce both converted `6100.acts` and `6100.evd` outputs.
- Read the generated output back and report validation metrics.

## Verified Build Evidence

The current 2K19 to 2K20 package path has been validated with the Victory 6100 test material:

- Portable app build completed successfully.
- Focused converter/package test suite passed.
- Batch folder-mode dry run matched the 2K19 motion, 2K19 event `0FOP`, 2K20 reference `ACTS`, and 2K20 reference `EVD` for id `6100`.
- Real batch build succeeded for id `6100`.
- Converted motion output: `174,976` bytes, `62` tracks.
- Converted ACTS output: `429,196` bytes.
- Converted EVD output: `20,610` bytes, `24` event bodies.
- Earlier `v0.9.0` testing established a visible WWE 2K20 in-game proof point for the bridge path.

## What This Release Is

Aurora Forge Converter `1.0.0a` is a focused 2K19 to 2K20 bridge preview distributed as a compiled Windows executable.

It is intended for controlled testing, modding research, and Patreon-gated early access.

## What This Release Is Not

To keep expectations clean:

- It is not a full WWE 2K25 or WWE 2K26 converter yet.
- It does not include source code.
- It does not include converter internals or research scripts.
- It does not include copyrighted game assets.
- It does not modify installed game files directly.
- It does not include a native mod loader.
- It does not claim universal support for every animation id.

## Source Code

Source code is private. This public repo intentionally contains only compiled downloads and public-facing release notes.

## Redistribution

Do not mirror, repackage, sell, or redistribute Aurora Forge Converter without permission.

Aurora Forge is independent modding software and is not affiliated with or endorsed by WWE, 2K, Visual Concepts, or related rights holders.
