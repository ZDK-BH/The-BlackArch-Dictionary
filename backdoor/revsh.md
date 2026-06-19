# revsh

**Category:** `backdoor`  
**Version in source list:** `215.174e309`  
**Package name:** `revsh`

## What it does

A reverse shell with terminal support, data tunneling, and advanced pivoting capabilities.

## What it can be used for

Understanding backdoor behavior, writing detections, and practicing incident response in an isolated malware lab.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed revsh
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql revsh | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
revsh --help
revsh -h
man revsh
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use an isolated VM or disposable lab network only.
2. Do not run samples on your daily machine.
3. Prefer static analysis, help output, and documentation review before execution.
4. Capture indicators, process behavior, file writes, and network attempts for defensive learning.

## Example commands

```bash
revsh --help
```

```bash
revsh -h
```

```bash
# Defensive lab workflow:
strings /path/to/sample 2>/dev/null | head
file /path/to/sample
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
