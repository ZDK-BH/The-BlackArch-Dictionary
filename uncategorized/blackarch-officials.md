# blackarch-officials

**Category:** `uncategorized`  
**Version in source list:** `20260407`  
**Package name:** `blackarch-officials`

## What it does

Meta package for installing official security tools from the Arch Linux repository.

## What it can be used for

General security-related tasks; exact purpose depends on the tool.

## How to install

On BlackArch or Arch with the BlackArch repo enabled:

```bash
sudo pacman -S --needed blackarch-officials
```

Confirm the installed files and find the actual executable name:

```bash
pacman -Ql blackarch-officials | grep '/bin/'
```

Open the built-in help before running anything meaningful:

```bash
blackarch-officials --help
blackarch-officials -h
man blackarch-officials
```

If the command name is different from the package name, use the executable shown by `pacman -Ql`.

## How to use it

1. Install only if you know why you need it.
2. Inspect package files and documentation.
3. Run help/version commands first.
4. Use a lab VM for unknown or unfamiliar tools.

## Example commands

```bash
blackarch-officials --help
```

```bash
blackarch-officials -h
```

```bash
pacman -Ql blackarch-officials | sed -n "1,120p"
```

## Notes

- Start with `--help`, `-h`, or the man page because options differ between tools and versions.
- Prefer a VM, local lab target, copied evidence file, or test repository for first runs.
- Save outputs with timestamps so you can compare results after fixes or configuration changes.
