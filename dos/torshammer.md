# torshammer

**Category:** `dos`  
**Version in source list:** `1.0`  
**Package name:** `torshammer`

## What it does

A slow POST Denial of Service testing tool written in Python.

## What it can be used for

Learning about availability risks and testing resilience in a closed lab only.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed torshammer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql torshammer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
torshammer --help
torshammer -h
man torshammer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Do not use against public systems or networks.
2. Build a private lab with disposable services and bandwidth limits.
3. Read documentation and understand traffic volume before any test.
4. Measure defensive controls such as rate limits, alerts, and service recovery.

## Example commands

```bash
torshammer --help
```

```bash
torshammer -h
```

```bash
# Safer preparation example:
ip addr
ss -tulpn
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
