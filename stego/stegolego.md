# stegolego

**Category:** `stego`  
**Version in source list:** `8.85354f6`  
**Package name:** `stegolego`

## What it does

Simple program for using stegonography to hide data within BMP images.

## What it can be used for

Finding or extracting hidden data in images, files, audio, or other carriers.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed stegolego
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql stegolego | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
stegolego --help
stegolego -h
man stegolego
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on copies of images/audio/documents.
2. Check file type, metadata, and visible strings first.
3. Run extraction/detection tools and compare outputs.
4. Document discovered payloads or absence of evidence.

## Example commands

```bash
stegolego --help
```

```bash
stegolego -h
```

```bash
file ./sample.png
```

```bash
# Local sample pattern:
stegolego ./sample.png
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
