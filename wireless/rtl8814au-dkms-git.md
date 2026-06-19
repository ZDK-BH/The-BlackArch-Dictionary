# rtl8814au-dkms-git

**Category:** `wireless`  
**Version in source list:** `5.8.5.1.r206.gb1866ce`  
**Package name:** `rtl8814au-dkms-git`

## What it does

RTL8814AU and RTL8813AU chipset driver with firmware v5.8.5.1.

## What it can be used for

Auditing Wi-Fi/RF configurations, frames, clients, access points, and lab wireless behavior.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed rtl8814au-dkms-git
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql rtl8814au-dkms-git | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
rtl8814au-dkms-git --help
rtl8814au-dkms-git -h
man rtl8814au-dkms-git
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Test only your own APs or approved wireless ranges.
2. Confirm adapter/driver support first.
3. Start with passive discovery and signal analysis.
4. Use findings to improve WPA settings, firmware, segmentation, and monitoring.

## Example commands

```bash
rtl8814au-dkms-git --help
```

```bash
rtl8814au-dkms-git -h
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
