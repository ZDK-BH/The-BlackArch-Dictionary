# rtl

**Category:** `radio`  
**Version in source list:** `25.12+92.r3790.20260609.ec1245ca`  
**Package name:** `rtl`

## What it does

A generic software defined radio data receiver, mainly for the 433.92 MHz, 868 MHz (SRD), 315 MHz, 345 MHz, and 915 MHz ISM bands.

## What it can be used for

Signal decoding, RF monitoring, and protocol experiments using SDR hardware.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed rtl
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql rtl | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
rtl --help
rtl -h
man rtl
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Check your local radio regulations before transmitting anything.
2. Start with receive-only examples.
3. Verify SDR hardware is detected.
4. Record metadata such as frequency, sample rate, and antenna setup.

## Example commands

```bash
rtl --help
```

```bash
rtl -h
```

```bash
lsusb
```

```bash
# Receive-only lab pattern after docs:
rtl --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
