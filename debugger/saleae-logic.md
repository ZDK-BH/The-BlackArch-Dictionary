# saleae-logic

**Category:** `debugger`  
**Version in source list:** `2.3.47`  
**Package name:** `saleae-logic`

## What it does

Debug happy.

## What it can be used for

Tracing programs, debugging crashes, exploit research, and malware behavior study.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed saleae-logic
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql saleae-logic | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
saleae-logic --help
saleae-logic -h
man saleae-logic
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Run inside a VM when debugging untrusted software.
2. Copy the binary and symbols into a working directory.
3. Start the debugger, set breakpoints, and observe crashes or code paths.
4. Use notes to understand behavior or create a patch.

## Example commands

```bash
saleae-logic --help
```

```bash
saleae-logic -h
```

```bash
# Local debugging pattern:
saleae-logic ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
