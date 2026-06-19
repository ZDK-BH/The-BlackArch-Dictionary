# python2-shodan

**Category:** `recon`  
**Version in source list:** `1.28.0`  
**Package name:** `python2-shodan`

## What it does

Python library and command-line utility for Shodan (https://developer.shodan.io).

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed python2-shodan
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql python2-shodan | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
python2-shodan --help
python2-shodan -h
man python2-shodan
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
python2-shodan --help
```

```bash
python2-shodan -h
```

```bash
# Authorized domain/lab pattern:
python2-shodan example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
