# Ocarina Recomp, Hookshot & TriAevum: release checksums and setup notes

A small, factual companion to **[ocarinarecomp.wiki](https://ocarinarecomp.wiki/)**, covering the three native PC recompilations of *The Legend of Zelda: Ocarina of Time*:

| Project | Repository | Game edition | Platforms |
|---|---|---|---|
| Ocarina Recomp | [sostenesfreitas/ocarina-recomp](https://github.com/sostenesfreitas/ocarina-recomp) | Switch 2 edition (v1.1.1) | Windows ZIP installer |
| Hookshot | [NotRexed/Hookshot](https://github.com/NotRexed/Hookshot) | Switch 2 edition (build e0f3ccfa) | Windows installer + launcher, Linux AppImage |
| TriAevum | [coccofresco/TriAevum](https://github.com/coccofresco/TriAevum) | Ocarina of Time 3D (3DS) | Windows ZIP, AppImage, Flatpak |

This repository contains **no binaries, game files, keys or ROMs**, and does not explain how to obtain them. Every project builds or prepares the game on your own PC from a copy you own. Download only from the repositories above.

## Latest release files and SHA-256 (checked 2026-11-08 15:50 UTC)

| Project | Tag | File | Bytes | SHA-256 |
|---|---|---|---|---|
| Ocarina Recomp | `v0.2.7` | `Ocarina-Setup-0.2.7-windows.zip` | 115,815,239 | `044c4584e16017caf19b6f9308bdd30f9977e50cd32516a68b89c2b7d09aee64` |
| Hookshot | `v2.0.0` | `HookshotBuilder.exe` | 175,616 | `46e1f7d6a8e2649fe34737f3d9536ff5f7e08acefc72d5194dd00ab2c1085672` |
| Hookshot | `v2.0.0` | `hookshot-setup.txt` | 1,658 | `b4ca5be4ee0b0e9ab8e5cd49d76ff77d4ce0366d3e89185e947011fc837acf9d` |
| Hookshot | `v2.0.0` | `Hookshot-v2.0.0-x86_64.AppImage` | 215,542,264 | `8d0e537110e4fb864f8c4d223036bcf2a2774c5f1d20a083419ca3f2d952e6f5` |
| TriAevum | `v0.8.0-beta.1.2` | `SHA256SUMS.txt` | 332 | `ebfdc35b8743fb1d32bc6da834e26fcef78e21488ed9566f1194308d276047ed` |
| TriAevum | `v0.8.0-beta.1.2` | `TriAevum-v0.8.0-beta.1.2-Linux-x86_64.AppImage` | 465,828,344 | `2e80fb50e1d21ffc5cc852a90f715408b82e65839e8baf8b3dbf6f9295d5296a` |
| TriAevum | `v0.8.0-beta.1.2` | `TriAevum-v0.8.0-beta.1.2-Linux-x86_64.flatpak` | 269,893,960 | `575db1812b37070e9512192bf760d5d78b9efda158b740a089a2eb1a528a54ef` |
| TriAevum | `v0.8.0-beta.1.2` | `TriAevum-v0.8.0-beta.1.2-Windows-x64.zip` | 550,467,290 | `23c3febe3a4dc1b7ffe652f21861f4c5b5068411a16df5fc721e52a80ba817a6` |

Verify a download:

```sh
# Windows
certutil -hashfile HookshotBuilder.exe SHA256
# Linux
sha256sum Hookshot-*-x86_64.AppImage
# macOS
shasum -a 256 Ocarina-Setup-*-windows.zip
```

Or drop the file into the in-browser checker on [ocarinarecomp.wiki](https://ocarinarecomp.wiki/) (WebCrypto, nothing is uploaded).

## Hookshot v2.0.0 (2026-11-08)

The first numbered Hookshot release. On Windows only `HookshotBuilder.exe` is needed: it downloads the builder and its tools (about 460 MB, once) and checks every part against the SHA-256 listed in `hookshot-setup.txt`. The old `HookshotBuilder.zip` ended with `device-lost-fix`.

- `hookshot.exe` now opens a launcher with **Play**, and **Update** when a newer release is out. Updates download only the changed parts and compile only what changed. The game and its DLLs moved to `bin\`; saves and settings stay.
- Fixes: flickering (#574), water flicker and fog haze, a crash on scene changes around Hyrule Castle, Castle Town and Kakariko (#287), neon colours on AMD.
- Earlier the same day: real ultrawide (HUD kept 16:9), about 45% more fps (33 → 47 in Kokiri on an RTX 4060 Ti), 4 GB card and Intel Arc fixes.

Full notes: [Hookshot guide](https://ocarinarecomp.wiki/hookshot/) · [changelog](https://ocarinarecomp.wiki/changelog/).

## Which one should I use?

- **Windows, simplest install, Brazilian Portuguese, emulator save import:** Ocarina Recomp.
- **Linux, frame generation, ultrawide, rebinding:** Hookshot. See the [Hookshot guide](https://ocarinarecomp.wiki/hookshot/).
- **You own the 3DS version:** TriAevum (no compiler needed).

Side-by-side table of fps reports, GPU support and features: [Hookshot vs Ocarina Recomp](https://ocarinarecomp.wiki/hookshot-vs-ocarina-recomp/).

## Requirements in one line

Vulkan 1.3 GPU **with mesh shaders** (GTX 16 / RTX 20, RX 6000, Intel Arc or newer; no GTX 10-series), 16 GB RAM or more (raise the Windows page file to 16384–32768 MB with 16 GB), 40–60 GB free while building. Details: [requirements](https://ocarinarecomp.wiki/requirements/).

## More

- [Downloads and all release checksums](https://ocarinarecomp.wiki/download/)
- [Compatibility status and known bugs](https://ocarinarecomp.wiki/compatibility-status/)
- [Controller setup](https://ocarinarecomp.wiki/controllers/)
- [Changelog](https://ocarinarecomp.wiki/changelog/)
- [Guia em português](https://ocarinarecomp.wiki/pt/) · [Guía en español](https://ocarinarecomp.wiki/es/)

---

Independent notes; not affiliated with the projects' developers or Nintendo. The Legend of Zelda and Ocarina of Time are trademarks of Nintendo. Text licensed CC BY 4.0.
