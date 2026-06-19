# python2-ivre

**Category:** `recon`  
**Version in source list:** `0.9.16.dev26`  
**Package name:** `python2-ivre`

## What it does

Network recon framework based on Nmap, Masscan, Zeek (Bro), Argus, Netflow,... (library)

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed python2-ivre
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql python2-ivre | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
python2-ivre --help
python2-ivre -h
man python2-ivre
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
python2-ivre --help
```

```bash
python2-ivre -h
```

```bash
# Authorized domain/lab pattern:
python2-ivre example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
