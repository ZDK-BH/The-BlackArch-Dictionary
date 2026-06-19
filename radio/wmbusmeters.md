# wmbusmeters

**Category:** `radio`  
**Version in source list:** `1.17.1`  
**Package name:** `wmbusmeters`

## What it does

Read the wired or wireless mbus protocol to acquire utility meter readings.

## What it can be used for

Signal decoding, RF monitoring, and protocol experiments using SDR hardware.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed wmbusmeters
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql wmbusmeters | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
wmbusmeters --help
wmbusmeters -h
man wmbusmeters
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Check your local radio regulations before transmitting anything.
2. Start with receive-only examples.
3. Verify SDR hardware is detected.
4. Record metadata such as frequency, sample rate, and antenna setup.

## Example commands

```bash
wmbusmeters --help
```

```bash
wmbusmeters -h
```

```bash
lsusb
```

```bash
# Receive-only lab pattern after docs:
wmbusmeters --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
