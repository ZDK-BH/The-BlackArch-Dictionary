# heaptrace

**Category:** `debugger`  
**Version in source list:** `2.2.8.2.r20.g06f43fc`  
**Package name:** `heaptrace`

## What it does

Helps visualize heap operations for pwn and debugging.

## What it can be used for

Tracing programs, debugging crashes, exploit research, and malware behavior study.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed heaptrace
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql heaptrace | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
heaptrace --help
heaptrace -h
man heaptrace
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run inside a VM when debugging untrusted software.
2. Copy the binary and symbols into a working directory.
3. Start the debugger, set breakpoints, and observe crashes or code paths.
4. Use notes to understand behavior or create a patch.

## Example commands

```bash
heaptrace --help
```

```bash
heaptrace -h
```

```bash
# Local debugging pattern:
heaptrace ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
