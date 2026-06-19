# stegseek

**Category:** `stego`  
**Version in source list:** `v0.6.r10.g5896978`  
**Package name:** `stegseek`

## What it does

Lightning fast steghide cracker.

## What it can be used for

Finding or extracting hidden data in images, files, audio, or other carriers.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed stegseek
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql stegseek | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
stegseek --help
stegseek -h
man stegseek
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on copies of images/audio/documents.
2. Check file type, metadata, and visible strings first.
3. Run extraction/detection tools and compare outputs.
4. Document discovered payloads or absence of evidence.

## Example commands

```bash
stegseek --help
```

```bash
stegseek -h
```

```bash
file ./sample.png
```

```bash
# Local sample pattern:
stegseek ./sample.png
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
