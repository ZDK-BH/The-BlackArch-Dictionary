# pre2k

**Category:** `windows`  
**Version in source list:** `24.ff51b3b`  
**Package name:** `pre2k`

## What it does

Query for existence of pre-windows 2000 computer objects which can be leveraged to gain a foothold in a target domain.

## What it can be used for

Windows administration, audit, forensics, reverse engineering, credential-risk review, or post-compromise simulation in a lab.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed pre2k
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql pre2k | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
pre2k --help
pre2k -h
man pre2k
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use a Windows lab VM or approved enterprise test environment.
2. Snapshot before running unfamiliar tools.
3. Read help and inspect files before execution.
4. Use results to harden AD, endpoints, logs, and permissions.

## Example commands

```bash
pre2k --help
```

```bash
pre2k -h
```

```bash
# Package contents:
pacman -Ql pre2k | sed -n "1,80p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
