# nfcutils

**Category:** `nfc`  
**Version in source list:** `61.49aa178`  
**Package name:** `nfcutils`

## What it does

A simple command that lists tags which are in your NFC device field.

## What it can be used for

Testing NFC/RFID systems, cards, readers, and lab emulation scenarios.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed nfcutils
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql nfcutils | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
nfcutils --help
nfcutils -h
man nfcutils
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only tags/cards/readers you own or have permission to test.
2. Start with read-only identification.
3. Keep dumps secure and labeled.
4. Use findings to choose stronger tags or access controls.

## Example commands

```bash
nfcutils --help
```

```bash
nfcutils -h
```

```bash
lsusb
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
