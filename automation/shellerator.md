# shellerator

**Category:** `automation`  
**Version in source list:** `69.4047fd2`  
**Package name:** `shellerator`

## What it does

Simple command-line tool aimed to help pentesters quickly generate one-liner reverse/bind shells in multiple languages.

## What it can be used for

Automating repeatable recon, scanning, wordlist, reporting, or assessment tasks.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed shellerator
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql shellerator | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
shellerator --help
shellerator -h
man shellerator
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Define an approved scope before automation so the tool does not wander outside your target list.
2. Use a small test input file first.
3. Check output manually before trusting results.
4. Add rate limits or delays when the tool supports them.

## Example commands

```bash
shellerator --help
```

```bash
shellerator -h
```

```bash
# Common safe pattern with a small lab target list:
shellerator -i targets.txt -o results.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
