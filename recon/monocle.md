# monocle

**Category:** `recon`  
**Version in source list:** `1.0`  
**Package name:** `monocle`

## What it does

A local network host discovery tool. In passive mode, it will listen for ARP request and reply packets. In active mode, it will send ARP requests to the specific IP range. The results are a list of IP and MAC addresses present on the local network.

## What it can be used for

Asset inventory, DNS/subdomain discovery, public metadata review, cloud exposure checks, and external attack-surface mapping.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed monocle
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql monocle | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
monocle --help
monocle -h
man monocle
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Confirm the domain/company/IP range is in scope.
2. Start with passive sources and public data.
3. Move to active checks only when authorized.
4. Deduplicate findings and validate important assets manually.

## Example commands

```bash
monocle --help
```

```bash
monocle -h
```

```bash
# Authorized domain/lab pattern:
monocle example.test
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
