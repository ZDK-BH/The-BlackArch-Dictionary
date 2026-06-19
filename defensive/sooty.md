# sooty

**Category:** `defensive`  
**Version in source list:** `335.6236fd1`  
**Package name:** `sooty`

## What it does

The SOC Analysts all-in-one CLI tool to automate and speed up workflow.

## What it can be used for

Hardening, monitoring, detection, honeypot support, rootkit checks, and defensive analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sooty
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sooty | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sooty --help
sooty -h
man sooty
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run from a trusted environment where possible.
2. Update signatures/rules if the tool supports it.
3. Save reports to a timestamped folder.
4. Treat alerts as leads and verify with additional evidence.

## Example commands

```bash
sooty --help
```

```bash
sooty -h
```

```bash
# Defensive scan/report pattern:
sooty --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
