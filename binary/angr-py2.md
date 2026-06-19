# angr-py2

**Category:** `binary`  
**Version in source list:** `7.8.9.26`  
**Package name:** `angr-py2`

## What it does

The next-generation binary analysis platform from UC Santa Barbaras Seclab.

## What it can be used for

Static/dynamic analysis of binaries, exploit research, patch diffing, and malware triage.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed angr-py2
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql angr-py2 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
angr-py2 --help
angr-py2 -h
man angr-py2
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample, never the only copy of a binary.
2. Start with file identification, strings, metadata, and help output.
3. Open the sample in the tool and record architecture, imports, functions, and suspicious behavior.
4. Use results to understand software behavior or verify patches.

## Example commands

```bash
angr-py2 --help
```

```bash
angr-py2 -h
```

```bash
# Typical local sample pattern:
angr-py2 ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
