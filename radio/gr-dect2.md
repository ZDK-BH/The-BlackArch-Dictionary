# gr-dect2

**Category:** `radio`  
**Version in source list:** `39.0d973fe`  
**Package name:** `gr-dect2`

## What it does

Real-time DECT voice channel decoding by Gnuradio.

## What it can be used for

Signal decoding, RF monitoring, and protocol experiments using SDR hardware.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed gr-dect2
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql gr-dect2 | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
gr-dect2 --help
gr-dect2 -h
man gr-dect2
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Check your local radio regulations before transmitting anything.
2. Start with receive-only examples.
3. Verify SDR hardware is detected.
4. Record metadata such as frequency, sample rate, and antenna setup.

## Example commands

```bash
gr-dect2 --help
```

```bash
gr-dect2 -h
```

```bash
lsusb
```

```bash
# Receive-only lab pattern after docs:
gr-dect2 --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
