# syms2elf

**Category:** `reversing`  
**Version in source list:** `12.329c2ce`  
**Package name:** `syms2elf`

## What it does

A plugin for Hex-Ray's IDA Pro and radare2 to export the symbols recognized to the ELF symbol table.

## What it can be used for

Understanding compiled software, file formats, protocols, obfuscation, and malware samples.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed syms2elf
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql syms2elf | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
syms2elf --help
syms2elf -h
man syms2elf
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on copied samples in a lab directory.
2. Begin with metadata, strings, and static inspection.
3. Use decompilation/disassembly features to map behavior.
4. Keep notes about functions, resources, and suspicious code paths.

## Example commands

```bash
syms2elf --help
```

```bash
syms2elf -h
```

```bash
# Local sample pattern:
syms2elf ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
