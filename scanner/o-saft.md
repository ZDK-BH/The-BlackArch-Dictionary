# o-saft

**Category:** `scanner`  
**Version in source list:** `7172.b4350981`  
**Package name:** `o-saft`

## What it does

A tool to show informations about SSL certificate and tests the SSL connection according given list of ciphers and various SSL configurations.

## What it can be used for

Finding exposed services, misconfigurations, versions, certificates, web paths, and vulnerability indicators.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed o-saft
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql o-saft | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
o-saft --help
o-saft -h
man o-saft
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Scan only approved IP ranges/domains.
2. Start with low-rate or passive scans if available.
3. Export results and verify findings manually.
4. Fix or report validated issues with clear evidence.

## Example commands

```bash
o-saft --help
```

```bash
o-saft -h
```

```bash
# Owned lab host pattern:
o-saft 192.0.2.10
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
