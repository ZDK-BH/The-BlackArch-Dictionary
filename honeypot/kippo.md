# kippo

**Category:** `honeypot`  
**Version in source list:** `287.b9eb06a`  
**Package name:** `kippo`

## What it does

A medium interaction SSH honeypot designed to log brute force attacks and most importantly, the entire shell interaction by the attacker.

## What it can be used for

Deploying decoy services/sensors to collect telemetry and study attacker behavior.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed kippo
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql kippo | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
kippo --help
kippo -h
man kippo
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Deploy in a segmented VM/container, not on your daily machine.
2. Restrict outbound traffic so a compromise cannot pivot.
3. Enable logging and rotate logs.
4. Review captured events and create detections.

## Example commands

```bash
kippo --help
```

```bash
kippo -h
```

```bash
# Prep a lab folder:
mkdir -p honeypot-logs
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
