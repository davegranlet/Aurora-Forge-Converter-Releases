# Aurora Forge Releases

Compiled Windows previews and public release notes for Aurora Forge Converter.

## Current NT100 Linux Preview: 1.8.0-beta.1

`1.8.0-beta.1` is the current native Linux x64 preview build of AuroraForge NT100.

Download:

- `Aurora-Forge-v1.8.0-beta.1-Linux-x64.tar.gz`
- `Aurora-Forge-v1.8.0-beta.1-Linux-x64.tar.gz.sha256.txt`

Run:

```sh
tar -xzf Aurora-Forge-v1.8.0-beta.1-Linux-x64.tar.gz
cd Aurora-Forge-v1.8.0-beta.1-Linux-x64
./AuroraForge\ NT100
```

If your file manager strips executable permissions:

```sh
chmod +x "AuroraForge NT100"
./AuroraForge\ NT100
```

Linux-native capabilities include the NT100 app shell, project work, prompt builders, prompt review/export, setup/reference pages, validation guidance, and CAK catalog browsing/search.

Windows-only pieces are allowed as user-provided helpers, but they are not bundled as Linux-native binaries. That includes DirectXTex `texconv.exe`, `AuroraCakHelper.exe`, `AuroraPac19Helper.exe`, WWE/Oodle DLLs, `dinput8.dll` loaders, and Windows-only converter EXEs. Full game injection/loading remains a Windows game workflow.

## Release Candidate: Aurora Forge Beta2

`Aurora Forge Beta2` is the integrated main-app release. The converter is launched from the signed-in Aurora Forge shell, which owns the access check and passes the verified session into the bundled capability.

Download candidate:

- `Aurora-Forge-v1.8.0-beta.1-Windows-x64.zip`
- `Aurora-Forge-Beta2-Preview.exe`

Verify downloads against `SHA256SUMS.txt` before running them.

## Current Scope

- Runs as a portable Windows desktop application with the Aurora Forge Beta2 shell as the user-facing home.
- Accepts decoded WWE 2K19 motion.
- Accepts a WWE 2K25 `.clips` template selected by the tester.
- Re-encodes selected motion groups into a separately written replacement `.clips` file.
- Builds and reopens a loader-ready replacement CAK through Aurora CAK Foundry.
- Keeps source files and installed game archives unchanged.
- Retains the earlier verified WWE 2K19 to WWE 2K20 bridge workflow.

## Beta Boundaries

- Controlled WWE 2K25 replacement is ready for owner testing, not a final compatibility claim.
- Additive `TEST 14000` picker and preview behavior is not yet proven.
- General full-body fidelity, final root/pose alignment, and facial conversion remain experimental.
- The executable does not include copyrighted game assets.
- Support is not claimed for every animation ID, game version, or extracted template.

See `TESTING_Beta2.md` for the release-gate procedure and `RELEASE_NOTES_Beta2.md` for details.

## WWE 2K25 Test Deployment and CAK Manager

Aurora Forge v1.8.0-beta.1 adds a dedicated, ownership-aware test manager that backs up and installs the exact verified loader pair, stages a controlled test CAK, manages direct-child CAKs without moving files, and restores only files it recorded.

## Umbrella App

Aurora Forge v1.8.0-beta.1 bundles this converter, the verified WWE 2K25 loader pair, the 33-project catalog, and the existing flagship tools. Its Windows ZIP is distributed as a GitHub Release asset because it exceeds GitHub's normal repository-file size limit.

## Repository Scope

This repository contains compiled release downloads and public-facing release documentation. Source projects and research history are managed separately.

## Community

- Discord: https://discord.gg/pBuHF4mugQ
- Patreon: https://www.patreon.com/cw/dgranletmwo

## Legal

Aurora Forge is independent modding software and is not affiliated with or endorsed by WWE, 2K, Visual Concepts, or related rights holders. Do not redistribute copyrighted game files.
