# koadic

**Category:** `automation`  
**Version in source list:** `3.457f9a3`  
**Package name:** `koadic`

## What it does

A Windows post-exploitation rootkit similar to other penetration testing tools such as Meterpreter and Powershell Empire.

## What it can be used for

Automating repeatable recon, scanning, wordlist, reporting, or assessment tasks.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed koadic
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql koadic | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
koadic --help
koadic -h
man koadic
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Define an approved scope before automation so the tool does not wander outside your target list.
2. Use a small test input file first.
3. Check output manually before trusting results.
4. Add rate limits or delays when the tool supports them.

## Example commands

```bash
koadic --help
```

```bash
koadic -h
```

```bash
# Common safe pattern with a small lab target list:
koadic -i targets.txt -o results.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
