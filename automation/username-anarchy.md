# username-anarchy

**Category:** `automation`  
**Version in source list:** `72.e063191`  
**Package name:** `username-anarchy`

## What it does

Tools for generating usernames when penetration testing.

## What it can be used for

Automating repeatable recon, scanning, wordlist, reporting, or assessment tasks.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed username-anarchy
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql username-anarchy | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
username-anarchy --help
username-anarchy -h
man username-anarchy
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Define an approved scope before automation so the tool does not wander outside your target list.
2. Use a small test input file first.
3. Check output manually before trusting results.
4. Add rate limits or delays when the tool supports them.

## Example commands

```bash
username-anarchy --help
```

```bash
username-anarchy -h
```

```bash
# Common safe pattern with a small lab target list:
username-anarchy -i targets.txt -o results.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
