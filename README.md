# Ocarina Recomp, Hookshot, NX2navi, TriAevum & Ocarina ReTuned: release checksums and setup notes

A factual companion to **[ocarinarecomp.wiki](https://ocarinarecomp.wiki/)**, covering the five native recompilations of *The Legend of Zelda: Ocarina of Time*:

| Project | Repository | Game edition | Platforms |
|---|---|---|---|
| Hookshot | [NotRexed/Hookshot](https://github.com/NotRexed/Hookshot) | Switch 2 edition (build e0f3ccfa) | Windows installer + launcher, Linux AppImage |
| NX2navi | [tangerineturtle1/NX2navi](https://github.com/tangerineturtle1/NX2navi) | Switch 2 edition (v1.1.1) | Windows setup + updater, Linux AppImage |
| Ocarina Recomp | [sostenesfreitas/ocarina-recomp](https://github.com/sostenesfreitas/ocarina-recomp) | Switch 2 edition (v1.1.1) | Windows ZIP installer + Hookshot migration scripts |
| TriAevum | [coccofresco/TriAevum](https://github.com/coccofresco/TriAevum) | Ocarina of Time 3D (3DS) | Windows ZIP, Linux AppImage, Flatpak |
| Ocarina ReTuned | [OTPR26/Ocarina-ReTuned](https://github.com/OTPR26/Ocarina-ReTuned) | Ocarina of Time 3D (3DS) | Windows, macOS 15+, Linux, Android ARM64 |

This repository contains **no binaries, game files, keys or ROMs**, and does not explain how to obtain them. Every project builds or prepares the game locally from a copy you own. Download only from the GitHub repositories above.

## Latest release files and SHA-256 (checked 2026-11-12 08:45 UTC)

| Project | Tag | File | Bytes | SHA-256 |
|---|---|---|---|---|
| Hookshot | `v2.1.0` | `HookshotBuilder.exe` | 175,616 | `46e1f7d6a8e2649fe34737f3d9536ff5f7e08acefc72d5194dd00ab2c1085672` |
| Hookshot | `v2.1.0` | `hookshot-setup.txt` | 1,687 | `c852e8c096f16d658a472ebcf6f72c37d9b5472df5155da913760cb6dc0f9cb2` |
| Hookshot | `v2.1.0` | `Hookshot-v2.1.0-x86_64.AppImage` | 216,133,816 | `0164e97c3114e22b4ad1ca7826f50d0eb5f35852586c1c4e4de2c3bd053fb50c` |
| NX2navi | `v0.8.0` | `NX2navi-Setup-0.8.0.exe` | 136,923,839 | `0ad3aeb1dafe81246e5a24e82804668c1b15159b27c84d95713e4d58f2a886ab` |
| NX2navi | `v0.8.0` | `NX2navi-Linux-0.8.0-x86_64.AppImage` | 101,087,736 | `b7deb7147658f0d0c97f4ed1b9721ce78eebc96c92111b617d1a2d333d2a39f7` |
| Ocarina Recomp | `v0.3.4` | `Ocarina-Setup-0.3.4-windows.zip` | 116,061,045 | `7e4906c2b9147dd6f974d382dbe1626e27ec9c69caa70f7167df9b31aca9dd72` |
| TriAevum | `v0.8.0-beta.1.2` | `TriAevum-v0.8.0-beta.1.2-Windows-x64.zip` | 550,467,290 | `23c3febe3a4dc1b7ffe652f21861f4c5b5068411a16df5fc721e52a80ba817a6` |
| TriAevum | `v0.8.0-beta.1.2` | `TriAevum-v0.8.0-beta.1.2-Linux-x86_64.AppImage` | 465,828,344 | `2e80fb50e1d21ffc5cc852a90f715408b82e65839e8baf8b3dbf6f9295d5296a` |
| TriAevum | `v0.8.0-beta.1.2` | `TriAevum-v0.8.0-beta.1.2-Linux-x86_64.flatpak` | 269,893,960 | `575db1812b37070e9512192bf760d5d78b9efda158b740a089a2eb1a528a54ef` |
| Ocarina ReTuned | `v0.6.8` | `Ocarina-ReTuned-0.6.8-Linux-x86_64.tar.gz` | 248,366,708 | `d06232f3b5c44d1647596137fa86f85fe24acaa9f95e74550209702b233885b3` |
| Ocarina ReTuned | `v0.6.8` | `Ocarina-ReTuned-0.6.8-Linux-ARM64.tar.gz` | 212,177,572 | `4a275b7a72546428b3ae0773c5918c04e7ea0192e4487957b0e90b402be4b843` |
| Ocarina ReTuned | `v0.6.8` | `Ocarina-ReTuned-0.6.7-Windows-x64.zip` | 222,737,102 | `5312d8204d29df36a6d8a0c71c83a92ca08eab5403f998d9bdf3e95810bd88a4` |
| Ocarina ReTuned | `v0.6.8` | `Ocarina-ReTuned-0.6.7-Windows-ARM64.zip` | 193,112,287 | `b3b0fed0b913f3dae5fa2052f10665e10a6275e0e598f74057ba76b1c12d5f60` |
| Ocarina ReTuned | `v0.6.8` | `Ocarina-ReTuned-0.6.6-Mac.zip` | 86,377,535 | `8666a19be74a84af9c28bc15bc0438f2bcd788fa7d325766e87c7dca338cbf00` |
| Ocarina ReTuned | `v0.6.8` | `Ocarina-ReTuned-0.6.5-Android-arm64.apk` | 140,921,338 | `8de3884a69d432d7d4ab983d47c869b4f6095d8bd751b8b5ad29b1c7a0a7c127` |

Verify a download locally, or drop the file into the in-browser SHA-256 checker on [ocarinarecomp.wiki](https://ocarinarecomp.wiki/) (WebCrypto, nothing is uploaded).

## November 11–12, 2026 release highlights

- **Ocarina Recomp `v0.3.4` (2026-11-11):** Upstream officially recommends **[Hookshot](https://ocarinarecomp.wiki/hookshot/)** for playing (`#212`) and shifts new runtime fixes there. `v0.3.4` adds `jogar\hookshot-preparar-jogo.bat` (unpacks `build\hookshot` with `romfs` and `exefs` folders for `HookshotBuilder.exe` even if you deleted the `.nup`) and `jogar\hookshot-copiar-save.bat` (`#216`), plus fixes for AMD RDNA 3 shader-prep freezes (`#208`), black Link in sunlight (`#91`), and Linux fullscreen/GPU choices (`#168`).
- **Hookshot `v2.1.0` (2026-11-11):** Expands the render-target pool to stop Castle Town guard-house crashes (`#1202`), supports >2 GB pipeline caches on Windows (`#1226`), and adds opt-in NVIDIA DLSS/DLAA/Reflex (`#841`), SDL gyro aiming (`#1114`), Switch Pro/Joy-Con HD rumble (`#1213`), 5.1 surround audio (`#1182`, `#1240`), Frame Generation Auto (`#1121`), and 4:3/16:10/5:4 aspect ratios (`#1224`). Guide: [Hookshot setup & migration](https://ocarinarecomp.wiki/hookshot/).
- **NX2navi `v0.8.0` (2026-11-11):** Cuts post-load hitches (1,374 ms to 115 ms entering Hyrule Field on RTX 5090), raises frame rates on NVIDIA and AMD, adds AMD FSR 4 upscaling on Radeon RX 6000/7000/9000 (driver 26.10.1+), a fallback for GPUs without mesh shaders, and fixes one-frame flashes and black frames. Guide: [NX2navi guide](https://ocarinarecomp.wiki/nx2navi/).
- **Ocarina ReTuned `v0.6.8` (2026-11-12 Linux Hotfix):** Fixes Linux ROM preparation failing to find bundled CMake and Ninja on direct app launch, following `v0.6.7` Windows portable mode, `v0.6.6` Mac CMake/Ninja fix, and `v0.6.5` Remake HUD preset. Guide: [Ocarina ReTuned guide](https://ocarinarecomp.wiki/ocarina-retuned/).

## Guides on ocarinarecomp.wiki

- [Hookshot vs Ocarina Recomp vs NX2navi comparison](https://ocarinarecomp.wiki/hookshot-vs-ocarina-recomp/)
- [All downloads and SHA-256 checksums](https://ocarinarecomp.wiki/download/)
- [System requirements (Vulkan 1.3, VRAM, RAM, page file)](https://ocarinarecomp.wiki/requirements/)
- [Compatibility status](https://ocarinarecomp.wiki/compatibility-status/) · [Troubleshooting](https://ocarinarecomp.wiki/troubleshooting/) · [Changelog](https://ocarinarecomp.wiki/changelog/)
- [Guia em português](https://ocarinarecomp.wiki/pt/) · [Guía en español](https://ocarinarecomp.wiki/es/)

---

Independent notes; not affiliated with the projects' developers or Nintendo. The Legend of Zelda and Ocarina of Time are trademarks of Nintendo. Text licensed CC BY 4.0.
