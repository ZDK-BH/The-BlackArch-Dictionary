# enum-shares

**Category:** `scanner`  
**Version in source list:** `7.97cba5a`  
**Package name:** `enum-shares`

## What it does

Tool that enumerates shared folders across the network and under a custom user account.

## What it can be used for

Finding exposed services, misconfigurations, versions, certificates, web paths, and vulnerability indicators.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed enum-shares
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql enum-shares | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
enum-shares --help
enum-shares -h
man enum-shares
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Scan only approved IP ranges/domains.
2. Start with low-rate or passive scans if available.
3. Export results and verify findings manually.
4. Fix or report validated issues with clear evidence.

## Example commands

```bash
enum-shares --help
```

```bash
enum-shares -h
```

```bash
# Owned lab host pattern:
enum-shares 192.0.2.10
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
