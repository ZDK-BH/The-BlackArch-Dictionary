# nsec3walker

**Category:** `recon`  
**Version in source list:** `20101223`  
**Package name:** `nsec3walker`

## What it does

Enumerate domain names using DNSSEC.

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed nsec3walker
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql nsec3walker | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
nsec3walker --help
nsec3walker -h
man nsec3walker
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
nsec3walker --help
```

```bash
nsec3walker -h
```

```bash
# Authorized domain/lab pattern:
nsec3walker example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
