# marc4dasm

**Category:** `disassembler`  
**Version in source list:** `6.f11860f`  
**Package name:** `marc4dasm`

## What it does

A disassembler for the Atmel MARC4 (a 4 bit Harvard micro).

## What it can be used for

Inspecting machine code, bytecode, shellcode, firmware, and exploit/malware samples.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed marc4dasm
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql marc4dasm | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
marc4dasm --help
marc4dasm -h
man marc4dasm
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Identify architecture and file type before disassembly.
2. Load the sample locally and inspect functions, strings, and cross-references.
3. Avoid executing unknown samples unless the lab is isolated.
4. Use analysis notes to understand control flow and patch impact.

## Example commands

```bash
marc4dasm --help
```

```bash
marc4dasm -h
```

```bash
# Local disassembly pattern:
marc4dasm ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
