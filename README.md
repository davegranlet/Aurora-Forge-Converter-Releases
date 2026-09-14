# Aurora Forge Converter

**A Windows desktop tool for bridging WWE 2K19 animation work into WWE 2K20.**

Aurora Forge Converter is built for practical modding research: direct conversion, validation, and repeatable output. This public repository is release-only. It contains compiled downloads, not source code.

## Current Release: 1.0.0a

`1.0.0a` is the first small update after the `v1.0.0` 2K20 package-builder milestone. It adds the batch/folder workflow and ships the current portable Windows build.

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

## Batch Tool Update

The `1.0.0a` update also splits the command-line batch converter into its own public source repository:

[Aurora-Forge-2K19-to-2K20-Converter](https://github.com/davegranlet/Aurora-Forge-2K19-to-2K20-Converter)

That source repo includes the single-id package builder, the batch wrapper, tests, and documentation for automatic folder matching and manifest-driven conversion.

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

Aurora Forge Converter `1.0.0a` is a focused 2K19 to 2K20 bridge release:

```text
WWE 2K19 decoded motion + event data -> WWE 2K20 ACTS/EVD package folder
```

It is intended for controlled testing, modding research, and Patreon-gated early access.

## What This Release Is Not

To keep expectations clean:

- It is not a full WWE 2K25 or WWE 2K26 converter yet.
- It does not include copyrighted game assets.
- It does not modify installed game files directly.
- It does not include a native mod loader.
- It does not claim universal support for every animation id.
- The measured EVD body conversion is currently proven for the Victory 6100 shape.

## Related Repositories

- [Aurora-Forge-2K19-to-2K20-Converter](https://github.com/davegranlet/Aurora-Forge-2K19-to-2K20-Converter) - public source for the converter/package builder.
- [Aurora-Forge-Converter-App](https://github.com/davegranlet/Aurora-Forge-Converter-App) - public source for the desktop app shell.
- [Aurora-Forge-2K19-PAC-Tools](https://github.com/davegranlet/Aurora-Forge-2K19-PAC-Tools) - public 2K19 PAC/archive helpers.

## Download

Get the latest compiled Windows build from the Releases page:

[Aurora Forge Converter Releases](https://github.com/davegranlet/Aurora-Forge-Converter-Releases/releases)

## Source Code

The compiled app download lives here. Source code is split into the related repositories above.

## Redistribution

Do not mirror, repackage, sell, or redistribute Aurora Forge Converter without permission.

Aurora Forge is independent modding software and is not affiliated with or endorsed by WWE, 2K, Visual Concepts, or related rights holders.
