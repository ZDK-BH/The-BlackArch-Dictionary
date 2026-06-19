# flare

**Category:** `misc`  
**Version in source list:** `0.6`  
**Package name:** `flare`

## What it does

Flare processes an SWF and extracts all scripts from it.

## What it can be used for

Supporting security workflows such as encoding, parsing, helper automation, lookup, or specialized analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed flare
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql flare | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
flare --help
flare -h
man flare
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Read the help and package contents first because miscellaneous tools vary widely.
2. Run on a small sample or lab input before using on important data.
3. Save outputs to a separate folder.
4. Document the exact command used for repeatability.

## Example commands

```bash
flare --help
```

```bash
flare -h
```

```bash
pacman -Ql flare | sed -n "1,120p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
