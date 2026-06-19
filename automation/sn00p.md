# sn00p

**Category:** `automation`  
**Version in source list:** `0.8`  
**Package name:** `sn00p`

## What it does

A modular tool written in bourne shell and designed to chain and automate security tools and tests.

## What it can be used for

Automating repeatable recon, scanning, wordlist, reporting, or assessment tasks.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sn00p
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sn00p | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sn00p --help
sn00p -h
man sn00p
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Define an approved scope before automation so the tool does not wander outside your target list.
2. Use a small test input file first.
3. Check output manually before trusting results.
4. Add rate limits or delays when the tool supports them.

## Example commands

```bash
sn00p --help
```

```bash
sn00p -h
```

```bash
# Common safe pattern with a small lab target list:
sn00p -i targets.txt -o results.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
