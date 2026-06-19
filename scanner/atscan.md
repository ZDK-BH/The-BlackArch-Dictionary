# atscan

**Category:** `scanner`  
**Version in source list:** `2461.06521a9`  
**Package name:** `atscan`

## What it does

Server, Site and Dork Scanner.

## What it can be used for

Finding exposed services, misconfigurations, versions, certificates, web paths, and vulnerability indicators.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed atscan
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql atscan | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
atscan --help
atscan -h
man atscan
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Scan only approved IP ranges/domains.
2. Start with low-rate or passive scans if available.
3. Export results and verify findings manually.
4. Fix or report validated issues with clear evidence.

## Example commands

```bash
atscan --help
```

```bash
atscan -h
```

```bash
# Owned lab host pattern:
atscan 192.0.2.10
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
