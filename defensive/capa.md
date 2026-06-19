# capa

**Category:** `defensive`  
**Version in source list:** `7.4.0`  
**Package name:** `capa`

## What it does

The FLARE team's open-source tool to identify capabilities in executable files.

## What it can be used for

Hardening, monitoring, detection, honeypot support, rootkit checks, and defensive analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed capa
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql capa | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
capa --help
capa -h
man capa
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run from a trusted environment where possible.
2. Update signatures/rules if the tool supports it.
3. Save reports to a timestamped folder.
4. Treat alerts as leads and verify with additional evidence.

## Example commands

```bash
capa --help
```

```bash
capa -h
```

```bash
# Defensive scan/report pattern:
capa --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
