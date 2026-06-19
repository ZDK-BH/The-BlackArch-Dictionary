# zgrab2

**Category:** `fingerprint`  
**Version in source list:** `v1.0.0.r61.ge5172a7`  
**Package name:** `zgrab2`

## What it does

Fast Application Layer Scanner.

## What it can be used for

Identifying services, frameworks, versions, CMSs, applications, or technologies.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed zgrab2
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql zgrab2 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
zgrab2 --help
zgrab2 -h
man zgrab2
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Start with passive or low-rate fingerprinting.
2. Compare output with headers, certificates, and application behavior.
3. Confirm version findings manually.
4. Use results to plan patching or authorized testing.

## Example commands

```bash
zgrab2 --help
```

```bash
zgrab2 -h
```

```bash
# Owned lab target pattern:
zgrab2 https://example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
