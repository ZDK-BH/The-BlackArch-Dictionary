# cryptohazemultiforcer

**Category:** `cracker`  
**Version in source list:** `1.31a`  
**Package name:** `cryptohazemultiforcer`

## What it does

High performance multihash brute forcer with CUDA support.

## What it can be used for

Testing password strength, recovering owned encrypted material, and auditing hashes or credentials supplied for an approved assessment.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed cryptohazemultiforcer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql cryptohazemultiforcer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
cryptohazemultiforcer --help
cryptohazemultiforcer -h
man cryptohazemultiforcer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only hashes, captures, archives, or credentials you own or are explicitly authorized to audit.
2. Prefer offline test data and small sample files first.
3. Keep wordlists legal and relevant to the audit objective.
4. Use results to improve password policy, MFA, lockouts, and monitoring.

## Example commands

```bash
cryptohazemultiforcer --help
```

```bash
cryptohazemultiforcer -h
```

```bash
# Offline lab pattern only:
cryptohazemultiforcer ./sample_hashes.txt ./wordlist.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
