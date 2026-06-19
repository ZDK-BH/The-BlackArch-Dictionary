# meanalyzer

**Category:** `firmware`  
**Version in source list:** `1.273.0`  
**Package name:** `meanalyzer`

## What it does

Intel Engine Firmware Analysis Tool.

## What it can be used for

Extracting, inspecting, emulating, or assessing firmware images.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed meanalyzer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql meanalyzer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
meanalyzer --help
meanalyzer -h
man meanalyzer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on firmware images from devices you own or vendor downloads.
2. Hash the original firmware before analysis.
3. Extract contents into a separate folder.
4. Review services, certificates, passwords, scripts, and update mechanisms.

## Example commands

```bash
meanalyzer --help
```

```bash
meanalyzer -h
```

```bash
# Local firmware pattern:
meanalyzer ./firmware.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
