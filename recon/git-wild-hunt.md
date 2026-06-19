# git-wild-hunt

**Category:** `recon`  
**Version in source list:** `16.6495672`  
**Package name:** `git-wild-hunt`

## What it does

A tool to hunt for credentials in github wild AKA git*hunt.

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed git-wild-hunt
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql git-wild-hunt | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
git-wild-hunt --help
git-wild-hunt -h
man git-wild-hunt
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
git-wild-hunt --help
```

```bash
git-wild-hunt -h
```

```bash
# Authorized domain/lab pattern:
git-wild-hunt example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
