# limeaide

**Category:** `forensic`  
**Version in source list:** `v2.0.0.r3.gce3c9b7`  
**Package name:** `limeaide`

## What it does

Remotely dump RAM of a Linux client and create a volatility profile for later analysis on your local host.

## What it can be used for

Disk, memory, browser, log, file, and mobile artifact analysis; evidence review and incident investigation.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed limeaide
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql limeaide | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
limeaide --help
limeaide -h
man limeaide
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Preserve originals and analyze copies only.
2. Hash evidence before and after copying.
3. Use read-only mounts where possible.
4. Export findings to a case folder with timestamps and notes.

## Example commands

```bash
limeaide --help
```

```bash
limeaide -h
```

```bash
sha256sum ./evidence.img
```

```bash
# Local evidence-copy pattern:
limeaide ./evidence-copy.img
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
