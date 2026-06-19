# ctunnel

**Category:** `tunnel`  
**Version in source list:** `0.7`  
**Package name:** `ctunnel`

## What it does

Tunnel and/or proxy TCP or UDP connections via a cryptographic tunnel.

## What it can be used for

Testing network paths, lab pivots, debugging connectivity, and controlled remote access scenarios.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed ctunnel
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql ctunnel | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
ctunnel --help
ctunnel -h
man ctunnel
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use tunnels only for systems you own or administer.
2. Bind services to localhost where possible.
3. Log connection endpoints and close tunnels after testing.
4. Avoid bypassing organizational policy without written approval.

## Example commands

```bash
ctunnel --help
```

```bash
ctunnel -h
```

```bash
# Local connectivity checks:
ss -tulpn
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
