# snare

**Category:** `honeypot`  
**Version in source list:** `188.b17fdfe`  
**Package name:** `snare`

## What it does

Super Next generation Advanced Reactive honeypot.

## What it can be used for

Deploying decoy services/sensors to collect telemetry and study attacker behavior.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed snare
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql snare | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
snare --help
snare -h
man snare
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Deploy in a segmented VM/container, not on your daily machine.
2. Restrict outbound traffic so a compromise cannot pivot.
3. Enable logging and rotate logs.
4. Review captured events and create detections.

## Example commands

```bash
snare --help
```

```bash
snare -h
```

```bash
# Prep a lab folder:
mkdir -p honeypot-logs
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
