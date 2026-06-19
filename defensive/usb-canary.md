# usb-canary

**Category:** `defensive`  
**Version in source list:** `31.bb23552`  
**Package name:** `usb-canary`

## What it does

A Linux or OSX tool that uses psutil to monitor devices while your computer is locked. In the case it detects someone plugging in or unplugging devices it can be configured to send you an SMS or alert you via Slack or Pushover.

## What it can be used for

Hardening, monitoring, detection, honeypot support, rootkit checks, and defensive analysis.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed usb-canary
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql usb-canary | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
usb-canary --help
usb-canary -h
man usb-canary
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run from a trusted environment where possible.
2. Update signatures/rules if the tool supports it.
3. Save reports to a timestamped folder.
4. Treat alerts as leads and verify with additional evidence.

## Example commands

```bash
usb-canary --help
```

```bash
usb-canary -h
```

```bash
# Defensive scan/report pattern:
usb-canary --help
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
