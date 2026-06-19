# matahari

**Category:** `tunnel`  
**Version in source list:** `0.1.30`  
**Package name:** `matahari`

## What it does

A reverse HTTP shell to execute commands on remote machines behind firewalls.

## What it can be used for

Testing network paths, lab pivots, debugging connectivity, and controlled remote access scenarios.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed matahari
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql matahari | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
matahari --help
matahari -h
man matahari
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use tunnels only for systems you own or administer.
2. Bind services to localhost where possible.
3. Log connection endpoints and close tunnels after testing.
4. Avoid bypassing organizational policy without written approval.

## Example commands

```bash
matahari --help
```

```bash
matahari -h
```

```bash
# Local connectivity checks:
ss -tulpn
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
