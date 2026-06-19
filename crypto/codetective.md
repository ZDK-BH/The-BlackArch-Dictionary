# codetective

**Category:** `crypto`  
**Version in source list:** `45.52b91f1`  
**Package name:** `codetective`

## What it does

A tool to determine the crypto/encoding algorithm used according to traces of its representation.

## What it can be used for

Encoding/decoding, cipher checks, key or hash analysis, certificate review, and crypto implementation testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed codetective
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql codetective | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
codetective --help
codetective -h
man codetective
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work with your own ciphertext, test vectors, or CTF challenge files.
2. Identify input and output formats first.
3. Run the smallest possible sample to verify syntax.
4. Record commands so successful decoding/decryption steps are reproducible.

## Example commands

```bash
codetective --help
```

```bash
codetective -h
```

```bash
# Local sample pattern:
echo "test" | codetective
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
