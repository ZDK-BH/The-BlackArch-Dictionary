# sn1per

**Category:** `automation`  
**Version in source list:** `720.a965fa4`  
**Package name:** `sn1per`

## What it does

Automated Pentest Recon Scanner.

## What it can be used for

Automating repeatable recon, scanning, wordlist, reporting, or assessment tasks.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sn1per
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sn1per | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sn1per --help
sn1per -h
man sn1per
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Define an approved scope before automation so the tool does not wander outside your target list.
2. Use a small test input file first.
3. Check output manually before trusting results.
4. Add rate limits or delays when the tool supports them.

## Example commands

```bash
sn1per --help
```

```bash
sn1per -h
```

```bash
# Common safe pattern with a small lab target list:
sn1per -i targets.txt -o results.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
