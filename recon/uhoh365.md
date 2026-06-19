# uhoh365

**Category:** `recon`  
**Version in source list:** `26.110277a`  
**Package name:** `uhoh365`

## What it does

Script to enumerate Office 365 users without performing login attempts

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed uhoh365
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql uhoh365 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
uhoh365 --help
uhoh365 -h
man uhoh365
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
uhoh365 --help
```

```bash
uhoh365 -h
```

```bash
# Authorized domain/lab pattern:
uhoh365 example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
