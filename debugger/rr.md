# rr

**Category:** `debugger`  
**Version in source list:** `6869.556551e4`  
**Package name:** `rr`

## What it does

A Record and Replay Framework.

## What it can be used for

Tracing programs, debugging crashes, exploit research, and malware behavior study.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed rr
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql rr | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
rr --help
rr -h
man rr
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run inside a VM when debugging untrusted software.
2. Copy the binary and symbols into a working directory.
3. Start the debugger, set breakpoints, and observe crashes or code paths.
4. Use notes to understand behavior or create a patch.

## Example commands

```bash
rr --help
```

```bash
rr -h
```

```bash
# Local debugging pattern:
rr ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
