# sipbrute

**Category:** `voip`  
**Version in source list:** `11.5be2fdd`  
**Package name:** `sipbrute`

## What it does

A utility to perform dictionary attacks against the VoIP SIP Register hash.

## What it can be used for

Testing SIP/VoIP configuration, enumeration, signaling, and call-system security in an approved lab.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sipbrute
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sipbrute | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sipbrute --help
sipbrute -h
man sipbrute
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only your own PBX, lab SIP server, or approved scope.
2. Start with inventory/fingerprinting features.
3. Avoid disrupting live phone systems.
4. Use findings to harden authentication, TLS/SRTP, and exposure.

## Example commands

```bash
sipbrute --help
```

```bash
sipbrute -h
```

```bash
# Lab VoIP prep:
ss -tulpn | grep -E "5060|5061" || true
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
