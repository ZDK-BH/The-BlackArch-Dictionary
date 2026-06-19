# ligolo-ng

**Category:** `tunnel`  
**Version in source list:** `v0.8.3.r0.g913fe64`  
**Package name:** `ligolo-ng`

## What it does

An advanced, yet simple, tunneling tool that uses a TUN interface.

## What it can be used for

Testing network paths, lab pivots, debugging connectivity, and controlled remote access scenarios.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed ligolo-ng
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql ligolo-ng | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
ligolo-ng --help
ligolo-ng -h
man ligolo-ng
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use tunnels only for systems you own or administer.
2. Bind services to localhost where possible.
3. Log connection endpoints and close tunnels after testing.
4. Avoid bypassing organizational policy without written approval.

## Example commands

```bash
ligolo-ng --help
```

```bash
ligolo-ng -h
```

```bash
# Local connectivity checks:
ss -tulpn
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
