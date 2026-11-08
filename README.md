# Ocarina Recomp, Hookshot & TriAevum: release checksums and setup notes

A small, factual companion to **[ocarinarecomp.wiki](https://ocarinarecomp.wiki/)**, covering the three native PC recompilations of *The Legend of Zelda: Ocarina of Time*:

| Project | Repository | Game edition | Platforms |
|---|---|---|---|
| Ocarina Recomp | [sostenesfreitas/ocarina-recomp](https://github.com/sostenesfreitas/ocarina-recomp) | Switch 2 edition (v1.1.1) | Windows ZIP installer |
| Hookshot | [NotRexed/Hookshot](https://github.com/NotRexed/Hookshot) | Switch 2 edition (build e0f3ccfa) | Windows builder, Linux AppImage |
| TriAevum | [coccofresco/TriAevum](https://github.com/coccofresco/TriAevum) | Ocarina of Time 3D (3DS) | Windows ZIP, AppImage, Flatpak |

This repository contains **no binaries, game files, keys or ROMs**, and does not explain how to obtain them. Every project builds or prepares the game on your own PC from a copy you own. Download only from the repositories above.

## Latest release files and SHA-256 (checked 2026-11-08 UTC)

| Project | Tag | File | Bytes | SHA-256 |
|---|---|---|---|---|
| Ocarina Recomp | `v0.2.7` | `Ocarina-Setup-0.2.7-windows.zip` | 115,815,239 | `044c4584e16017caf19b6f9308bdd30f9977e50cd32516a68b89c2b7d09aee64` |
| Hookshot | `device-lost-fix` | `Hookshot-device-lost-fix-x86_64.AppImage` | 215,493,112 | `29e6214c4403567fc64b04dffee2d37051208d64f8f4d098c7bd97ad7f222774` |
| Hookshot | `device-lost-fix` | `HookshotBuilder.zip` | 398,156,393 | `c663d16738e3d8970c40bc12e0f2587f96a2e582228139dc0bbb9b4ed79078d9` |
| TriAevum | `v0.8.0-beta.1.2` | `SHA256SUMS.txt` | 332 | `ebfdc35b8743fb1d32bc6da834e26fcef78e21488ed9566f1194308d276047ed` |
| TriAevum | `v0.8.0-beta.1.2` | `TriAevum-v0.8.0-beta.1.2-Linux-x86_64.AppImage` | 465,828,344 | `2e80fb50e1d21ffc5cc852a90f715408b82e65839e8baf8b3dbf6f9295d5296a` |
| TriAevum | `v0.8.0-beta.1.2` | `TriAevum-v0.8.0-beta.1.2-Linux-x86_64.flatpak` | 269,893,960 | `575db1812b37070e9512192bf760d5d78b9efda158b740a089a2eb1a528a54ef` |
| TriAevum | `v0.8.0-beta.1.2` | `TriAevum-v0.8.0-beta.1.2-Windows-x64.zip` | 550,467,290 | `23c3febe3a4dc1b7ffe652f21861f4c5b5068411a16df5fc721e52a80ba817a6` |

Verify a download:

```sh
# Windows
certutil -hashfile HookshotBuilder.zip SHA256
# Linux
sha256sum Hookshot-*-x86_64.AppImage
# macOS
shasum -a 256 Ocarina-Setup-*-windows.zip
```

Or drop the file into the in-browser checker on [ocarinarecomp.wiki](https://ocarinarecomp.wiki/) (WebCrypto, nothing is uploaded).

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
