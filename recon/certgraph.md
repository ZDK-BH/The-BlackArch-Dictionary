# certgraph

**Category:** `recon`  
**Version in source list:** `194.9826815`  
**Package name:** `certgraph`

## What it does

Crawl the graph of certificate Alternate Names.

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed certgraph
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql certgraph | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
certgraph --help
certgraph -h
man certgraph
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
certgraph --help
```

```bash
certgraph -h
```

```bash
# Authorized domain/lab pattern:
certgraph example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
