# firmware-mod-kit

**Category:** `firmware`  
**Version in source list:** `0.99.r119.gc72f45d`  
**Package name:** `firmware-mod-kit`

## What it does

Modify firmware images without recompiling.

## What it can be used for

Extracting, inspecting, emulating, or assessing firmware images.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed firmware-mod-kit
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql firmware-mod-kit | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
firmware-mod-kit --help
firmware-mod-kit -h
man firmware-mod-kit
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on firmware images from devices you own or vendor downloads.
2. Hash the original firmware before analysis.
3. Extract contents into a separate folder.
4. Review services, certificates, passwords, scripts, and update mechanisms.

## Example commands

```bash
firmware-mod-kit --help
```

```bash
firmware-mod-kit -h
```

```bash
# Local firmware pattern:
firmware-mod-kit ./firmware.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
