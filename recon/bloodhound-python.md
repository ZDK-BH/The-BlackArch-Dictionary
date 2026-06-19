# bloodhound-python

**Category:** `recon`  
**Version in source list:** `v1.0.1.r186.gfd3f322`  
**Package name:** `bloodhound-python`

## What it does

Python data collector for Bloodhound legcacy (v4)

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed bloodhound-python
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql bloodhound-python | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
bloodhound-python --help
bloodhound-python -h
man bloodhound-python
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
bloodhound-python --help
```

```bash
bloodhound-python -h
```

```bash
# Authorized domain/lab pattern:
bloodhound-python example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
