# h2buster

**Category:** `scanner`  
**Version in source list:** `79.6c4dd1c`  
**Package name:** `h2buster`

## What it does

A threaded, recursive, web directory brute-force scanner over HTTP/2.

## What it can be used for

Finding exposed services, misconfigurations, versions, certificates, web paths, and vulnerability indicators.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed h2buster
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql h2buster | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
h2buster --help
h2buster -h
man h2buster
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Scan only approved IP ranges/domains.
2. Start with low-rate or passive scans if available.
3. Export results and verify findings manually.
4. Fix or report validated issues with clear evidence.

## Example commands

```bash
h2buster --help
```

```bash
h2buster -h
```

```bash
# Owned lab host pattern:
h2buster 192.0.2.10
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
