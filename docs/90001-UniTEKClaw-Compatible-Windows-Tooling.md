# UniTEKClaw Compatible Windows Tooling

**Document:** 90001
**Status:** v1.0
**Date:** 2026-05-16
**Author:** Bryan Fred
**AI attribution:** drafted in paired session with MyClaw.ai (Claude), reviewed and approved by Bryan Fred.

---

## 1. Purpose

This document is the companion to [`10005-Tool-Access-And-Certification-Model.md`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/10005-Tool-Access-And-Certification-Model.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/10005-Tool-Access-And-Certification-Model.md)) §6.3. It lists Windows-compatible compilers and IDEs that UniTEKClaw's Claws operate with, beyond the Recommended stack (Visual Studio Professional Subscription, DevExpress Ultimate Subscription).

The list is **maintained operational reference**, not a Foundation rule. It updates as new compilers become available, as tooling versions are tested for compatibility, and as the Foundation's language-neutral posture (per [`00029-Machine-Level-Integration.md`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/00029-Machine-Level-Integration.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/00029-Machine-Level-Integration.md)) §1) extends UniTEKClaw into new substrates.

The list is **guidelines, not absolutes** (per `10005` §6 framing). A Certified UniCORE Expert may operate with a combination not listed here; the public Discussion forums on the Foundation repositories are where any questions or proposals are raised.

---

## 2. Language coverage

UniTEKClaw supports development across two tracks, derived from the Foundation:

1. **The enterprise reference track** — .NET 10 / C# / XAF / XPO, plus the ordinary web/data/scripting languages a Certified Expert encounters in normal Solution work.
2. **The machine-level reference track** — C++ and the other machine-level languages enumerated in [`00029-Machine-Level-Integration.md`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/00029-Machine-Level-Integration.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/00029-Machine-Level-Integration.md)) §3, for firmware, embedded systems, real-time operating systems, robotic control, spacecraft avionics, and hardware-description targets (FPGA / ASIC).

The Claws operate across both tracks because the Foundation does. Governance must extend wherever the Solution operates.

---

## 3. Enterprise reference track tooling

### 3.1 .NET / C# / XAF / XPO

**Recommended (from [`10005`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/10005-Tool-Access-And-Certification-Model.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/10005-Tool-Access-And-Certification-Model.md)) §6.2):**

- **Visual Studio Professional Subscription** or higher edition (Enterprise). This is the canonical IDE for UniTEKClaw's own development and for producing applications that follow UniTEKClaw's pattern.
- **DevExpress Ultimate Subscription** — the full XAF (eXpressApp Framework) and XPO (eXpress Persistent Objects) stack, plus the wider DevExpress component library.

**Alternative:**

- **JetBrains Rider** — Cross-platform .NET IDE. Strong refactoring, debugger, and code-analysis tooling. Compatible with .NET SDK projects; XAF design-time tooling (XAF Model Editor, DevExpress design surfaces) is limited compared to Visual Studio. Suitable for Experts working on .NET code without the heavy XAF design surface.
- **Visual Studio Community Edition** — Free edition with the same compiler and most of the same tooling as Professional, subject to Microsoft's eligibility rules (individual developers, open-source, small organisations, classroom use). Where eligibility permits, Community is fully sufficient for UniTEKClaw work.
- **`dotnet` CLI (SDK only)** — Command-line .NET build, test, run. Sufficient for compile/test cycles without any IDE; useful for headless build agents or for Experts working in editors that are not IDEs (Visual Studio Code, Neovim, Emacs).

**Compilers / runtimes:**

- **MSBuild** — the canonical .NET build engine. Bundled with Visual Studio and with the .NET SDK.
- **Roslyn** — the C# compiler. Bundled with the .NET SDK.

### 3.2 JavaScript / TypeScript

UniTEKClaw users producing web frontends for their Solutions encounter JavaScript and TypeScript. Common cases: Blazor + TypeScript interop, ASP.NET MVC views, React/Vue/Angular Solution frontends, browser-based AI prototypes.

**Recommended:**

- **Visual Studio Code** — Microsoft's free cross-platform editor. Strong TypeScript/JavaScript tooling, integrated terminal, Git, extension ecosystem. Free of charge.
- **Visual Studio Professional / Enterprise** — first-class TypeScript and JavaScript support for ASP.NET integrated work.

**Alternative:**

- **JetBrains WebStorm** — Commercial editor specialised for JavaScript/TypeScript.
- **Sublime Text / Notepad++ / Vim / Neovim / Emacs** — General-purpose text editors with TypeScript/JavaScript language-server support.

**Compilers / runtimes:**

- **TypeScript compiler (`tsc`)** — bundled with `typescript` npm package.
- **Node.js + npm/yarn/pnpm** — JavaScript runtime + package management.
- **esbuild / swc / Vite / webpack** — modern build pipelines, choice depends on the Solution's frontend stack.

### 3.3 Python

UniTEKClaw users may use Python for data processing, scripting, scientific computing, ML preprocessing, and integration with Python-only libraries.

**Recommended:**

- **Visual Studio Code with Python extension** — Free, full-featured Python development including debugger, formatter, linter.
- **Visual Studio (Python Tools for Visual Studio, PTVS)** — first-class Python support in Visual Studio Professional / Enterprise.

**Alternative:**

- **JetBrains PyCharm Professional or Community** — Commercial (Pro) or free (Community) Python IDE.
- **JupyterLab / Jupyter Notebook** — Notebook environment for exploratory work.
- **Plain editor + `python` CLI** — for command-line work and scripting.

**Compilers / runtimes:**

- **CPython** — the reference Python interpreter, from python.org. The standard choice on Windows.
- **PyPy** — alternative interpreter with JIT compilation, for performance-critical scripts.

### 3.4 SQL

UniTEKClaw requires SQL Server Express at minimum (per [`10005`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/10005-Tool-Access-And-Certification-Model.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/10005-Tool-Access-And-Certification-Model.md)) §6.1). SQL development tooling is essential.

**Recommended:**

- **SQL Server Management Studio (SSMS)** — Microsoft's free management and query tool for SQL Server. Standard for SQL Server work on Windows.
- **Azure Data Studio** — Microsoft's modern, cross-platform alternative. Free.

**Alternative:**

- **JetBrains DataGrip** — Commercial multi-database IDE. Strong cross-database SQL tooling.
- **DBeaver Community / Enterprise** — Free (Community) or commercial (Enterprise) multi-database tool.
- **Visual Studio + SQL Server Data Tools (SSDT)** — Database project work integrated with Visual Studio.

### 3.5 PowerShell and shell scripting

For Windows automation, build scripts, deployment, and operational glue.

**Recommended:**

- **PowerShell 7+ (Core)** — Cross-platform, current PowerShell. Bundled with Windows or installable via winget / MSI.
- **Visual Studio Code with PowerShell extension** — Free editor with full PowerShell debugging.

**Alternative:**

- **Windows PowerShell ISE** — Legacy PowerShell 5.1 editor, bundled with older Windows. Use PowerShell 7+ for new work.
- **WSL (Windows Subsystem for Linux)** — Runs bash, zsh, fish, and other Unix shells natively on Windows. Useful for Experts comfortable with Unix tooling.
- **Git Bash** — Lightweight bash environment bundled with Git for Windows.

---

## 4. Machine-level reference track tooling

Per [`00029-Machine-Level-Integration.md`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/00029-Machine-Level-Integration.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/00029-Machine-Level-Integration.md)) §3, the Foundation supports C++ (primary machine-level reference), C, Rust, Ada / SPARK, Assembly, Verilog / VHDL, and any other machine-level language adopted by humans for safety-critical domains.

UniTEKClaw operates with the toolchains for these languages on Windows. The Claws can pair with an Expert producing firmware, embedded systems, real-time operating systems, robotic control loops, spacecraft avionics, hibernation life-support controllers, or hardware-description code, the same way they pair on .NET work.

### 4.1 C++

**Recommended:**

- **Visual Studio Professional / Enterprise** with the **Desktop development with C++** workload. The Microsoft Visual C++ (MSVC) compiler is canonical for Windows C++ work.

**Alternative:**

- **Visual Studio Code with C/C++ extension + a compiler** — Free editor, paired with a compiler of choice.
- **JetBrains CLion** — Commercial cross-platform C/C++ IDE.
- **Qt Creator** — Cross-platform C++ IDE, particularly suited to Qt-based GUI work.
- **CodeBlocks** — Free, open-source C/C++ IDE.

**Compilers (Windows-compatible):**

- **MSVC (Microsoft Visual C++)** — Bundled with Visual Studio. The Windows reference compiler.
- **MinGW-w64 (GCC for Windows)** — GCC ported to Windows. Standalone, free.
- **Clang / LLVM for Windows** — Apple's compiler stack, available on Windows via the LLVM project or via Visual Studio's `clang-cl` integration.
- **Intel C++ Compiler (icx / icpx)** — Commercial, focused on high-performance computing.

### 4.2 C

C is a subset of C++ in tooling terms — every C++ compiler listed in §4.1 also compiles C. The same IDEs apply. The Expert chooses C-mode compilation (`/std:c11`, `/std:c17`, or equivalent) when producing C rather than C++ code.

For embedded / RTOS / firmware work specifically:

**Compilers (cross-compiled for embedded targets, hosted on Windows):**

- **ARM GCC (`arm-none-eabi-gcc`)** — Cross-compiler for ARM Cortex-M, the dominant embedded MCU family.
- **Keil MDK (ARM)** — Commercial, IDE + compiler bundle for ARM development.
- **IAR Embedded Workbench** — Commercial, multi-architecture embedded IDE.
- **SEGGER Embedded Studio** — Commercial, free for some uses, multi-architecture.

### 4.3 Rust

**Recommended:**

- **Visual Studio Code with rust-analyzer extension** — Free, the standard Rust development environment on Windows.

**Alternative:**

- **JetBrains RustRover** — JetBrains' dedicated Rust IDE (commercial).
- **JetBrains CLion + IntelliJ Rust plugin** — older path, still supported.
- **Visual Studio with Rust Tools** — Microsoft's Rust support is improving but not the primary path.

**Compilers / toolchain:**

- **`rustc`** + **`cargo`** via **rustup** — the canonical Rust toolchain, free, cross-platform. The Windows installer at `rustup.rs` installs everything needed.

### 4.4 Ada / SPARK

For aerospace, defence, and safety-critical work where SPARK's formal verification matters.

**Recommended:**

- **GNAT Studio** — AdaCore's Ada IDE. Commercial editions and a free GPL edition (GNAT Community).

**Alternative:**

- **Visual Studio Code with Ada extension** — Lightweight editor integration.

**Compilers:**

- **GNAT (GCC for Ada)** — the reference Ada compiler, available in GNAT Community (free) and GNAT Pro (commercial, AdaCore).
- **SPARK Pro** — AdaCore's formal verification toolset for SPARK subset.

### 4.5 Assembly

For low-level work where high-level languages are insufficient, bounded and reviewed per [`00029`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/00029-Machine-Level-Integration.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/00029-Machine-Level-Integration.md)) §3.

**Tooling:**

- **MASM (Microsoft Macro Assembler)** — Bundled with Visual Studio. Canonical Windows x86 / x64 assembler.
- **NASM (Netwide Assembler)** — Free, multi-format, multi-platform assembler.
- **YASM** — Modular assembler, NASM-compatible syntax.
- **GAS (GNU Assembler)** — Bundled with GCC / MinGW-w64. AT&T syntax.
- **`fasm` (flat assembler)** — Free, self-hosting assembler.

For cross-architecture work (ARM assembly, RISC-V assembly), the same GCC / LLVM cross-toolchains in §4.2 apply.

### 4.6 Verilog / VHDL (hardware description)

For FPGA / ASIC enforcement of governance, per [`00029`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/00029-Machine-Level-Integration.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/00029-Machine-Level-Integration.md)) §5.3.

**Recommended (vendor-specific, depending on target FPGA):**

- **AMD/Xilinx Vivado** — Commercial, free WebPACK edition available, for Xilinx FPGAs.
- **Intel/Altera Quartus Prime** — Commercial, free Lite edition available, for Intel FPGAs.
- **Lattice Diamond / Radiant** — Free editions for Lattice FPGAs.
- **Microchip Libero SoC** — Free Silver edition for Microchip / Microsemi FPGAs.

**Alternative (vendor-neutral):**

- **Visual Studio Code with Verilog HDL / SystemVerilog / VHDL extensions** — Lightweight editing.
- **Verilator** — Open-source Verilog simulator for testbench-driven verification.
- **GHDL** — Open-source VHDL simulator.
- **Icarus Verilog** — Open-source Verilog simulator.

### 4.7 Other machine-level languages

Per [`00029`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/00029-Machine-Level-Integration.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/00029-Machine-Level-Integration.md)) §3, the Foundation accepts "any other machine-level language adopted by humans for safety-critical domains." If an Expert is producing Foundation-aligned work in a language not listed above, the Discussion forums on the Foundation repositories are the place to propose its addition to this document.

Candidate languages that may be added as use cases arise:

- **D** — systems language, GCC and LLVM backends.
- **Zig** — modern systems language, ships its own toolchain.
- **Go** — when targeting cross-platform services or systems work that does not require manual memory management.
- **Nim** — systems language with garbage collection.
- **OCaml / F#** — typed functional languages used in some defence / aerospace contexts (F# is .NET; OCaml has independent toolchains).
- **Erlang / Elixir** — for fault-tolerant concurrent systems (BEAM VM).

---

## 5. Cross-cutting tooling

Independent of language, UniTEKClaw users will use:

### 5.1 Version control

- **Git** for Windows (`git-scm.com`). Required for any work touching public Foundation repositories. Note: UniTEKClaw itself is forbidden from accessing the three public Foundation repositories (UniVERSE, TrueAI, UniCORE-AI) via GitHub per the read-only-non-GitHub rule; that rule applies to the UniTEKClaw application, not to the Expert's general use of Git.
- **GitHub Desktop**, **TortoiseGit**, **GitKraken**, **Sourcetree**, or **Fork** for GUI Git workflows.
- **Visual Studio Git integration** for in-IDE Git.

### 5.2 Containers and virtualisation

- **Docker Desktop for Windows** — for containerised Solutions.
- **Podman Desktop** — alternative to Docker Desktop.
- **WSL 2** — Microsoft's Linux subsystem; useful for Linux-targeted Solutions and for running Unix toolchains natively.
- **Hyper-V** / **VirtualBox** / **VMware Workstation** — for the separate-machine boundary in [`10005`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/10005-Tool-Access-And-Certification-Model.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/10005-Tool-Access-And-Certification-Model.md)) §3.6, or for virtualised test targets. (Note: virtualisation is not a substitute for the physical separate machine required for non-Foundation work; see `10005` §3.6.)

### 5.3 Editors that work across all languages

For Experts who prefer a single editor across all languages they touch:

- **Visual Studio Code** — Microsoft's free editor. Strong extension ecosystem covering every language above. The most common single-editor choice on Windows.
- **JetBrains Fleet** — JetBrains' polyglot editor (in development at time of writing).
- **Sublime Text** — commercial, fast, lightweight.
- **Vim / Neovim** — for Experts who prefer modal editing.
- **Emacs** — for Experts who prefer the Emacs paradigm.

### 5.4 AI assistants outside UniTEKClaw

When a Certified Expert works **inside** UniTEKClaw, the paired AgentClaw is the only AI they pair with for Foundation work. **Outside** UniTEKClaw (on the separate non-Foundation machine, on different projects, in ordinary editor use), other AI assistants — GitHub Copilot, Cursor, Codeium, Tabnine, JetBrains AI Assistant, Claude Code, Codex, and so on — may be used at the Expert's discretion. These are not regulated by this document or by `10005`; they fall outside Foundation scope when used outside Foundation work.

---

## 6. What this document does not cover

- **The Recommended-stack version pinning.** Specific Visual Studio versions, specific DevExpress release numbers, specific .NET SDK versions are tracked in the UniTEKClaw release notes, not here.
- **Cloud provider tooling.** AWS, Azure, GCP, and other cloud SDKs and CLIs are language-agnostic and are not enumerated here.
- **Test frameworks.** xUnit / NUnit / MSTest / FluentAssertions / Moq / Bogus / Verify and their counterparts in other languages are testing concerns, not compiler / IDE concerns.
- **Static analysis and linters.** SonarQube, Roslyn analysers, clang-tidy, cppcheck, pylint, rustfmt, and the rest are quality concerns, recommended but not gated here.
- **The Foundation language-neutral posture itself.** That is locked in [`00029-Machine-Level-Integration.md`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/00029-Machine-Level-Integration.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/00029-Machine-Level-Integration.md)) §1. This document is operational reference, not Foundation policy.

---

## 7. Cross-references

| Document | Relationship |
|---|---|
| [`10005-Tool-Access-And-Certification-Model.md`](https://git.unitek-systems.com/UniCORE/TrueAI/src/branch/main/docs/10005-Tool-Access-And-Certification-Model.md) (mirror: [GitHub](https://github.com/bryanunitek/TrueAI/blob/main/docs/10005-Tool-Access-And-Certification-Model.md)) | §6.3 references this document as the Alternative tier of the three-tier software prerequisites |
| [`00029-Machine-Level-Integration.md`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/00029-Machine-Level-Integration.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/00029-Machine-Level-Integration.md)) | §3 enumerates the machine-level languages this document provides tooling lists for |
| [`00060-Supported-AI-Provider-List.md`](https://git.unitek-systems.com/UniCORE/UniVERSE/src/branch/main/docs/00060-Supported-AI-Provider-List.md) (mirror: [GitHub](https://github.com/bryanunitek/UniVERSE/blob/main/docs/00060-Supported-AI-Provider-List.md)) | Companion list for AI providers (Anthropic, OpenAI, etc.) the paired AgentClaw inside UniTEKClaw can connect to; this document lists compilers / IDEs the Expert pairs with the AgentClaw to use |

---

## 8. Document history

| Version | Date | Author | Change |
|---|---|---|---|
| 1.0 | 2026-05-16 | Bryan Fred | Initial compatible-tooling list. Enterprise reference track (.NET / C# / XAF / XPO, JavaScript / TypeScript, Python, SQL, PowerShell). Machine-level reference track (C++, C, Rust, Ada / SPARK, Assembly, Verilog / VHDL, plus candidate-language note). Cross-cutting tooling (version control, containers, editors, external AI assistants). |
