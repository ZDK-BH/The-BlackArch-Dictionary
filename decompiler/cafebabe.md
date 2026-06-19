# cafebabe

**Category:** `decompiler`  
**Version in source list:** `0.1.2`  
**Package name:** `cafebabe`

## What it does

Java bytecode editor & decompiler.

## What it can be used for

Recovering higher-level structure from binaries, bytecode, mobile apps, or .NET/Java artifacts.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed cafebabe
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql cafebabe | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
cafebabe --help
cafebabe -h
man cafebabe
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample file.
2. Open the binary or package in read-only analysis mode if available.
3. Review classes/functions/resources rather than executing unknown code.
4. Export notes, pseudocode, or reports for later review.

## Example commands

```bash
cafebabe --help
```

```bash
cafebabe -h
```

```bash
# Local sample pattern:
cafebabe ./sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
