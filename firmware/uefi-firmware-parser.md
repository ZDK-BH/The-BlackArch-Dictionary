# uefi-firmware-parser

**Category:** `firmware`  
**Version in source list:** `214.86d2834`  
**Package name:** `uefi-firmware-parser`

## What it does

Parse BIOS/Intel ME/UEFI firmware related structures: Volumes, FileSystems, Files, etc.

## What it can be used for

Extracting, inspecting, emulating, or assessing firmware images.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed uefi-firmware-parser
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql uefi-firmware-parser | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
uefi-firmware-parser --help
uefi-firmware-parser -h
man uefi-firmware-parser
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on firmware images from devices you own or vendor downloads.
2. Hash the original firmware before analysis.
3. Extract contents into a separate folder.
4. Review services, certificates, passwords, scripts, and update mechanisms.

## Example commands

```bash
uefi-firmware-parser --help
```

```bash
uefi-firmware-parser -h
```

```bash
# Local firmware pattern:
uefi-firmware-parser ./firmware.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
