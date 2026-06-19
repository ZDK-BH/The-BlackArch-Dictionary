# gpredict

**Category:** `radio`  
**Version in source list:** `1692.59476d4`  
**Package name:** `gpredict`

## What it does

A real-time satellite tracking and orbit prediction application.

## What it can be used for

Signal decoding, RF monitoring, and protocol experiments using SDR hardware.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed gpredict
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql gpredict | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
gpredict --help
gpredict -h
man gpredict
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Check your local radio regulations before transmitting anything.
2. Start with receive-only examples.
3. Verify SDR hardware is detected.
4. Record metadata such as frequency, sample rate, and antenna setup.

## Example commands

```bash
gpredict --help
```

```bash
gpredict -h
```

```bash
lsusb
```

```bash
# Receive-only lab pattern after docs:
gpredict --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
