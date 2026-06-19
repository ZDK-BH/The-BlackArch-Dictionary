# rfidiot

**Category:** `wireless`  
**Version in source list:** `107.88f2ef9`  
**Package name:** `rfidiot`

## What it does

An open source python library for exploring RFID devices.

## What it can be used for

Auditing Wi-Fi/RF configurations, frames, clients, access points, and lab wireless behavior.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed rfidiot
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql rfidiot | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
rfidiot --help
rfidiot -h
man rfidiot
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Test only your own APs or approved wireless ranges.
2. Confirm adapter/driver support first.
3. Start with passive discovery and signal analysis.
4. Use findings to improve WPA settings, firmware, segmentation, and monitoring.

## Example commands

```bash
rfidiot --help
```

```bash
rfidiot -h
```

```bash
iw dev
```

```bash
rfkill list
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
