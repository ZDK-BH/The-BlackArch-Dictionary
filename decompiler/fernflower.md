# fernflower

**Category:** `decompiler`  
**Version in source list:** `802.c03cae7a`  
**Package name:** `fernflower`

## What it does

An analytical decompiler for Java.

## What it can be used for

Recovering higher-level structure from binaries, bytecode, mobile apps, or .NET/Java artifacts.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed fernflower
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql fernflower | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
fernflower --help
fernflower -h
man fernflower
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample file.
2. Open the binary or package in read-only analysis mode if available.
3. Review classes/functions/resources rather than executing unknown code.
4. Export notes, pseudocode, or reports for later review.

## Example commands

```bash
fernflower --help
```

```bash
fernflower -h
```

```bash
# Local sample pattern:
fernflower ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
