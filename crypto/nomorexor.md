# nomorexor

**Category:** `crypto`  
**Version in source list:** `2.84489f9`  
**Package name:** `nomorexor`

## What it does

Tool to help guess a files 256 byte XOR key by using frequency analysis.

## What it can be used for

Encoding/decoding, cipher checks, key or hash analysis, certificate review, and crypto implementation testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed nomorexor
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql nomorexor | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
nomorexor --help
nomorexor -h
man nomorexor
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work with your own ciphertext, test vectors, or CTF challenge files.
2. Identify input and output formats first.
3. Run the smallest possible sample to verify syntax.
4. Record commands so successful decoding/decryption steps are reproducible.

## Example commands

```bash
nomorexor --help
```

```bash
nomorexor -h
```

```bash
# Local sample pattern:
echo "test" | nomorexor
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
