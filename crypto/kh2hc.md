# kh2hc

**Category:** `crypto`  
**Version in source list:** `0.1.0.r2.g96b9e68`  
**Package name:** `kh2hc`

## What it does

Convert OpenSSH known_hosts file hashed with HashKnownHosts to hashes crackable by Hashcat.

## What it can be used for

Encoding/decoding, cipher checks, key or hash analysis, certificate review, and crypto implementation testing.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed kh2hc
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql kh2hc | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
kh2hc --help
kh2hc -h
man kh2hc
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work with your own ciphertext, test vectors, or CTF challenge files.
2. Identify input and output formats first.
3. Run the smallest possible sample to verify syntax.
4. Record commands so successful decoding/decryption steps are reproducible.

## Example commands

```bash
kh2hc --help
```

```bash
kh2hc -h
```

```bash
# Local sample pattern:
echo "test" | kh2hc
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
