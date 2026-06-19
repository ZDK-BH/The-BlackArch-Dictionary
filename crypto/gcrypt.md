# gcrypt

**Category:** `crypto`  
**Version in source list:** `32.d3f9f06`  
**Package name:** `gcrypt`

## What it does

Simple, secure and performance file encryption tool written in C

## What it can be used for

Encoding/decoding, cipher checks, key or hash analysis, certificate review, and crypto implementation testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed gcrypt
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql gcrypt | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
gcrypt --help
gcrypt -h
man gcrypt
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work with your own ciphertext, test vectors, or CTF challenge files.
2. Identify input and output formats first.
3. Run the smallest possible sample to verify syntax.
4. Record commands so successful decoding/decryption steps are reproducible.

## Example commands

```bash
gcrypt --help
```

```bash
gcrypt -h
```

```bash
# Local sample pattern:
echo "test" | gcrypt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
