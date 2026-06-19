# secure-delete

**Category:** `anti-forensic`  
**Version in source list:** `1.b63d814`  
**Package name:** `secure-delete`

## What it does

Secure file, disk, swap, memory erasure utilities.

## What it can be used for

Understanding evidence-tampering techniques so defenders can detect and prevent them.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed secure-delete
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql secure-delete | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
secure-delete --help
secure-delete -h
man secure-delete
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use isolated lab systems only.
2. Study behavior to improve logging, backups, and evidence preservation.
3. Avoid running destructive functions on real systems.
4. Record indicators that defenders can monitor.

## Example commands

```bash
secure-delete --help
```

```bash
secure-delete -h
```

```bash
# Defensive baseline:
journalctl -n 50 --no-pager
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
