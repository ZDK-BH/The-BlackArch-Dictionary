# sipp

**Category:** `voip`  
**Version in source list:** `1574.5c4e8dc`  
**Package name:** `sipp`

## What it does

A free Open Source test tool / traffic generator for the SIP protocol.

## What it can be used for

Testing SIP/VoIP configuration, enumeration, signaling, and call-system security in an approved lab.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sipp
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sipp | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sipp --help
sipp -h
man sipp
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only your own PBX, lab SIP server, or approved scope.
2. Start with inventory/fingerprinting features.
3. Avoid disrupting live phone systems.
4. Use findings to harden authentication, TLS/SRTP, and exposure.

## Example commands

```bash
sipp --help
```

```bash
sipp -h
```

```bash
# Lab VoIP prep:
ss -tulpn | grep -E "5060|5061" || true
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
