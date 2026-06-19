# c7decrypt

**Category:** `crypto`  
**Version in source list:** `0.3.3`  
**Package name:** `c7decrypt`

## What it does

Cisco password type encryptor and decryptor.

## What it can be used for

Encoding/decoding, cipher checks, key or hash analysis, certificate review, and crypto implementation testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed c7decrypt
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql c7decrypt | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
c7decrypt --help
c7decrypt -h
man c7decrypt
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work with your own ciphertext, test vectors, or CTF challenge files.
2. Identify input and output formats first.
3. Run the smallest possible sample to verify syntax.
4. Record commands so successful decoding/decryption steps are reproducible.

## Example commands

```bash
c7decrypt --help
```

```bash
c7decrypt -h
```

```bash
# Local sample pattern:
echo "test" | c7decrypt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
