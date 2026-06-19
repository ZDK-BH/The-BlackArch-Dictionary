# ubertooth

**Category:** `bluetooth`  
**Version in source list:** `2020.12.R1.r35.gc9dfdbd`  
**Package name:** `ubertooth`

## What it does

A 2.4 GHz wireless development board suitable for Bluetooth experimentation. Open source hardware and software. Tools only.

## What it can be used for

Bluetooth/BLE discovery, protocol analysis, device inventory, and lab pairing security tests.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed ubertooth
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql ubertooth | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
ubertooth --help
ubertooth -h
man ubertooth
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only Bluetooth devices you own or have permission to test.
2. Confirm your adapter is visible with bluetoothctl or hciconfig/iw tools.
3. Start with passive discovery or read-only inventory features.
4. Document device names, addresses, services, and firmware versions for hardening.

## Example commands

```bash
ubertooth --help
```

```bash
ubertooth -h
```

```bash
bluetoothctl show
```

```bash
# Lab inventory pattern:
ubertooth --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
