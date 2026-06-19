# gsmevil2

**Category:** `radio`  
**Version in source list:** `18.ce64fa5`  
**Package name:** `gsmevil2`

## What it does

Python web-based tool which use for capturing imsi numbers and sms.

## What it can be used for

Signal decoding, RF monitoring, and protocol experiments using SDR hardware.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed gsmevil2
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql gsmevil2 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
gsmevil2 --help
gsmevil2 -h
man gsmevil2
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Check your local radio regulations before transmitting anything.
2. Start with receive-only examples.
3. Verify SDR hardware is detected.
4. Record metadata such as frequency, sample rate, and antenna setup.

## Example commands

```bash
gsmevil2 --help
```

```bash
gsmevil2 -h
```

```bash
lsusb
```

```bash
# Receive-only lab pattern after docs:
gsmevil2 --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
