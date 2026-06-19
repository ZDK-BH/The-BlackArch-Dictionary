# kismet2earth

**Category:** `wireless`  
**Version in source list:** `2.0`  
**Package name:** `kismet2earth`

## What it does

A set of utilities that convert from Kismet logs to Google Earth .kml format.

## What it can be used for

Auditing Wi-Fi/RF configurations, frames, clients, access points, and lab wireless behavior.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed kismet2earth
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql kismet2earth | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
kismet2earth --help
kismet2earth -h
man kismet2earth
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Test only your own APs or approved wireless ranges.
2. Confirm adapter/driver support first.
3. Start with passive discovery and signal analysis.
4. Use findings to improve WPA settings, firmware, segmentation, and monitoring.

## Example commands

```bash
kismet2earth --help
```

```bash
kismet2earth -h
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
