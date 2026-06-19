# mp3nema

**Category:** `forensic`  
**Version in source list:** `0.4`  
**Package name:** `mp3nema`

## What it does

A tool aimed at analyzing and capturing data that is hidden between frames in an MP3 file or stream, otherwise noted as "out of band" data.

## What it can be used for

Disk, memory, browser, log, file, and mobile artifact analysis; evidence review and incident investigation.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed mp3nema
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql mp3nema | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
mp3nema --help
mp3nema -h
man mp3nema
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Preserve originals and analyze copies only.
2. Hash evidence before and after copying.
3. Use read-only mounts where possible.
4. Export findings to a case folder with timestamps and notes.

## Example commands

```bash
mp3nema --help
```

```bash
mp3nema -h
```

```bash
sha256sum ./evidence.img
```

```bash
# Local evidence-copy pattern:
mp3nema ./evidence-copy.img
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
