# salinewin-source-code

> **⚠️ Security research / source-code archive**
>
> This repository contains the source tree for **salinewin** and a separate **salinewin-safety** project. Some components are low-level Windows code and may interact with disk or boot-related functionality. Treat the repository as untrusted code and do not build or execute it on a production machine.

## 🍂 Autumn Season Coming

**Autumn 2026 is coming. 🍁**

> 🍂 **Autumn Season 2026 — Coming Soon**  
> 🌅 September 23, 2026  
> 🍁 A new season, a new chapter.

This seasonal notice is an informational update for the repository. Development and source-code safety guidance remain unchanged.

## 📦 Archive Status

**Archive is allowed.**

This repository may be preserved as a historical source-code archive. Archiving means the existing source, documentation, and version history can remain available for reference while active development is paused or ended.

- **Archive:** Allowed
- **Source history:** Preserved
- **Future changes:** Optional
- **Safety guidance:** Remains in effect
- **Repository access:** Existing GitHub access rules still apply

Archival status does not make the code safe to build or execute. Review all source code before using it.

## Repository status

- **Repository:** `arnikipad/salinewin-source-code`
- **Branch:** `main`
- **Purpose:** Source-code archive and research reference
- **Platform:** Windows / Visual Studio project files
- **Public repository:** Yes

## Projects

### `salinewin/`

The main Visual Studio solution is located at:

`salinewin/salinewin.sln`

The project tree currently includes:

- `PayloadMBR/` — low-level payload-related source tree
- `salinewin/` — application source tree
- `Release/` — release/build output directory
- `x64/` — x64 build directory

Because the repository contains low-level components, review the source carefully before compiling or running anything.

### `salinewin-safety/`

A separate Visual Studio solution is provided at:

`salinewin-safety/salinewin-safety.sln`

Its repository tree includes its own:

- `salinewin/` source directory
- `Release/` build directory
- `x64/` build directory

Use the safety project when working on non-destructive testing, documentation, or defensive development.

## ⚠️ Safety notice

This repository is **not intended for use on systems or data that you cannot afford to lose**.

Before compiling unfamiliar low-level code:

1. Read the source code completely.
2. Use an isolated virtual machine or disposable test environment.
3. Do not run it with administrator privileges unless you have explicitly verified every privileged operation.
4. Keep important files and backups outside the test environment.
5. Do not test disk, boot-sector, partition, or recovery-related functionality on a real production installation.
6. If you are unsure what a component does, do not execute it.

The presence of source code in this repository does **not** mean that a binary is safe to execute.

## Building

The repository contains Visual Studio solution files. If you are reviewing the project for legitimate development or security research:

1. Clone the repository.
2. Open the appropriate `.sln` file in Visual Studio.
3. Review project dependencies and build configuration.
4. Prefer a disposable Windows virtual machine for compilation and testing.
5. Inspect generated binaries before executing them.

Do not assume that a successful compilation means the resulting program is safe.

## Responsible use

Use this repository for:

- source-code study
- defensive security research
- malware-analysis education in an isolated lab
- compatibility and build-system research
- development of safer test implementations

Do not use it to damage systems, destroy data, bypass security controls, or deploy destructive functionality against systems without authorization.

## Contributions

When contributing, prefer changes that improve:

- safety
- documentation
- reproducibility
- isolated testing
- defensive analysis
- clear warnings around privileged or destructive operations

Avoid adding functionality whose primary purpose is destructive or unauthorized system modification.

## Disclaimer

The repository is provided for educational, research, and development purposes. You are responsible for understanding and testing code before running it and for complying with applicable laws, policies, and authorization requirements.

---

**Status:** Source-code archive / security-research project  
**Archive:** 📦 Allowed  
**Season:** 🍂 Autumn 2026 — Coming Soon  
**Safety:** Review before build or execution
