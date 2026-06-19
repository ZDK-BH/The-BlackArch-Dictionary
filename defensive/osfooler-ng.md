# osfooler-ng

**Category:** `defensive`  
**Version in source list:** `2.c0b20d6`  
**Package name:** `osfooler-ng`

## What it does

Prevents remote active/passive OS fingerprinting by tools like nmap or p0f.

## What it can be used for

Hardening, monitoring, detection, honeypot support, rootkit checks, and defensive analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed osfooler-ng
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql osfooler-ng | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
osfooler-ng --help
osfooler-ng -h
man osfooler-ng
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run from a trusted environment where possible.
2. Update signatures/rules if the tool supports it.
3. Save reports to a timestamped folder.
4. Treat alerts as leads and verify with additional evidence.

## Example commands

```bash
osfooler-ng --help
```

```bash
osfooler-ng -h
```

```bash
# Defensive scan/report pattern:
osfooler-ng --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
