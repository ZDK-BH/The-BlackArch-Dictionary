# recaf

**Category:** `decompiler`  
**Version in source list:** `4.0.0.alpha.r22.g709b3f9`  
**Package name:** `recaf`

## What it does

Modern Java bytecode editor.

## What it can be used for

Recovering higher-level structure from binaries, bytecode, mobile apps, or .NET/Java artifacts.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed recaf
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql recaf | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
recaf --help
recaf -h
man recaf
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample file.
2. Open the binary or package in read-only analysis mode if available.
3. Review classes/functions/resources rather than executing unknown code.
4. Export notes, pseudocode, or reports for later review.

## Example commands

```bash
recaf --help
```

```bash
recaf -h
```

```bash
# Local sample pattern:
recaf ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
