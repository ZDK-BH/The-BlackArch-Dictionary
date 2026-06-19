# spoofy

**Category:** `spoof`  
**Version in source list:** `v1.0.3.r0.g28db5fd`  
**Package name:** `spoofy`

## What it does

Check if a list of domains can be spoofed based on SPF and DMARC records.

## What it can be used for

Understanding spoofing risks, validating defenses, and training detection systems.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed spoofy
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql spoofy | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
spoofy --help
spoofy -h
man spoofy
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use an isolated lab network only.
2. Understand the protocol impact before generating traffic.
3. Run packet capture from a separate monitor host to observe effects.
4. Use results to tune alerts and harden network controls.

## Example commands

```bash
spoofy --help
```

```bash
spoofy -h
```

```bash
# Lab network prep:
ip addr
ip route
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
