# ssl-hostname-resolver

**Category:** `recon`  
**Version in source list:** `1`  
**Package name:** `ssl-hostname-resolver`

## What it does

CN (Common Name) grabber on X.509 Certificates over HTTPS.

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed ssl-hostname-resolver
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql ssl-hostname-resolver | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
ssl-hostname-resolver --help
ssl-hostname-resolver -h
man ssl-hostname-resolver
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
ssl-hostname-resolver --help
```

```bash
ssl-hostname-resolver -h
```

```bash
# Authorized domain/lab pattern:
ssl-hostname-resolver example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
