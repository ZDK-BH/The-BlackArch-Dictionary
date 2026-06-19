# lfle

**Category:** `forensic`  
**Version in source list:** `24.f28592c`  
**Package name:** `lfle`

## What it does

Recover event log entries from an image by heurisitically looking for record structures.

## What it can be used for

Disk, memory, browser, log, file, and mobile artifact analysis; evidence review and incident investigation.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed lfle
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql lfle | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
lfle --help
lfle -h
man lfle
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Preserve originals and analyze copies only.
2. Hash evidence before and after copying.
3. Use read-only mounts where possible.
4. Export findings to a case folder with timestamps and notes.

## Example commands

```bash
lfle --help
```

```bash
lfle -h
```

```bash
sha256sum ./evidence.img
```

```bash
# Local evidence-copy pattern:
lfle ./evidence-copy.img
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
