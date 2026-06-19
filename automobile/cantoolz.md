# cantoolz

**Category:** `automobile`  
**Version in source list:** `425.82d330b`  
**Package name:** `cantoolz`

## What it does

Framework for black-box CAN network analysis.

## What it can be used for

Vehicle bus/CAN protocol research and security testing in safe lab setups.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed cantoolz
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql cantoolz | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
cantoolz --help
cantoolz -h
man cantoolz
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use a simulator, bench setup, or vehicle you own with safety precautions.
2. Start in listen-only/read-only modes where available.
3. Log frames and annotate test conditions.
4. Do not test on public roads or safety-critical systems.

## Example commands

```bash
cantoolz --help
```

```bash
cantoolz -h
```

```bash
# CAN lab inventory:
ip link
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
