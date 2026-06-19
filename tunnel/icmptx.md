# icmptx

**Category:** `tunnel`  
**Version in source list:** `0.2.r12.g2235866`  
**Package name:** `icmptx`

## What it does

IP over ICMP tunnel.

## What it can be used for

Testing network paths, lab pivots, debugging connectivity, and controlled remote access scenarios.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed icmptx
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql icmptx | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
icmptx --help
icmptx -h
man icmptx
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use tunnels only for systems you own or administer.
2. Bind services to localhost where possible.
3. Log connection endpoints and close tunnels after testing.
4. Avoid bypassing organizational policy without written approval.

## Example commands

```bash
icmptx --help
```

```bash
icmptx -h
```

```bash
# Local connectivity checks:
ss -tulpn
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
