# base64dump

**Category:** `misc`  
**Version in source list:** `0.0.14`  
**Package name:** `base64dump`

## What it does

Extract and decode base64 strings from files.

## What it can be used for

Supporting security workflows such as encoding, parsing, helper automation, lookup, or specialized analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed base64dump
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql base64dump | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
base64dump --help
base64dump -h
man base64dump
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Read the help and package contents first because miscellaneous tools vary widely.
2. Run on a small sample or lab input before using on important data.
3. Save outputs to a separate folder.
4. Document the exact command used for repeatability.

## Example commands

```bash
base64dump --help
```

```bash
base64dump -h
```

```bash
pacman -Ql base64dump | sed -n "1,120p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
