# pwd-hash

**Category:** `crypto`  
**Version in source list:** `2.0`  
**Package name:** `pwd-hash`

## What it does

A password hashing tool that use the crypt function to generate the hash of a string given on standard input.

## What it can be used for

Encoding/decoding, cipher checks, key or hash analysis, certificate review, and crypto implementation testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed pwd-hash
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql pwd-hash | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
pwd-hash --help
pwd-hash -h
man pwd-hash
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work with your own ciphertext, test vectors, or CTF challenge files.
2. Identify input and output formats first.
3. Run the smallest possible sample to verify syntax.
4. Record commands so successful decoding/decryption steps are reproducible.

## Example commands

```bash
pwd-hash --help
```

```bash
pwd-hash -h
```

```bash
# Local sample pattern:
echo "test" | pwd-hash
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
