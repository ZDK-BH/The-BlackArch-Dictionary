# steghide

**Category:** `stego`  
**Version in source list:** `0.5.1`  
**Package name:** `steghide`

## What it does

Embeds a message in a file by replacing some of the least significant bits.

## What it can be used for

Finding or extracting hidden data in images, files, audio, or other carriers.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed steghide
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql steghide | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
steghide --help
steghide -h
man steghide
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on copies of images/audio/documents.
2. Check file type, metadata, and visible strings first.
3. Run extraction/detection tools and compare outputs.
4. Document discovered payloads or absence of evidence.

## Example commands

```bash
steghide --help
```

```bash
steghide -h
```

```bash
file ./sample.png
```

```bash
# Local sample pattern:
steghide ./sample.png
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
