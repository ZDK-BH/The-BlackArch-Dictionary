# binwally

**Category:** `binary`  
**Version in source list:** `4.0aabd8b`  
**Package name:** `binwally`

## What it does

Binary and Directory tree comparison tool using the Fuzzy Hashing concept (ssdeep).

## What it can be used for

Static/dynamic analysis of binaries, exploit research, patch diffing, and malware triage.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed binwally
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql binwally | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
binwally --help
binwally -h
man binwally
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample, never the only copy of a binary.
2. Start with file identification, strings, metadata, and help output.
3. Open the sample in the tool and record architecture, imports, functions, and suspicious behavior.
4. Use results to understand software behavior or verify patches.

## Example commands

```bash
binwally --help
```

```bash
binwally -h
```

```bash
# Typical local sample pattern:
binwally ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
