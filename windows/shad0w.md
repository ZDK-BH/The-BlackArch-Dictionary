# shad0w

**Category:** `windows`  
**Version in source list:** `387.d35b9dc`  
**Package name:** `shad0w`

## What it does

A modular C2 framework designed to successfully operate on mature environments.

## What it can be used for

Windows administration, audit, forensics, reverse engineering, credential-risk review, or post-compromise simulation in a lab.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed shad0w
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql shad0w | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
shad0w --help
shad0w -h
man shad0w
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use a Windows lab VM or approved enterprise test environment.
2. Snapshot before running unfamiliar tools.
3. Read help and inspect files before execution.
4. Use results to harden AD, endpoints, logs, and permissions.

## Example commands

```bash
shad0w --help
```

```bash
shad0w -h
```

```bash
# Package contents:
pacman -Ql shad0w | sed -n "1,80p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
