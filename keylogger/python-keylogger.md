# python-keylogger

**Category:** `keylogger`  
**Version in source list:** `2.7.3`  
**Package name:** `python-keylogger`

## What it does

Simple keystroke logger.

## What it can be used for

Studying keylogger behavior for detection engineering and awareness training.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed python-keylogger
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql python-keylogger | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
python-keylogger --help
python-keylogger -h
man python-keylogger
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use isolated lab VMs only.
2. Do not deploy on anyone’s real system.
3. Focus on identifying files, processes, permissions, and network behavior.
4. Use findings to build detections and hardening rules.

## Example commands

```bash
python-keylogger --help
```

```bash
python-keylogger -h
```

```bash
# Defensive review helpers:
ps aux | head
find . -maxdepth 2 -type f | sort
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
