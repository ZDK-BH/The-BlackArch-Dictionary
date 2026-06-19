# fl0p

**Category:** `fingerprint`  
**Version in source list:** `0.1`  
**Package name:** `fl0p`

## What it does

A passive L7 flow fingerprinter that examines TCP/UDP/ICMP packet sequences, can peek into cryptographic tunnels, can tell human beings and robots apart, and performs a couple of other infosec-related tricks.

## What it can be used for

Identifying services, frameworks, versions, CMSs, applications, or technologies.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed fl0p
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql fl0p | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
fl0p --help
fl0p -h
man fl0p
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Start with passive or low-rate fingerprinting.
2. Compare output with headers, certificates, and application behavior.
3. Confirm version findings manually.
4. Use results to plan patching or authorized testing.

## Example commands

```bash
fl0p --help
```

```bash
fl0p -h
```

```bash
# Owned lab target pattern:
fl0p https://example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
