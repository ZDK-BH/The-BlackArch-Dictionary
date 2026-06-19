# bytecode-viewer

**Category:** `binary`  
**Version in source list:** `2.12`  
**Package name:** `bytecode-viewer`

## What it does

A Java 8/Android APK Reverse Engineering Suite.

## What it can be used for

Static/dynamic analysis of binaries, exploit research, patch diffing, and malware triage.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed bytecode-viewer
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql bytecode-viewer | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
bytecode-viewer --help
bytecode-viewer -h
man bytecode-viewer
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Work on a copied sample, never the only copy of a binary.
2. Start with file identification, strings, metadata, and help output.
3. Open the sample in the tool and record architecture, imports, functions, and suspicious behavior.
4. Use results to understand software behavior or verify patches.

## Example commands

```bash
bytecode-viewer --help
```

```bash
bytecode-viewer -h
```

```bash
# Typical local sample pattern:
bytecode-viewer ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
