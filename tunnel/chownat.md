# chownat

**Category:** `tunnel`  
**Version in source list:** `0.08b`  
**Package name:** `chownat`

## What it does

Allows two peers behind two separate NATs with no port forwarding and no DMZ setup on their routers to directly communicate with each other

## What it can be used for

Testing network paths, lab pivots, debugging connectivity, and controlled remote access scenarios.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed chownat
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql chownat | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
chownat --help
chownat -h
man chownat
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use tunnels only for systems you own or administer.
2. Bind services to localhost where possible.
3. Log connection endpoints and close tunnels after testing.
4. Avoid bypassing organizational policy without written approval.

## Example commands

```bash
chownat --help
```

```bash
chownat -h
```

```bash
# Local connectivity checks:
ss -tulpn
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
