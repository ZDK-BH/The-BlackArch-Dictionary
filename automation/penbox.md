# penbox

**Category:** `automation`  
**Version in source list:** `81.3b77c69`  
**Package name:** `penbox`

## What it does

A Penetration Testing Framework - The Tool With All The Tools.

## What it can be used for

Automating repeatable recon, scanning, wordlist, reporting, or assessment tasks.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed penbox
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql penbox | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
penbox --help
penbox -h
man penbox
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Define an approved scope before automation so the tool does not wander outside your target list.
2. Use a small test input file first.
3. Check output manually before trusting results.
4. Add rate limits or delays when the tool supports them.

## Example commands

```bash
penbox --help
```

```bash
penbox -h
```

```bash
# Common safe pattern with a small lab target list:
penbox -i targets.txt -o results.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
