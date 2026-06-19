# passe-partout

**Category:** `cracker`  
**Version in source list:** `0.1`  
**Package name:** `passe-partout`

## What it does

Tool to extract RSA and DSA private keys from any process linked with OpenSSL. The target memory is scanned to lookup specific OpenSSL patterns.

## What it can be used for

Testing password strength, recovering owned encrypted material, and auditing hashes or credentials supplied for an approved assessment.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed passe-partout
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql passe-partout | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
passe-partout --help
passe-partout -h
man passe-partout
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only hashes, captures, archives, or credentials you own or are explicitly authorized to audit.
2. Prefer offline test data and small sample files first.
3. Keep wordlists legal and relevant to the audit objective.
4. Use results to improve password policy, MFA, lockouts, and monitoring.

## Example commands

```bash
passe-partout --help
```

```bash
passe-partout -h
```

```bash
# Offline lab pattern only:
passe-partout ./sample_hashes.txt ./wordlist.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
