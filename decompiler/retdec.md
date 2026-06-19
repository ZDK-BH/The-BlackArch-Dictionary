# retdec

**Category:** `decompiler`  
**Version in source list:** `2161.04df6def`  
**Package name:** `retdec`

## What it does

Retargetable machine-code decompiler based on LLVM.

## What it can be used for

Recovering higher-level structure from binaries, bytecode, mobile apps, or .NET/Java artifacts.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed retdec
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql retdec | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
retdec --help
retdec -h
man retdec
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample file.
2. Open the binary or package in read-only analysis mode if available.
3. Review classes/functions/resources rather than executing unknown code.
4. Export notes, pseudocode, or reports for later review.

## Example commands

```bash
retdec --help
```

```bash
retdec -h
```

```bash
# Local sample pattern:
retdec ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
