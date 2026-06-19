# local-php-security-checker

**Category:** `code-audit`  
**Version in source list:** `v2.1.3.r1.g1d1fdac`  
**Package name:** `local-php-security-checker`

## What it does

A command line tool that checks your PHP application packages with known security vulnerabilities.

## What it can be used for

Finding insecure patterns in code, dependencies, infrastructure-as-code, and application logic.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed local-php-security-checker
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql local-php-security-checker | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
local-php-security-checker --help
local-php-security-checker -h
man local-php-security-checker
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run it against your own repository or a deliberately vulnerable training repo.
2. Start with default scan settings.
3. Review findings manually to remove false positives.
4. Fix issues, commit changes, and rerun the scan.

## Example commands

```bash
local-php-security-checker --help
```

```bash
local-php-security-checker -h
```

```bash
# Common local repo pattern:
local-php-security-checker ./project
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
