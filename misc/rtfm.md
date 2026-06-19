# rtfm

**Category:** `misc`  
**Version in source list:** `95.a807a80`  
**Package name:** `rtfm`

## What it does

A database of common, interesting or useful commands, in one handy referable form.

## What it can be used for

Supporting security workflows such as encoding, parsing, helper automation, lookup, or specialized analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed rtfm
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql rtfm | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
rtfm --help
rtfm -h
man rtfm
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Read the help and package contents first because miscellaneous tools vary widely.
2. Run on a small sample or lab input before using on important data.
3. Save outputs to a separate folder.
4. Document the exact command used for repeatability.

## Example commands

```bash
rtfm --help
```

```bash
rtfm -h
```

```bash
pacman -Ql rtfm | sed -n "1,120p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
