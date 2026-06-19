# pcileech

**Category:** `hardware`  
**Version in source list:** `4.19.5`  
**Package name:** `pcileech`

## What it does

Tool, which uses PCIe hardware devices to read and write from the target system memory.

## What it can be used for

Firmware, chipset, bus, boot, platform, or device security testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed pcileech
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql pcileech | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
pcileech --help
pcileech -h
man pcileech
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Read documentation carefully because hardware tools can affect system stability.
2. Run read-only checks first.
3. Save logs before making changes.
4. Use results to patch firmware, lock BIOS/UEFI settings, and improve physical security.

## Example commands

```bash
pcileech --help
```

```bash
pcileech -h
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
