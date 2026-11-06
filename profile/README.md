<p align="center">
  <img src="https://raw.githubusercontent.com/ps2build/.github/main/profile/icon.png" alt="ps2build" width="120">
</p>

<h1 align="center">PS2BUILD</h1>

<h3 align="center">The modern build platform for PlayStation 2 development.</h3>

<p align="center">
  <a href="https://github.com/ps2build/ps2build/releases">Download</a> ·
  <a href="https://ps2build.dev">Documentation</a> ·
  <a href="https://github.com/ps2build/ps2build-samples">Samples</a> ·
  <a href="https://github.com/ps2build/ps2build/issues">Support</a>
</p>

---

## Overview

ps2build is an end-to-end platform for building PlayStation 2 software. One declarative `ps2.yaml` describes your Emotion Engine (EE) and I/O Processor (IOP) targets. ps2build generates the build, IDE metadata and installable packages, and keeps the SDK and compilers up to date.

| | |
|---|---|
| **Declarative builds** | Describe `ee`, `iop`, `ee_lib` and `iop_lib` targets in one file. No hand-written Makefiles. |
| **Two compilers** | Build with the GCC or LLVM toolchain, including a PS2-aware LLVM fork for R5900 and R3000A. |
| **Self-updating SDK** | `ps2build update` installs and upgrades the toolchain, SDK and tools. Each component versions independently. |
| **IDE ready** | Emits `compile_commands.json` and a JSON Schema for `ps2.yaml` completion. |
| **Package ecosystem** | Build and install libraries into the SDK, and consume them from other projects. |
| **Automation** | Built-in MCP server, plus GitHub Actions for CI. |

## Get started

Install on Linux or macOS:

```
curl -sSfL https://ps2build.dev/install.sh | sh
```

Install on Windows (PowerShell):

```
irm https://ps2build.dev/install.ps1 | iex
```

Then create and build a project:

```
ps2build init my-game
cd my-game
ps2build build
```

## Platform

| Area | Repositories |
|---|---|
| **Build system** | [ps2build](https://github.com/ps2build/ps2build) · [manifest](https://github.com/ps2build/manifest) · [ninja](https://github.com/ps2build/ninja) · [cmake](https://github.com/ps2build/cmake) |
| **Toolchains** | [toolchain](https://github.com/ps2build/toolchain) · [llvm-toolchain](https://github.com/ps2build/llvm-toolchain) · [llvm](https://github.com/ps2build/llvm) · [gcc](https://github.com/ps2build/gcc) · [binutils-gdb](https://github.com/ps2build/binutils-gdb) · [newlib](https://github.com/ps2build/newlib) · [newlib-llvm](https://github.com/ps2build/newlib-llvm) |
| **SDK** | [sdk-core](https://github.com/ps2build/sdk-core) · [sdk-world](https://github.com/ps2build/sdk-world) · [ps2_drivers](https://github.com/ps2build/ps2_drivers) · [pthread-embedded](https://github.com/ps2build/pthread-embedded) |
| **Libraries** | [ps2gl](https://github.com/ps2build/ps2gl) · [ps2stuff](https://github.com/ps2build/ps2stuff) · [romfs](https://github.com/ps2build/romfs) · [freetype](https://github.com/ps2build/freetype) · [libjpeg-turbo](https://github.com/ps2build/libjpeg-turbo) · [ogg](https://github.com/ps2build/ogg) · [vorbis](https://github.com/ps2build/vorbis) |
| **Developer tools** | [tools](https://github.com/ps2build/tools) · [vcl](https://github.com/ps2build/vcl) |
| **CI** | [setup-sdk](https://github.com/ps2build/setup-sdk) |
| **Learn** | [docs](https://github.com/ps2build/docs) · [ps2build-samples](https://github.com/ps2build/ps2build-samples) |

## Open source

ps2build is released under CC0 1.0 Universal. Third-party components keep their own licenses, listed in each repository.

## Contributing

Contributions are welcome. Read the `CONTRIBUTING.md` in the repository you want to change, and open an issue before starting large work.

---

<p align="center"><sub>PlayStation and PS2 are trademarks of Sony Interactive Entertainment Inc. ps2build is an independent project and is not affiliated with or endorsed by Sony.</sub></p>
