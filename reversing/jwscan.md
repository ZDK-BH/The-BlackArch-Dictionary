# jwscan

**Category:** `reversing`  
**Version in source list:** `7.874b3a5`  
**Package name:** `jwscan`

## What it does

Scanner for Jar to EXE wrapper like Launch4j, Exe4j, JSmooth, Jar2Exe.

## What it can be used for

Understanding compiled software, file formats, protocols, obfuscation, and malware samples.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed jwscan
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql jwscan | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
jwscan --help
jwscan -h
man jwscan
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on copied samples in a lab directory.
2. Begin with metadata, strings, and static inspection.
3. Use decompilation/disassembly features to map behavior.
4. Keep notes about functions, resources, and suspicious code paths.

## Example commands

```bash
jwscan --help
```

```bash
jwscan -h
```

```bash
# Local sample pattern:
jwscan ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
