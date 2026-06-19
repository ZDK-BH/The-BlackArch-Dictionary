# binaryninja

**Category:** `reversing`  
**Version in source list:** `5.3.9757`  
**Package name:** `binaryninja`

## What it does

A new kind of reversing platform (demo version).

## What it can be used for

Understanding compiled software, file formats, protocols, obfuscation, and malware samples.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed binaryninja
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql binaryninja | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
binaryninja --help
binaryninja -h
man binaryninja
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on copied samples in a lab directory.
2. Begin with metadata, strings, and static inspection.
3. Use decompilation/disassembly features to map behavior.
4. Keep notes about functions, resources, and suspicious code paths.

## Example commands

```bash
binaryninja --help
```

```bash
binaryninja -h
```

```bash
# Local sample pattern:
binaryninja ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
