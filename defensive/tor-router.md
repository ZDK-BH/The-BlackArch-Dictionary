# tor-router

**Category:** `defensive`  
**Version in source list:** `22.5b79c1c`  
**Package name:** `tor-router`

## What it does

A tool that allow you to make TOR your default gateway and send all internet connections under TOR (as transparent proxy) for increase privacy/anonymity without extra unnecessary code.

## What it can be used for

Hardening, monitoring, detection, honeypot support, rootkit checks, and defensive analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed tor-router
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql tor-router | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
tor-router --help
tor-router -h
man tor-router
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run from a trusted environment where possible.
2. Update signatures/rules if the tool supports it.
3. Save reports to a timestamped folder.
4. Treat alerts as leads and verify with additional evidence.

## Example commands

```bash
tor-router --help
```

```bash
tor-router -h
```

```bash
# Defensive scan/report pattern:
tor-router --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
