# OSB Legacy

Original source code and legacy implementations for OSB (Operating System Basic).

## Overview

This repository preserves the original BASIC source code of OSB, created by the project owner between ages 14-16 in Basic (BC7), nearly 30 years ago. It also contains the legacy hosted shell implementation that was the predecessor to the current userspace shell.

## Contents

### original-src/
The original BASIC source code including:
- **OSB.BAS** - Main kernel/shell source
- **XWIN/** - XWIN animations and effects (RADIAIS, CIRCULOS, COMPLEX, LINHAS, FOGO)
- **CONF/** - Configuration files
- **HELP/** - Help system
- **APLIC/** - Application files
- **GAMES/** - Game files
- Various `.COM` and `.EXE` compiled binaries

### legacy-shell/
The legacy hosted .NET shell implementation that preceded the current userspace shell architecture. This includes:
- **Program.cs** - Main shell entry point
- **Kernel/** - Shell environment, config, and command modules
- **Apps/** - Applications (Calendar, Hangman, etc.)
- **Games/** - Games
- **CONF/** - Configuration files (OSB.HLP, etc.)
- **I18N/** - Internationalization files

## Purpose

This repository serves as:
- Historical reference for the original OSB implementation
- Source material for porting legacy features to the new architecture
- Documentation of the evolution from BASIC to modern .NET

## Building (Legacy Shell)

```bash
cd legacy-shell
dotnet build
```

## Part of OSB

This is part of the [OSB](https://github.com/osb-system) - Operating System Basic project, a DOS-like operating system built from scratch.

## License

MIT License - see [LICENSE](LICENSE) for details.