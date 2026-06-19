# dc3dd

**Category:** `forensic`  
**Version in source list:** `7.2.646`  
**Package name:** `dc3dd`

## What it does

A patched version of dd that includes a number of features useful for computer forensics.

## What it can be used for

Disk, memory, browser, log, file, and mobile artifact analysis; evidence review and incident investigation.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed dc3dd
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql dc3dd | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
dc3dd --help
dc3dd -h
man dc3dd
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Preserve originals and analyze copies only.
2. Hash evidence before and after copying.
3. Use read-only mounts where possible.
4. Export findings to a case folder with timestamps and notes.

## Example commands

```bash
dc3dd --help
```

```bash
dc3dd -h
```

```bash
sha256sum ./evidence.img
```

```bash
# Local evidence-copy pattern:
dc3dd ./evidence-copy.img
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
