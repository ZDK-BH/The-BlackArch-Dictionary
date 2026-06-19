# atear

**Category:** `wireless`  
**Version in source list:** `139.245ec8d`  
**Package name:** `atear`

## What it does

Wireless Hacking, WiFi Security, Vulnerability Analyzer, Pentestration.

## What it can be used for

Auditing Wi-Fi/RF configurations, frames, clients, access points, and lab wireless behavior.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed atear
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql atear | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
atear --help
atear -h
man atear
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Test only your own APs or approved wireless ranges.
2. Confirm adapter/driver support first.
3. Start with passive discovery and signal analysis.
4. Use findings to improve WPA settings, firmware, segmentation, and monitoring.

## Example commands

```bash
atear --help
```

```bash
atear -h
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
