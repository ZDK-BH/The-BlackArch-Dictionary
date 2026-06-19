# bluphish

**Category:** `bluetooth`  
**Version in source list:** `9.a7200bd`  
**Package name:** `bluphish`

## What it does

Bluetooth device and service discovery tool that can be used for security assessment and penetration testing.

## What it can be used for

Bluetooth/BLE discovery, protocol analysis, device inventory, and lab pairing security tests.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed bluphish
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql bluphish | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
bluphish --help
bluphish -h
man bluphish
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only Bluetooth devices you own or have permission to test.
2. Confirm your adapter is visible with bluetoothctl or hciconfig/iw tools.
3. Start with passive discovery or read-only inventory features.
4. Document device names, addresses, services, and firmware versions for hardening.

## Example commands

```bash
bluphish --help
```

```bash
bluphish -h
```

```bash
bluetoothctl show
```

```bash
# Lab inventory pattern:
bluphish --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
