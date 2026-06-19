# wpa-bruteforcer

**Category:** `wireless`  
**Version in source list:** `4.d5f8586`  
**Package name:** `wpa-bruteforcer`

## What it does

Attacking WPA/WPA encrypted access point without client.

## What it can be used for

Auditing Wi-Fi/RF configurations, frames, clients, access points, and lab wireless behavior.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed wpa-bruteforcer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql wpa-bruteforcer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
wpa-bruteforcer --help
wpa-bruteforcer -h
man wpa-bruteforcer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Test only your own APs or approved wireless ranges.
2. Confirm adapter/driver support first.
3. Start with passive discovery and signal analysis.
4. Use findings to improve WPA settings, firmware, segmentation, and monitoring.

## Example commands

```bash
wpa-bruteforcer --help
```

```bash
wpa-bruteforcer -h
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
