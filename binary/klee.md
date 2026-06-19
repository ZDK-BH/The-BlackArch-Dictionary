# klee

**Category:** `binary`  
**Version in source list:** `2.1`  
**Package name:** `klee`

## What it does

A symbolic virtual machine built on top of the LLVM compiler infrastructure.

## What it can be used for

Static/dynamic analysis of binaries, exploit research, patch diffing, and malware triage.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed klee
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql klee | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
klee --help
klee -h
man klee
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample, never the only copy of a binary.
2. Start with file identification, strings, metadata, and help output.
3. Open the sample in the tool and record architecture, imports, functions, and suspicious behavior.
4. Use results to understand software behavior or verify patches.

## Example commands

```bash
klee --help
```

```bash
klee -h
```

```bash
# Typical local sample pattern:
klee ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
