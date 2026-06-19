# python-uncompyle6

**Category:** `decompiler`  
**Version in source list:** `3.9.3`  
**Package name:** `python-uncompyle6`

## What it does

A Python cross-version decompiler.

## What it can be used for

Recovering higher-level structure from binaries, bytecode, mobile apps, or .NET/Java artifacts.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed python-uncompyle6
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql python-uncompyle6 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
python-uncompyle6 --help
python-uncompyle6 -h
man python-uncompyle6
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample file.
2. Open the binary or package in read-only analysis mode if available.
3. Review classes/functions/resources rather than executing unknown code.
4. Export notes, pseudocode, or reports for later review.

## Example commands

```bash
python-uncompyle6 --help
```

```bash
python-uncompyle6 -h
```

```bash
# Local sample pattern:
python-uncompyle6 ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
