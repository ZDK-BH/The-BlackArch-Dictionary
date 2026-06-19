# protos-sip

**Category:** `voip`  
**Version in source list:** `2`  
**Package name:** `protos-sip`

## What it does

SIP test suite.

## What it can be used for

Testing SIP/VoIP configuration, enumeration, signaling, and call-system security in an approved lab.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed protos-sip
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql protos-sip | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
protos-sip --help
protos-sip -h
man protos-sip
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only your own PBX, lab SIP server, or approved scope.
2. Start with inventory/fingerprinting features.
3. Avoid disrupting live phone systems.
4. Use findings to harden authentication, TLS/SRTP, and exposure.

## Example commands

```bash
protos-sip --help
```

```bash
protos-sip -h
```

```bash
# Lab VoIP prep:
ss -tulpn | grep -E "5060|5061" || true
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
