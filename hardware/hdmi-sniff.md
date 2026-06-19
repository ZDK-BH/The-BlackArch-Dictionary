# hdmi-sniff

**Category:** `hardware`  
**Version in source list:** `5.f7fbc0e`  
**Package name:** `hdmi-sniff`

## What it does

HDMI DDC (I2C) inspection tool. It is designed to demonstrate just how easy it is to recover HDCP crypto keys from HDMI devices.

## What it can be used for

Firmware, chipset, bus, boot, platform, or device security testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed hdmi-sniff
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql hdmi-sniff | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
hdmi-sniff --help
hdmi-sniff -h
man hdmi-sniff
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Read documentation carefully because hardware tools can affect system stability.
2. Run read-only checks first.
3. Save logs before making changes.
4. Use results to patch firmware, lock BIOS/UEFI settings, and improve physical security.

## Example commands

```bash
hdmi-sniff --help
```

```bash
hdmi-sniff -h
```

```bash
# System inventory first:
lscpu
lsusb
lspci
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
