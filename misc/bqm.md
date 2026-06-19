# bqm

**Category:** `misc`  
**Version in source list:** `v1.5.1.r5.ge287280`  
**Package name:** `bqm`

## What it does

Download BloudHound query lists, deduplicate entries and merge them in one file.

## What it can be used for

Supporting security workflows such as encoding, parsing, helper automation, lookup, or specialized analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed bqm
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql bqm | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
bqm --help
bqm -h
man bqm
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Read the help and package contents first because miscellaneous tools vary widely.
2. Run on a small sample or lab input before using on important data.
3. Save outputs to a separate folder.
4. Document the exact command used for repeatability.

## Example commands

```bash
bqm --help
```

```bash
bqm -h
```

```bash
pacman -Ql bqm | sed -n "1,120p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
