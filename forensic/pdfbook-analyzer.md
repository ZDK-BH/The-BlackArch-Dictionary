# pdfbook-analyzer

**Category:** `forensic`  
**Version in source list:** `2`  
**Package name:** `pdfbook-analyzer`

## What it does

Utility for facebook memory forensics.

## What it can be used for

Disk, memory, browser, log, file, and mobile artifact analysis; evidence review and incident investigation.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed pdfbook-analyzer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql pdfbook-analyzer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
pdfbook-analyzer --help
pdfbook-analyzer -h
man pdfbook-analyzer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Preserve originals and analyze copies only.
2. Hash evidence before and after copying.
3. Use read-only mounts where possible.
4. Export findings to a case folder with timestamps and notes.

## Example commands

```bash
pdfbook-analyzer --help
```

```bash
pdfbook-analyzer -h
```

```bash
sha256sum ./evidence.img
```

```bash
# Local evidence-copy pattern:
pdfbook-analyzer ./evidence-copy.img
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
