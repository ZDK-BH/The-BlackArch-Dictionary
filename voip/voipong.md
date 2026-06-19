# voipong

**Category:** `voip`  
**Version in source list:** `2.0`  
**Package name:** `voipong`

## What it does

A utility which detects all Voice Over IP calls on a pipeline, and for those which are G711 encoded, dumps actual conversation to separate wave files.

## What it can be used for

Testing SIP/VoIP configuration, enumeration, signaling, and call-system security in an approved lab.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed voipong
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql voipong | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
voipong --help
voipong -h
man voipong
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use only your own PBX, lab SIP server, or approved scope.
2. Start with inventory/fingerprinting features.
3. Avoid disrupting live phone systems.
4. Use findings to harden authentication, TLS/SRTP, and exposure.

## Example commands

```bash
voipong --help
```

```bash
voipong -h
```

```bash
# Lab VoIP prep:
ss -tulpn | grep -E "5060|5061" || true
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
