# wdict

**Category:** `wordlist`  
**Version in source list:** `v0.1.20.r0.g05d896c`  
**Package name:** `wdict`

## What it does

Create dictionaries by scraping webpages or crawling local files.

## What it can be used for

Generating or using lists for approved testing, discovery, or password-policy audits.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed wdict
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql wdict | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
wdict --help
wdict -h
man wdict
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use wordlists only for approved testing.
2. Keep lists relevant and small at first.
3. Deduplicate and sort before use.
4. Record which list/version produced each result.

## Example commands

```bash
wdict --help
```

```bash
wdict -h
```

```bash
# Wordlist hygiene:
sort -u input.txt > wordlist-clean.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
