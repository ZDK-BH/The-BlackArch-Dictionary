# wpa2-halfhandshake-crack

**Category:** `wireless`  
**Version in source list:** `29.3f42124`  
**Package name:** `wpa2-halfhandshake-crack`

## What it does

A POC to show it is possible to capture enough of a handshake with a user from a fake AP to crack a WPA2 network without knowing the passphrase of the actual AP.

## What it can be used for

Auditing Wi-Fi/RF configurations, frames, clients, access points, and lab wireless behavior.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed wpa2-halfhandshake-crack
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql wpa2-halfhandshake-crack | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
wpa2-halfhandshake-crack --help
wpa2-halfhandshake-crack -h
man wpa2-halfhandshake-crack
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Test only your own APs or approved wireless ranges.
2. Confirm adapter/driver support first.
3. Start with passive discovery and signal analysis.
4. Use findings to improve WPA settings, firmware, segmentation, and monitoring.

## Example commands

```bash
wpa2-halfhandshake-crack --help
```

```bash
wpa2-halfhandshake-crack -h
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
