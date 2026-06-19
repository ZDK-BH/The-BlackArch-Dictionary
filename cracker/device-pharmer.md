# device-pharmer

**Category:** `cracker`  
**Version in source list:** `40.b06a460`  
**Package name:** `device-pharmer`

## What it does

Opens 1K+ IPs or Shodan search results and attempts to login.

## What it can be used for

Testing password strength, recovering owned encrypted material, and auditing hashes or credentials supplied for an approved assessment.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed device-pharmer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql device-pharmer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
device-pharmer --help
device-pharmer -h
man device-pharmer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only hashes, captures, archives, or credentials you own or are explicitly authorized to audit.
2. Prefer offline test data and small sample files first.
3. Keep wordlists legal and relevant to the audit objective.
4. Use results to improve password policy, MFA, lockouts, and monitoring.

## Example commands

```bash
device-pharmer --help
```

```bash
device-pharmer -h
```

```bash
# Offline lab pattern only:
device-pharmer ./sample_hashes.txt ./wordlist.txt
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
