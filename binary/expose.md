# expose

**Category:** `binary`  
**Version in source list:** `1110.30264af`  
**Package name:** `expose`

## What it does

A Dynamic Symbolic Execution (DSE) engine for JavaScript

## What it can be used for

Static/dynamic analysis of binaries, exploit research, patch diffing, and malware triage.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed expose
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql expose | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
expose --help
expose -h
man expose
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample, never the only copy of a binary.
2. Start with file identification, strings, metadata, and help output.
3. Open the sample in the tool and record architecture, imports, functions, and suspicious behavior.
4. Use results to understand software behavior or verify patches.

## Example commands

```bash
expose --help
```

```bash
expose -h
```

```bash
# Typical local sample pattern:
expose ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
