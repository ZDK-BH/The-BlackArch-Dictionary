# smbclient-ng

**Category:** `networking`  
**Version in source list:** `3.0.0.r11.g1970cc6`  
**Package name:** `smbclient-ng`

## What it does

Interact with SMB shares.

## What it can be used for

Protocol testing, service diagnostics, routing/tunneling labs, packet handling, and network behavior analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed smbclient-ng
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql smbclient-ng | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
smbclient-ng --help
smbclient-ng -h
man smbclient-ng
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Identify your interface and lab network first.
2. Use read-only/listen modes where available.
3. Keep tests inside owned or authorized networks.
4. Save packet captures/logs for review.

## Example commands

```bash
smbclient-ng --help
```

```bash
smbclient-ng -h
```

```bash
ip addr
```

```bash
ss -tulpn
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
