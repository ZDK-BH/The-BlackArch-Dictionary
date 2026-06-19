# python2-pcodedmp

**Category:** `disassembler`  
**Version in source list:** `1.2.6`  
**Package name:** `python2-pcodedmp`

## What it does

A VBA p-code disassembler.

## What it can be used for

Inspecting machine code, bytecode, shellcode, firmware, and exploit/malware samples.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed python2-pcodedmp
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql python2-pcodedmp | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
python2-pcodedmp --help
python2-pcodedmp -h
man python2-pcodedmp
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Identify architecture and file type before disassembly.
2. Load the sample locally and inspect functions, strings, and cross-references.
3. Avoid executing unknown samples unless the lab is isolated.
4. Use analysis notes to understand control flow and patch impact.

## Example commands

```bash
python2-pcodedmp --help
```

```bash
python2-pcodedmp -h
```

```bash
# Local disassembly pattern:
python2-pcodedmp ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
