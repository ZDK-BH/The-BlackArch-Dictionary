# lfi-scanner

**Category:** `scanner`  
**Version in source list:** `4.0`  
**Package name:** `lfi-scanner`

## What it does

This is a simple perl script that enumerates local file inclusion attempts when given a specific target.

## What it can be used for

Finding exposed services, misconfigurations, versions, certificates, web paths, and vulnerability indicators.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed lfi-scanner
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql lfi-scanner | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
lfi-scanner --help
lfi-scanner -h
man lfi-scanner
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Scan only approved IP ranges/domains.
2. Start with low-rate or passive scans if available.
3. Export results and verify findings manually.
4. Fix or report validated issues with clear evidence.

## Example commands

```bash
lfi-scanner --help
```

```bash
lfi-scanner -h
```

```bash
# Owned lab host pattern:
lfi-scanner 192.0.2.10
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
