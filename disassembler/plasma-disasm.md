# plasma-disasm

**Category:** `disassembler`  
**Version in source list:** `922.ec7df9b`  
**Package name:** `plasma-disasm`

## What it does

An interactive disassembler for x86/ARM/MIPS. It can generates indented pseudo-code with colored syntax.

## What it can be used for

Inspecting machine code, bytecode, shellcode, firmware, and exploit/malware samples.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed plasma-disasm
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql plasma-disasm | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
plasma-disasm --help
plasma-disasm -h
man plasma-disasm
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Identify architecture and file type before disassembly.
2. Load the sample locally and inspect functions, strings, and cross-references.
3. Avoid executing unknown samples unless the lab is isolated.
4. Use analysis notes to understand control flow and patch impact.

## Example commands

```bash
plasma-disasm --help
```

```bash
plasma-disasm -h
```

```bash
# Local disassembly pattern:
plasma-disasm ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
