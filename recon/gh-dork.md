# gh-dork

**Category:** `recon`  
**Version in source list:** `3.799f86f`  
**Package name:** `gh-dork`

## What it does

Github dorking tool.

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed gh-dork
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql gh-dork | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
gh-dork --help
gh-dork -h
man gh-dork
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
gh-dork --help
```

```bash
gh-dork -h
```

```bash
# Authorized domain/lab pattern:
gh-dork example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
