# jpexs-decompiler

**Category:** `decompiler`  
**Version in source list:** `15.1.0`  
**Package name:** `jpexs-decompiler`

## What it does

JPEXS Free Flash Decompiler.

## What it can be used for

Recovering higher-level structure from binaries, bytecode, mobile apps, or .NET/Java artifacts.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed jpexs-decompiler
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql jpexs-decompiler | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
jpexs-decompiler --help
jpexs-decompiler -h
man jpexs-decompiler
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample file.
2. Open the binary or package in read-only analysis mode if available.
3. Review classes/functions/resources rather than executing unknown code.
4. Export notes, pseudocode, or reports for later review.

## Example commands

```bash
jpexs-decompiler --help
```

```bash
jpexs-decompiler -h
```

```bash
# Local sample pattern:
jpexs-decompiler ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
