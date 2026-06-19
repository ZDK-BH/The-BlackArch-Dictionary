# firstorder

**Category:** `sniffer`  
**Version in source list:** `8.107eb6a`  
**Package name:** `firstorder`

## What it does

A traffic analyzer to evade Empire communication from Anomaly-Based IDS.

## What it can be used for

Capturing and analyzing traffic for troubleshooting, malware analysis, IDS tuning, and authorized network review.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed firstorder
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql firstorder | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
firstorder --help
firstorder -h
man firstorder
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Capture only traffic from networks and devices you are allowed to monitor.
2. Start with a specific interface and short capture window.
3. Filter for the protocol or host you are investigating.
4. Store captures securely because they may contain secrets.

## Example commands

```bash
firstorder --help
```

```bash
firstorder -h
```

```bash
ip link
```

```bash
# Capture prep:
mkdir -p pcaps
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
