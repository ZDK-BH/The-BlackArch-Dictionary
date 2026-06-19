# yeti

**Category:** `defensive`  
**Version in source list:** `3432.1f5b1261`  
**Package name:** `yeti`

## What it does

A platform meant to organize observables, indicators of compromise, TTPs, and knowledge on threats in a single, unified repository.

## What it can be used for

Hardening, monitoring, detection, honeypot support, rootkit checks, and defensive analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed yeti
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql yeti | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
yeti --help
yeti -h
man yeti
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run from a trusted environment where possible.
2. Update signatures/rules if the tool supports it.
3. Save reports to a timestamped folder.
4. Treat alerts as leads and verify with additional evidence.

## Example commands

```bash
yeti --help
```

```bash
yeti -h
```

```bash
# Defensive scan/report pattern:
yeti --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
