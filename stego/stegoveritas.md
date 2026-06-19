# stegoveritas

**Category:** `stego`  
**Version in source list:** `1.10`  
**Package name:** `stegoveritas`

## What it does

Automatic image steganography analysis tool.

## What it can be used for

Finding or extracting hidden data in images, files, audio, or other carriers.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed stegoveritas
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql stegoveritas | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
stegoveritas --help
stegoveritas -h
man stegoveritas
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on copies of images/audio/documents.
2. Check file type, metadata, and visible strings first.
3. Run extraction/detection tools and compare outputs.
4. Document discovered payloads or absence of evidence.

## Example commands

```bash
stegoveritas --help
```

```bash
stegoveritas -h
```

```bash
file ./sample.png
```

```bash
# Local sample pattern:
stegoveritas ./sample.png
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
