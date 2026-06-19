# finalrecon

**Category:** `recon`  
**Version in source list:** `v1.1.8.r4.gb5db3a4`  
**Package name:** `finalrecon`

## What it does

OSINT Tool for All-In-One Web Reconnaissance.

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed finalrecon
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql finalrecon | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
finalrecon --help
finalrecon -h
man finalrecon
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
finalrecon --help
```

```bash
finalrecon -h
```

```bash
# Authorized domain/lab pattern:
finalrecon example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
