# waldo

**Category:** `recon`  
**Version in source list:** `29.ee4f960`  
**Package name:** `waldo`

## What it does

A lightweight and multithreaded directory and subdomain bruteforcer implemented in Python.

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed waldo
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql waldo | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
waldo --help
waldo -h
man waldo
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
waldo --help
```

```bash
waldo -h
```

```bash
# Authorized domain/lab pattern:
waldo example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
