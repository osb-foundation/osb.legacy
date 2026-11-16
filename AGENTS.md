# AGENTS.md — OSB Legacy

This file guides coding agents working in the `osb.legacy` repository.

## Project Identity

**OSB Legacy** preserves the original BASIC source code of OSB (created in Basic/BC7) and the legacy hosted .NET shell implementation. This repository serves as historical reference and source material for porting legacy features.

## Code Policy

1. **Preservation Priority**
   - This is a legacy/archive repository.
   - Preserve original code as-is for historical reference.
   - Do not modernize or refactor legacy code.

2. **BASIC Source (original-src/)**
   - Original code from the BASIC/BC7 era.
   - Preserve formatting, comments, and structure.
   - Reference only for porting to modern implementations.

3. **Legacy Shell (legacy-shell/)**
   - Old hosted .NET shell implementation.
   - Predecessor to the current userspace shell.
   - May be referenced when porting features to the new architecture.

## Architecture

### original-src/
- Original BASIC source files (.BAS)
- Compiled binaries (.COM, .EXE)
- Configuration and help files
- XWIN animations and effects

### legacy-shell/
- C# hosted shell implementation
- Environment and configuration management
- Command modules (File, System, etc.)
- Apps (Calendar, Hangman, etc.)
- I18N support

## Build and Validation

```bash
# Legacy shell (if building)
cd legacy-shell
dotnet build
```

## Change Workflow for Agents

1. Inspect relevant files first.
2. Preserve original code as-is.
3. Document any changes made for reference.
4. Do not break historical accuracy.

## Non-Goals and Cautions

- Do not modernize or refactor legacy code.
- Do not remove original files.
- Do not introduce new dependencies to legacy code.

## Documentation Anchors

- `README.md`: High-level project/user documentation.