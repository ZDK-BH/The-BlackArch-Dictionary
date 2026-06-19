# wifichannelmonitor

**Category:** `windows`  
**Version in source list:** `1.70`  
**Package name:** `wifichannelmonitor`

## What it does

A utility for Windows that captures wifi traffic on the channel you choose, using Microsoft Network Monitor capture driver.

## What it can be used for

Windows administration, audit, forensics, reverse engineering, credential-risk review, or post-compromise simulation in a lab.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed wifichannelmonitor
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql wifichannelmonitor | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
wifichannelmonitor --help
wifichannelmonitor -h
man wifichannelmonitor
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use a Windows lab VM or approved enterprise test environment.
2. Snapshot before running unfamiliar tools.
3. Read help and inspect files before execution.
4. Use results to harden AD, endpoints, logs, and permissions.

## Example commands

```bash
wifichannelmonitor --help
```

```bash
wifichannelmonitor -h
```

```bash
# Package contents:
pacman -Ql wifichannelmonitor | sed -n "1,80p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
