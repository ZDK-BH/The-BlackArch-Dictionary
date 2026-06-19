# pstoreview

**Category:** `windows`  
**Version in source list:** `1.0`  
**Package name:** `pstoreview`

## What it does

Lists the contents of the Protected Storage.

## What it can be used for

Windows administration, audit, forensics, reverse engineering, credential-risk review, or post-compromise simulation in a lab.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed pstoreview
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql pstoreview | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
pstoreview --help
pstoreview -h
man pstoreview
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use a Windows lab VM or approved enterprise test environment.
2. Snapshot before running unfamiliar tools.
3. Read help and inspect files before execution.
4. Use results to harden AD, endpoints, logs, and permissions.

## Example commands

```bash
pstoreview --help
```

```bash
pstoreview -h
```

```bash
# Package contents:
pacman -Ql pstoreview | sed -n "1,80p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
