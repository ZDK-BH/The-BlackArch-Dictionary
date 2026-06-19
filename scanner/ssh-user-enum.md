# ssh-user-enum

**Category:** `scanner`  
**Version in source list:** `7.ae453c1`  
**Package name:** `ssh-user-enum`

## What it does

SSH User Enumeration Script in Python Using The Timing Attack.

## What it can be used for

Finding exposed services, misconfigurations, versions, certificates, web paths, and vulnerability indicators.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed ssh-user-enum
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql ssh-user-enum | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
ssh-user-enum --help
ssh-user-enum -h
man ssh-user-enum
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Scan only approved IP ranges/domains.
2. Start with low-rate or passive scans if available.
3. Export results and verify findings manually.
4. Fix or report validated issues with clear evidence.

## Example commands

```bash
ssh-user-enum --help
```

```bash
ssh-user-enum -h
```

```bash
# Owned lab host pattern:
ssh-user-enum 192.0.2.10
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
