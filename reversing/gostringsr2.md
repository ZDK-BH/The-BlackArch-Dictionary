# gostringsr2

**Category:** `reversing`  
**Version in source list:** `1.1.2`  
**Package name:** `gostringsr2`

## What it does

Extract strings from a Go binary using radare2.

## What it can be used for

Understanding compiled software, file formats, protocols, obfuscation, and malware samples.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed gostringsr2
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql gostringsr2 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
gostringsr2 --help
gostringsr2 -h
man gostringsr2
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on copied samples in a lab directory.
2. Begin with metadata, strings, and static inspection.
3. Use decompilation/disassembly features to map behavior.
4. Keep notes about functions, resources, and suspicious code paths.

## Example commands

```bash
gostringsr2 --help
```

```bash
gostringsr2 -h
```

```bash
# Local sample pattern:
gostringsr2 ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
