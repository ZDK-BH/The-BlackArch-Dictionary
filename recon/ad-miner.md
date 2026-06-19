# ad-miner

**Category:** `recon`  
**Version in source list:** `v1.9.0.r0.gac3d473`  
**Package name:** `ad-miner`

## What it does

Active Directory audit tool that extract data from Bloodhound to uncover security weaknesses and generate an HTML report

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed ad-miner
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql ad-miner | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
ad-miner --help
ad-miner -h
man ad-miner
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
ad-miner --help
```

```bash
ad-miner -h
```

```bash
# Authorized domain/lab pattern:
ad-miner example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
