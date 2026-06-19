# fraud-bridge

**Category:** `tunnel`  
**Version in source list:** `rel.0.32s.r3.g88a5baa`  
**Package name:** `fraud-bridge`

## What it does

ICMP and DNS tunneling via IPv4 and IPv6.

## What it can be used for

Testing network paths, lab pivots, debugging connectivity, and controlled remote access scenarios.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed fraud-bridge
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql fraud-bridge | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
fraud-bridge --help
fraud-bridge -h
man fraud-bridge
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use tunnels only for systems you own or administer.
2. Bind services to localhost where possible.
3. Log connection endpoints and close tunnels after testing.
4. Avoid bypassing organizational policy without written approval.

## Example commands

```bash
fraud-bridge --help
```

```bash
fraud-bridge -h
```

```bash
# Local connectivity checks:
ss -tulpn
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
