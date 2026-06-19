# shelling

**Category:** `misc`  
**Version in source list:** `227.0a6c135`  
**Package name:** `shelling`

## What it does

An offensive approach to the anatomy of improperly written OS command injection sanitisers.

## What it can be used for

Supporting security workflows such as encoding, parsing, helper automation, lookup, or specialized analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed shelling
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql shelling | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
shelling --help
shelling -h
man shelling
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Read the help and package contents first because miscellaneous tools vary widely.
2. Run on a small sample or lab input before using on important data.
3. Save outputs to a separate folder.
4. Document the exact command used for repeatability.

## Example commands

```bash
shelling --help
```

```bash
shelling -h
```

```bash
pacman -Ql shelling | sed -n "1,120p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
