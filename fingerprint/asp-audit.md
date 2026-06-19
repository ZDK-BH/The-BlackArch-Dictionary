# asp-audit

**Category:** `fingerprint`  
**Version in source list:** `2BETA`  
**Package name:** `asp-audit`

## What it does

An ASP fingerprinting tool and vulnerability scanner.

## What it can be used for

Identifying services, frameworks, versions, CMSs, applications, or technologies.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed asp-audit
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql asp-audit | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
asp-audit --help
asp-audit -h
man asp-audit
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Start with passive or low-rate fingerprinting.
2. Compare output with headers, certificates, and application behavior.
3. Confirm version findings manually.
4. Use results to plan patching or authorized testing.

## Example commands

```bash
asp-audit --help
```

```bash
asp-audit -h
```

```bash
# Owned lab target pattern:
asp-audit https://example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
