# subscraper

**Category:** `recon`  
**Version in source list:** `34.29aa5cc`  
**Package name:** `subscraper`

## What it does

Tool that performs subdomain enumeration through various techniques.

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed subscraper
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql subscraper | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
subscraper --help
subscraper -h
man subscraper
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
subscraper --help
```

```bash
subscraper -h
```

```bash
# Authorized domain/lab pattern:
subscraper example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
