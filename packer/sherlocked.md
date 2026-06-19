# sherlocked

**Category:** `packer`  
**Version in source list:** `1.f190c2b`  
**Package name:** `sherlocked`

## What it does

Universal script packer-- transforms any type of script into a protected ELF executable, encrypted with anti-debugging.

## What it can be used for

Studying binary packing, obfuscation, and unpacking for malware/reversing workflows.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed sherlocked
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql sherlocked | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
sherlocked --help
sherlocked -h
man sherlocked
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Use local sample binaries only.
2. Hash the original and packed/unpacked outputs.
3. Compare file sections, strings, and detection behavior.
4. Use observations to improve static-analysis workflows.

## Example commands

```bash
sherlocked --help
```

```bash
sherlocked -h
```

```bash
# Local sample pattern:
sherlocked ./sample.bin
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
