# missionplanner

**Category:** `drone`  
**Version in source list:** `1.3.83`  
**Package name:** `missionplanner`

## What it does

A GroundControl Station for Ardupilot.

## What it can be used for

Drone communication/protocol security research and lab assessment.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed missionplanner
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql missionplanner | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
missionplanner --help
missionplanner -h
man missionplanner
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use owned drones/controllers or simulators only.
2. Keep tests in a safe physical space and comply with local rules.
3. Start with passive observation and logs.
4. Use results to improve firmware, pairing, and network settings.

## Example commands

```bash
missionplanner --help
```

```bash
missionplanner -h
```

```bash
# Lab prep:
ip addr
rfkill list
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
