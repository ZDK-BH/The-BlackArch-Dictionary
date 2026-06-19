# country-ip-blocks

**Category:** `wordlist`  
**Version in source list:** `6365.1ad7ecd`  
**Package name:** `country-ip-blocks`

## What it does

CIDR country-level IP data, straight from the Regional Internet Registries, updated hourly.

## What it can be used for

Generating or using lists for approved testing, discovery, or password-policy audits.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed country-ip-blocks
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql country-ip-blocks | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
country-ip-blocks --help
country-ip-blocks -h
man country-ip-blocks
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use wordlists only for approved testing.
2. Keep lists relevant and small at first.
3. Deduplicate and sort before use.
4. Record which list/version produced each result.

## Example commands

```bash
country-ip-blocks --help
```

```bash
country-ip-blocks -h
```

```bash
# Wordlist hygiene:
sort -u input.txt > wordlist-clean.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
