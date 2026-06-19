# sagan

**Category:** `ids`  
**Version in source list:** `2.0.2`  
**Package name:** `sagan`

## What it does

A snort-like log analysis engine.

## What it can be used for

IDS testing, tuning, signature validation, and network defense.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sagan
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sagan | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sagan --help
sagan -h
man sagan
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Deploy sensors on networks you control.
2. Start with default rules/configuration.
3. Generate benign test traffic and confirm alerts.
4. Tune rules to reduce false positives and catch real issues.

## Example commands

```bash
sagan --help
```

```bash
sagan -h
```

```bash
# Sensor prep:
ip link
mkdir -p ids-logs
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
