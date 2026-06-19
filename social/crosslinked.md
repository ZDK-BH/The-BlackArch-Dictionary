# crosslinked

**Category:** `social`  
**Version in source list:** `v0.3.0.r23.g2ae8d7b`  
**Package name:** `crosslinked`

## What it does

LinkedIn enumeration tool to extract valid employee names from an organization through search engine scraping.

## What it can be used for

Public-information review, awareness training, and phishing-defense education.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed crosslinked
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql crosslinked | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
crosslinked --help
crosslinked -h
man crosslinked
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only test accounts, training domains, or approved awareness programs.
2. Do not collect real credentials or personal data without a formal authorization process.
3. Focus on education, detection, and reporting workflows.
4. Keep logs sanitized and delete sensitive test data after the exercise.

## Example commands

```bash
crosslinked --help
```

```bash
crosslinked -h
```

```bash
# Training-only prep:
mkdir -p awareness-lab
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
